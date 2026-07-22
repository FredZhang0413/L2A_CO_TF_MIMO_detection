# CM-MAE: 物理引导跨模态掩码自编码器预实验进展汇报

> ISAC系统中相机-mmWave信道跨模态表示学习

---

## 1. 研究动机与问题

在通感一体化（ISAC）系统中，视觉传感器（相机）和通信信道（mmWave CFR）天然蕴含互补的场景几何信息：
- 视觉：提供高分辨率纹理、语义信息（物体类别、遮挡关系）
- 信道：提供精确的空间传播信息（LoS/NLoS路径、AOA/AOD、时延）

**核心挑战**：两者模态差异极大（像素网格 vs. 复值频响），缺乏大规模配对标注数据，如何自监督地学习对齐的跨模态表示？

---

## 2. CM-MAE 方法概述

提出 **Physics-Grounded Cross-Modal Masked Autoencoder (CM-MAE)**：

1. **物理可解释的前端**：将复值信道频率响应（CFR）通过3D过采样DFT波束空间变换 + NMS连通域聚类，提取出物理传播路径簇（azimuth × elevation × delay），每个簇对应一条多径传播路径
2. **双ViT编码器**：视觉侧用PatchEmbed处理16×16图像块；CSI侧用ClusterEmbed处理3D波束空间小立方体，加入Fourier 3D位置编码和路径能量/质量嵌入
3. **联合Transformer解码器**：两种模态token拼接（带模态类型嵌入），用mask token替换被掩码位置，通过cross-attention实现跨模态信息补全
4. **四阶段课程学习**：从纯重建→全局对比对齐→几何引导掩码→细粒度路径-像素对应，逐步解锁跨模态能力
5. **弱监督变体(W)/无监督变体(U)**：W变体利用射线追踪几何标签训练OT对应头，U变体完全自监督

---

## 3. 模型架构

```
图像 I (B,3,224,224)               信道 CFR H (B,16,8,128,complex)
       │                                      │
       ▼                                      ▼
  PatchEmbed (16×16)                 3D Beamspace Transform
  + Ray Dir Encoding                 + NMS Cluster Extraction
       │                                      │
       ▼                                      ▼
  196 vision tokens                 Q variable CSI clusters
  (B,196,192)                       (B,Q,192) + padding mask
       │                                      │
       ▼                                      ▼
  ┌──────────────┐               ┌──────────────────┐
  │ Vision ViT   │◄── CLS token  │ CSI ViT Encoder  │◄── scale token
  │ Encoder (6L) │               │ (6 layers)       │   (no extra CLS)
  └──────┬───────┘               └────────┬─────────┘
         │                                │
         ▼                                ▼
    vis_cls (B,192)                 csi_scale (B,192)
    vis_tokens (B,196,192)          csi_tokens (B,Q,192)
         │                                │
         └────────────┬───────────────────┘
                      ▼
            ┌─────────────────────┐
            │  Joint Decoder (4L) │  mask tokens + cross-attn
            │  (vis + csi concat) │
            └──────────┬──────────┘
                       ▼
            ┌─────────────────────┐
            │ Reconstruction Heads│
            ├─────────────────────┤
            │ vis_head → pixels   │
            │ csi_head → beam cube│
            └─────────────────────┘
```

### 关键设计点
| 组件 | 设计 | 物理动机 |
|------|------|----------|
| Beamspace Transform | 过采样DFT字典 (N_az=128, N_el=64, N_tau=128) | 稀疏表示传播路径，避免分辨率损失 |
| NMS Clustering | 3D非极大值抑制 + 连通域标记 | 提取物理可解释的传播路径簇 |
| Fourier PosEnc | 随机Fourier特征编码(θ,φ,τ) | 适合3D角度-时延连续坐标 |
| Modality Emb | 可学习模态类型向量 | 区分视觉/CSI token |
| Dual Dustbin OT | Sinkhorn最优传输 + 双垃圾桶 | 处理无匹配的patch和cluster |
| Soft Contrastive | UE位置高斯核 + 信道余弦相似度 → soft target | 物理先验引导全局对齐 |

---

## 4. 四阶段课程训练策略

| 阶段 | Masking策略 | 损失函数 | 目标 |
|------|------------|----------|------|
| **A** (Warm-up) | 随机块掩码 (vis: 0.7, csi: 0.5) | L_rec_vis + β·L_rec_csi | 学习单模态基础表示和重建能力 |
| **B1** (Global Alignment) | 同A | L_rec + λ₂·L_ctr | 加入软对比损失，全局对齐两个模态的CLS token |
| **B2** (Geometry Mask) | 几何引导跨模态掩码（遮挡对应路径区域） | L_rec + λ₂·L_ctr | 强制模型利用跨模态信息补全被物理遮挡的区域 |
| **C** (Correspondence) | 同B2 | L_rec + λ₂·L_ctr + λ₃·L_OT | 加入OT路径-像素对应损失（W变体），学习细粒度对齐 |

---

## 5. 预实验完成情况

### ✅ 已完成工作

1. **完整CM-MAE框架搭建** (代码量约2000行)
   - `config.py` — 全参数配置（系统/场景/波束空间/模型/训练）
   - `beamspace.py` — 3D波束空间变换、NMS簇提取、归一化
   - `data.py` — 合成射线追踪数据集生成（CFR+图像+LoS/Dir/Refl几何标签）
   - `models.py` — PatchEmbed、ClusterEmbed（含cube MLP + Fourier PE）、双ViT编码器、JointDecoder（mask token + 模态嵌入）、Reconstruction Heads、OT Correspondence Head
   - `masking.py` — 随机掩码、坐标邻域掩码、几何引导跨模态掩码
   - `losses.py` — 软对比损失、掩码MSE重建损失、OT Sinkhorn损失、AUCpp指标
   - `train.py` — 四阶段课程训练主循环（cosine lr + warmup + grad clip）

2. **Bug修复与张量形状对齐**
   - 修复einsum维度错误（波束空间变换）
   - 修复CSI encoder双重CLS问题（scale token已充当全局token，设置`add_cls_token=False`）
   - 修复variable-length cluster padding mask处理
   - 修复OT损失tensor类型错误
   - 修复soft contrastive loss复数张量兼容性

3. **预实验
**
   - ✅ 前向传播全部shape对齐
   - ✅ 反向梯度流通正常（所有参数有grad）
   - ✅ AdamW优化器更新正常
   - ✅ 四阶段训练各1 epoch完整跑通
   - ✅ Sinkhorn OT迭代收敛
   - ✅ AUCpp指标计算正常

### 📊 快速测试结果（CPU，64训练样本，1 epoch/stage）

| 阶段 | l_rec_v | l_rec_c | l_ctr | l_corr | AUCpp |
|------|---------|---------|-------|--------|-------|
| A | 1.0089 | 0.9904 | - | - | - |
| B1 | 1.0016 | 0.9878 | 1.3864 | - | - |
| B2 | 1.0004 | 0.9829 | 1.3864 | - | - |
| C | 0.9997 | 0.9865 | 1.3863 | 0.5523 | 0.5137 |

> 注：以上为随机初始化1 epoch结果，l_ctr≈ln(2)=1.386符合未训练对比损失的预期；AUCpp≈0.51接近随机水平，说明需要更多训练epoch。模型参数量 **7.61M**。

---

## 6. 代码结构

```
multi-modal_comm/
├── config.py          # 所有超参数 (dataclass)
├── beamspace.py       # 波束空间变换 + NMS聚类
├── data.py            # 合成数据集 + DataLoader
├── models.py          # CMMAEModel 及其组件
├── masking.py         # 三种掩码策略
├── losses.py          # 损失函数 + AUCpp指标
├── train.py           # 主训练脚本
├── quick_test.py      # 快速验证脚本
└── README_REPORT.md   # 本文件
```

---

## 7. 下一步计划

### 短期（1-2周）
- [ ] 接入真实射线追踪数据集（替换当前合成数据）
- [ ] 在GPU上跑完整训练（各阶段10-20 epochs），观察AUCpp随训练提升
- [ ] 消融实验：验证每个阶段/模块的贡献（w/o beamspace, w/o contrastive, w/o OT, etc.）
- [ ] 加入物理正则项（波束空间TV平滑 + 稀疏约束）到重建损失
- [ ] 实现下游任务验证：波束预测 / 定位（用预训练特征）

### 中期（1个月）
- [ ] 收集/构建真实场景数据集（DeepSense / RADIATE / 自采集）
- [ ] 对比baseline：MAE单模态预训练、CLIP-style对比学习、无beamspace直接输入CFR
- [ ] 无监督变体(U)实验：不依赖射线追踪标签的几何引导掩码
- [ ] 不同遮挡/稀疏度下的鲁棒性分析

### 长期
- [ ] ISAC演示系统：实时相机→信道估计/波束预测
- [ ] 论文撰写

---

## 8. 运行方式

```bash
# 验证pipeline正确
cd /root/colum_comm/multi-modal_comm
python train.py --smoke_test --device cpu --batch_size 4

# 四阶段快速验证
python quick_test.py

# GPU完整训练
python train.py --variant W --batch_size 16 --device cuda --num_train 400
```

---



