# ICML 2026 Oral / Spotlight：剩余论文速览（第 181–490 篇）

> 共 **310** 篇：**89 Oral + 221 Spotlight**。
> 排序延续前序对话，从 **LASER: Learning Active Sensing for Continuum Field Reconstruction** 之后开始。
> 每篇提供 5 条摘要级 takeaway，基于 ICML 2026 官方虚拟会场与 OpenReview 元数据；问题、方法、机制与结果尽量保留英文技术表述，第 5 点给出中文研究启示。适合快速筛选，不替代阅读全文。

## 目录
- 第 181–210 篇：Latent / Learning / Long-context
- 第 211–240 篇：Lookahead / Optimization / Memory / Multimodal
- 第 241–270 篇：Multimodal / Neural / Offline RL / Theory
- 第 271–300 篇：Optimization / Causality / Position papers
- 第 301–330 篇：Position papers / Post-training / Privacy / RL
- 第 331–360 篇：Reasoning / Robustness / Safety / Scaling
- 第 361–390 篇：Scientific ML / Sequence modeling / Speech / Spatiotemporal
- 第 391–420 篇：Stability / Interpretability / Theory / Tool agents
- 第 421–450 篇：Reasoning / Tokenization / Training / Security
- 第 451–490 篇：Diffusion / Vision / World models / VLA

## 181. [Spotlight] LaST_0: Latent Spatio-Temporal Chain-of-Thought for Robotic Vision-Language-Action Model

1. 问题：However, explicit reasoning typically incurs non-negligible inference latency, which constrains the temporal resolution required for robotic manipulation.
2. 方法：提出/研究 **LaST_0**；To mitigate these limitations, we propose LaST_0, a framework that enables efficient reasoning before acting through a Latent Spatio-Temporal Chain-of-Thought…
3. 机制：Furthermore, LaST_0 adopts a dual-system architecture implemented via a Mixture-of-Transformers design, where a reasoning expert conducts low-frequency latent inference and an acting…
4. 结果：Across 10 real-world tasks spanning tabletop, mobile, and dexterous hand manipulation, LaST_0 improves mean success rates by 13%, 14% and 14% over…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[LaST_0: Latent Spatio-Temporal Chain-of-Thought for Robotic Vision-Language-Action Model](https://openreview.net/forum?id=lwOoBzJykL)

## 182. [Spotlight] Latent Collaboration in Multi-Agent Systems

1. 问题：Multi-agent systems (MAS) extend large language models (LLMs) from independent single-model reasoning to coordinative system-level intelligence.
2. 方法：提出/研究 **LatentMAS**；We introduce LatentMAS, an end-to-end training-free framework that enables pure latent collaboration among LLM agents.
3. 机制：In LatentMAS, each agent first performs auto-regressive latent thoughts generation through last-layer hidden embeddings instead of text.
4. 结果：In addition, empirical evaluations across 9 comprehensive benchmarks spanning math and science reasoning, commonsense understanding, and code generation show that LatentMAS outperforms…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Latent Collaboration in Multi-Agent Systems](https://openreview.net/forum?id=syG9I9ofd8)

## 183. [Spotlight] Latent Laplace Diffusion for Irregular Multivariate Time Series

1. 问题：Irregular multivariate time series impose a trade-off for long-horizon forecasting: discrete methods can distort temporal structure via re-gridding, while continuous-time models often…
2. 方法：提出/研究 **Latent Laplace Diffusion (LLapDiff)**；To bridge this gap, we present Latent Laplace Diffusion (LLapDiff), a generative framework that models the target as a low-dimensional…
3. 机制：Irregular multivariate time series impose a trade-off for long-horizon forecasting: discrete methods can distort temporal structure via re-gridding, while continuous-time models often…
4. 结果：Extensive experiments show that LLapDiff improves over baselines in long-horizon forecasting, and its continuous-time generative nature supports missing-value imputation by querying the…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Latent Laplace Diffusion for Irregular Multivariate Time Series](https://openreview.net/forum?id=t73XUJvyQr)

## 184. [Spotlight] Latent Spherical Flow Policy for Reinforcement Learning with Combinatorial Actions

1. 问题：Reinforcement learning (RL) with combinatorial action spaces remains challenging because feasible action sets are exponentially large and governed by complex feasibility constraints…
2. 方法：提出/研究 **solver-induced latent spherical flow policy that brings the expressive**；We propose a solver-induced latent spherical flow policy that brings the expressiveness of modern generative policies to combinatorial RL while…
3. 机制：Our method, LSFlow, learns a stochastic policy in a compact continuous latent space via spherical flow matching, and delegates feasibility to a…
4. 结果：Empirically, our approach outperforms state-of-the-art baselines by an average of 20.6\% across a range of challenging combinatorial RL tasks.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Latent Spherical Flow Policy for Reinforcement Learning with Combinatorial Actions](https://openreview.net/forum?id=07wwDFdi3k)

## 185. [Spotlight] Learning Biophysical Models of Large-Scale Multineuronal Data To Enable Precise Neurostimulation

1. 问题：However, fitting HH biophysical parameters typically requires intracellular recordings, which are invasive and low-throughput, limiting the ability to capture the geometry and…
2. 方法：提出/研究 **framework to rapidly infer HH parameters from designed features of…**；Here, we introduce a framework to rapidly infer HH parameters from designed features of extracellular MEA measurements by leveraging differentiable…
3. 机制：Here, we introduce a framework to rapidly infer HH parameters from designed features of extracellular MEA measurements by leveraging differentiable biophysical simulation…
4. 结果：Our framework predicted previously unseen multi-electrode stimulation responses with 90.4\% accuracy using HH models fit from only a few minutes of recording…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Learning Biophysical Models of Large-Scale Multineuronal Data To Enable Precise Neurostimulation](https://openreview.net/forum?id=4hoiRJsmpp)

## 186. [Spotlight] Learning Coupled Continuous-Time Latent Dynamics from Irregular Events

1. 问题：Modeling dynamic dependencies from irregularly sampled event sequences is a fundamental challenge in modern machine learning.
2. 方法：提出/研究 **Coupled Continuous-Time Latent Dynamics (CoCLD) framework that jointly**；We propose a Coupled Continuous-Time Latent Dynamics (CoCLD) framework that jointly models individual latent dynamics and population-level distributional shifts, and…
3. 机制：CoCLD integrates a Diffusion-based Latent Interpolator with neural ordinary differential equations, enabling principled interpolation, generation, and alignment of latent states across arbitrary…
4. 理论/证据：We show that the proposed coupling mechanism yields a consistent estimator of continuous-time latent dynamics under sparse and irregular observations.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Learning Coupled Continuous-Time Latent Dynamics from Irregular Events](https://openreview.net/forum?id=HfQ0X1lTGg)

## 187. [Spotlight] Learning Credal Ensembles via Distributionally Robust Optimization

1. 问题：However, most state-of-the-art (SOTA) methods primarily define EU as disagreement induced by random training initializations, which mainly reflects sensitivity to optimization randomness…
2. 方法：提出/研究 **EU as disagreement between models trained under different degrees of…**；In response, we formulate EU as disagreement between models trained under different degrees of relaxation of the i.i.d. assumption between…
3. 机制：Building on this idea, we propose *CreDRO*, which learns an ensemble of plausible models via distributionally robust optimization.
4. 结果：Empirically, CreDRO consistently outperforms SOTA credal approaches on downstream tasks, including out-of-distribution detection on extensive benchmarks and selective classification in…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Learning Credal Ensembles via Distributionally Robust Optimization](https://openreview.net/forum?id=cRTbp2pv7X)

## 188. [Spotlight] Learning Hamiltonian Flow Maps: Mean Flow Consistency for Large-Timestep Molecular Dynamics

1. 问题：Simulating the long-time evolution of Hamiltonian systems is limited by the small timesteps required for stable numerical integration.
2. 方法：提出/研究 **framework to learn *Hamiltonian Flow Maps* by predicting the *mean*…**；To overcome this constraint, we introduce a framework to learn *Hamiltonian Flow Maps* by predicting the *mean* phase-space evolution over…
3. 机制：To overcome this constraint, we introduce a framework to learn *Hamiltonian Flow Maps* by predicting the *mean* phase-space evolution over a chosen…
4. 结果：Validated across diverse Hamiltonian systems, our method in particular improves upon molecular dynamics simulations using machine-learned force fields (MLFF).
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Learning Hamiltonian Flow Maps: Mean Flow Consistency for Large-Timestep Molecular Dynamics](https://openreview.net/forum?id=EBSn23DLwB)

## 189. [Oral] Learning Human-Robot Collaboration via Heterogeneous-Agent Lyapunov Policy Optimization

1. 问题：However, inherent heterogeneity between robots and humans creates a rationality gap (RG), where decentralized policy updates deviate from cooperative joint optimization.
2. 方法：提出/研究 **heterogeneous-agent Lyapunov policy optimization (HALO)**；We propose heterogeneous-agent Lyapunov policy optimization (HALO), a framework that stabilizes decentralized MARL by enforcing Lyapunov-based contraction in policy-parameter space.
3. 机制：HALO rectifies decentralized gradients via optimal quadratic projections, ensuring monotonic contraction of RG and enabling effective exploration of open-ended interaction spaces.
4. 结果：Extensive simulations and real-world humanoid-robot experiments show that this certified stability improves generalization and robustness in collaborative corner cases.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Learning Human-Robot Collaboration via Heterogeneous-Agent Lyapunov Policy Optimization](https://openreview.net/forum?id=uBvlUE2wrP)

## 190. [Spotlight] Learning in Structured Stackelberg Games

1. 问题：In the online setting, we first prove that standard learning-theoretic measures of complexity do not characterize the difficulty of the leader's learning…
2. 方法：提出/研究 **Learning in Structured Stackelberg Games**；In the distributional setting, we provide analogous results by showing that two new dimensions control the sample complexity upper- and…
3. 机制：In the distributional setting, we provide analogous results by showing that two new dimensions control the sample complexity upper- and lower-bound.
4. 理论/证据：Motivated by applications such as security games and AI safety, we show how this additional structure can help the leader…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Learning in Structured Stackelberg Games](https://openreview.net/forum?id=XrKzHGg2jB)

## 191. [Spotlight] Learning Randomized Reductions

1. 问题：Randomized self-reductions (RSRs) express f(x) using f evaluated at random correlated points, enabling self-correcting programs, instance-hiding protocols, and applications in complexity theory…
2. 方法：提出/研究 **Bitween for automated RSR learning**；We present Bitween for automated RSR learning.
3. 机制：Second, we develop Vanilla Bitween, which integrates multiple backends (linear regression, genetic programming, symbolic regression, and mixed-integer programming).
4. 结果：Agentic Bitween discovers RSRs for 64 of 80 functions (80%), outperforming pure neural baselines in both RSR discovery and verification accuracy.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Learning Randomized Reductions](https://openreview.net/forum?id=hCAEcqig2C)

## 192. [Spotlight] Learning Structured Reasoning via Tractable Trajectory Control

1. 问题：However, complex reasoning trajectories remain sparse in unconstrained sampling, and standard RL often fails to guarantee the acquisition of diverse reasoning behaviors.
2. 方法：提出/研究 **systematic discovery and reinforcement of diverse reasoning patterns t**；We propose a systematic discovery and reinforcement of diverse reasoning patterns through structured reasoning, a paradigm that requires targeted exploration…
3. 机制：To this end, we propose Ctrl-R, a framework for learning structured reasoning via tractable trajectory control that actively guides the rollout process…
4. 结果：Experiments demonstrate that Ctrl-R enables effective exploration and internalization of previously unattainable reasoning patterns, yielding consistent improvements across language and vision–language models…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Learning Structured Reasoning via Tractable Trajectory Control](https://openreview.net/forum?id=x6J7va4BYz)

## 193. [Spotlight] Learning to Discover at Test Time

1. 问题：How can we use AI to discover a new state of the art for a scientific problem?
2. 方法：提出/研究 **method Test-Time Training to Discover (TTT-Discove**；Prior work in test-time scaling, such as AlphaEvolve, performs search by prompting a frozen LLM.
3. 机制：Prior work in test-time scaling, such as AlphaEvolve, performs search by prompting a frozen LLM.
4. 结果：All our results are achieved with an open model, OpenAI gpt-oss-120b, and can be reproduced with our publicly available code, in contrast…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Learning to Discover at Test Time](https://openreview.net/forum?id=96zNuQrH9Y)

## 194. [Spotlight] Learning to Execute Graph Algorithms Exactly with Graph Neural Networks

1. 问题：Understanding what graph neural networks can learn, especially their ability to learn to execute algorithms, remains a central theoretical challenge.
2. 方法：提出/研究 **Learning to Execute Graph Algorithms Exactly with Graph…**；To illustrate the learning power of our setting, we establish a rigorous learnability result for the LOCAL model of distributed…
3. 机制：To illustrate the learning power of our setting, we establish a rigorous learnability result for the LOCAL model of distributed computation.
4. 结果：We further demonstrate positive learnability results for widely studied algorithms such as message flooding, breadth-first and depth-first search, and Bellman-Ford.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Learning to Execute Graph Algorithms Exactly with Graph Neural Networks](https://openreview.net/forum?id=YKEmoqwkE9)

## 195. [Oral] Learning to Theorize the World from Observation

1. 问题：However, in machine learning, it remains unclear how to endow AI systems with such theory-building capability from raw, non-textual observation alone.
2. 方法：提出/研究 **Learning-to-Theorize (L2T)**；In this paper, we introduce Learning-to-Theorize (L2T), a learning paradigm in which an AI system acquires the ability to construct…
3. 机制：In this paper, we introduce Learning-to-Theorize (L2T), a learning paradigm in which an AI system acquires the ability to construct theories represented…
4. 结果：In experiments, we show that this formulation enables explanation-driven generalization, allowing observations to be understood in terms of the programs…
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[Learning to Theorize the World from Observation](https://openreview.net/forum?id=wsA8LgHU5U)

## 196. [Oral] Learning Unmasking Policies for Diffusion Language Models

1. 问题：However, such heuristics have downsides: they require manual tuning, and we observe that their performance degrades with larger block sizes.
2. 方法：提出/研究 **Learning Unmasking Policies for Diffusion Language Models**；One critical design aspect of dLLMs is the sampling procedure that selects which tokens to unmask at each diffusion step.
3. 机制：One critical design aspect of dLLMs is the sampling procedure that selects which tokens to unmask at each diffusion step.
4. 结果：Our experiments show that these trained policies match the performance of state-of-the-art heuristics when combined with semi-autoregressive (block) generation, while outperforming them…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Learning Unmasking Policies for Diffusion Language Models](https://openreview.net/forum?id=F9NDKf5oPy)

## 197. [Spotlight] Learning with Admissibility: Robust Fuzzy Hashing for Cross-Modal Retrieval with Noisy Labels

1. 问题：Recently, cross-modal hashing (CMH) has garnered significant attention due to its low storage costs and high retrieval efficiency.
2. 方法：提出/研究 **novel Robust Fuzzy Cross-modal Hashing framework (RFCMH) that introduc**；To address these limitations, we propose a novel Robust Fuzzy Cross-modal Hashing framework (RFCMH) that introduces fuzzy set theory to…
3. 机制：To address these limitations, we propose a novel Robust Fuzzy Cross-modal Hashing framework (RFCMH) that introduces fuzzy set theory to endow the…
4. 结果：Extensive experiments on multiple benchmarks demonstrate that RFCMH achieves state-of-the-art retrieval performance.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Learning with Admissibility: Robust Fuzzy Hashing for Cross-Modal Retrieval with Noisy Labels](https://openreview.net/forum?id=reYe33OKVp)

## 198. [Spotlight] Learning-to-Optimize via Deep Unfolded Flows

1. 问题：Subsequently, we unfold this velocity field as the internal iteration of an optimization sequence, and fine-tune it in an end-to-end manner by…
2. 方法：提出/研究 ***FlowOptimizer***；We introduce *FlowOptimizer*, a deep unfolded, flow-based framework for learned iterative optimization.
3. 机制：Motivated by the expressiveness of flow models, we represent each optimization iteration via a velocity field that operates on a population of…
4. 结果：FlowOptimizer consistently outperforms well-established sampling-based/gradient-based traditional optimization and learning-to-optimize methods, often by orders of magnitude in terms of solution quality.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Learning-to-Optimize via Deep Unfolded Flows](https://openreview.net/forum?id=ZOtOq7hxJP)

## 199. [Spotlight] Less is Enough: Synthesizing Diverse Data in LLM Feature Space with Sparse Autoencoders

1. 问题：The diversity of post-training data is critical for effective downstream performance in large language models (LLMs).
2. 方法：提出/研究 *****Feature Activation Coverage* (FAC)** which measures data diversity**；In this work, we introduce ***Feature Activation Coverage* (FAC)** which measures data diversity in an interpretable feature space.
3. 机制：In this work, we introduce ***Feature Activation Coverage* (FAC)** which measures data diversity in an interpretable feature space.
4. 结果：Experiments show that our approach consistently improves both data diversity and downstream performance on various tasks, including instruction following, toxicity detection, reward…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Less is Enough: Synthesizing Diverse Data in LLM Feature Space with Sparse Autoencoders](https://openreview.net/forum?id=GVupwQ0578)

## 200. [Spotlight] LiftQuant: Continuous Bit-Width LLM via Dimensional Lifting and Projection

1. 问题：Existing quantization methods are fundamentally limited by rigid, integer-based bit-widths (e.g., 2, 3-bit), resulting in a "deployment gap" where Large Language Models…
2. 方法：提出/研究 **LiftQuant**；To bridge this gap, we introduce LiftQuant, a novel framework that enables continuous bit-width control for true Pareto-optimal deployment.
3. 机制：To bridge this gap, we introduce LiftQuant, a novel framework that enables continuous bit-width control for true Pareto-optimal deployment.
4. 结果：This flexibility is transformative: LiftQuant enables a 70B LLM to be compressed to 2.4 bits to precisely fit a 24GB GPU, where…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[LiftQuant: Continuous Bit-Width LLM via Dimensional Lifting and Projection](https://openreview.net/forum?id=1GvXUhLIMP)

## 201. [Spotlight] LiME: Lightweight Mixture of Experts for Efficient Multimodal Multi-task Learning

1. 问题：MoE-PEFT methods combine Mixture of Experts with parameter-efficient fine-tuning for multi-task adaptation, but require separate adapters per expert—causing trainable parameters to scale…
2. 方法：提出/研究 **LiME**；We propose LiME (Lightweight Mixture of Experts), which achieves expert specialization through lightweight modulation rather than adapter replication.
3. 机制：We propose LiME (Lightweight Mixture of Experts), which achieves expert specialization through lightweight modulation rather than adapter replication.
4. 结果：Experiments on MMT-47, a multimodal multi-task benchmark with 47 tasks spanning text, image, and video, demonstrate that LiME achieves competitive or superior…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[LiME: Lightweight Mixture of Experts for Efficient Multimodal Multi-task Learning](https://openreview.net/forum?id=KRSZj8z5Lr)

## 202. [Spotlight] LIMSSR: LLM-Driven Sequence-to-Score Reasoning under Training-Time Incomplete Multimodal Observations

1. 问题：We propose LIMSSR (LLM-Driven Incomplete Multimodal Sequence-to-Score Reasoning), a framework that reformulates this challenge as a conditional sequence reasoning task.
2. 方法：提出/研究 **LIMSSR**；We propose LIMSSR (LLM-Driven Incomplete Multimodal Sequence-to-Score Reasoning), a framework that reformulates this challenge as a conditional sequence reasoning task.
3. 机制：LIMSSR leverages the semantic reasoning capabilities of Large Language Models via Prompt-Guided Context-Aware Modality Imputation and Multidimensional Representation Fusion to infer latent…
4. 结果：Extensive experiments on three Action Quality Assessment datasets demonstrate that LIMSSR significantly outperforms state-of-the-art baselines without relying on complete training data, establishing…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[LIMSSR: LLM-Driven Sequence-to-Score Reasoning under Training-Time Incomplete Multimodal Observations](https://openreview.net/forum?id=0RLF7Sj2Fg)

## 203. [Spotlight] Linear Causal Representation Learning by Topological Ordering, Pruning, and Disentanglement

1. 问题：However, these prerequisites can be easy to violate in practice.
2. 方法：提出/研究 **novel linear CRL algorithm that**；In this work, we propose a novel linear CRL algorithm that, unlike existing methods, operates under weaker assumptions on environment…
3. 机制：We further validate our new algorithm via synthetic experiments and an interpretability analysis of large language models, demonstrating both its superiority over…
4. 结果：We further validate our new algorithm via synthetic experiments and an interpretability analysis of large language models, demonstrating both its superiority over…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Linear Causal Representation Learning by Topological Ordering, Pruning, and Disentanglement](https://openreview.net/forum?id=4COS6SMf8r)

## 204. [Spotlight] Linguistic Nepotism: Trading-off Quality for Language Preference in Multilingual RAG

1. 问题：Multilingual Retrieval-Augmented Generation (mRAG) systems enable language models to answer knowledge-intensive queries with citation-supported responses across languages.
2. 方法：提出/研究 **controlled methodology using model internals to measure language prefe**；To investigate this, we introduce a controlled methodology using model internals to measure language preference while holding other factors such…
3. 机制：To investigate this, we introduce a controlled methodology using model internals to measure language preference while holding other factors such as document…
4. 理论/证据：To investigate this, we introduce a controlled methodology using model internals to measure language preference while holding other factors such…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Linguistic Nepotism: Trading-off Quality for Language Preference in Multilingual RAG](https://openreview.net/forum?id=MDfCV0UHSb)

## 205. [Spotlight] Linguistic Properties and Model Scale in Brain Encoding: From Small to Compressed Language Models

1. 问题：Recent work has shown that scaling large language models (LLMs) improves their alignment with human brain activity, yet it remains unclear what…
2. 方法：提出/研究 **Linguistic Properties and Model Scale in Brain Encoding**；Although larger models often yield better task performance and brain alignment, they are increasingly difficult to analyze mechanistically.
3. 机制：Although larger models often yield better task performance and brain alignment, they are increasingly difficult to analyze mechanistically.
4. 结果：Across model families up to 14B parameters, we find that 3B SLMs achieve brain predictivity indistinguishable from larger LLMs, whereas 1B models…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Linguistic Properties and Model Scale in Brain Encoding: From Small to Compressed Language Models](https://openreview.net/forum?id=WK1NvxRMsL)

## 206. [Spotlight] Listening Through the Noise: Cauchy-Driven Diffusion Bridges for Robust Gastrointestinal Auscultation and Clinical Benchmarking

1. 问题：However, the diagnostic utility of BS is often compromised by its spectral overlap with non-stationary speech interference.
2. 方法：提出/研究 **novel Cauchy-driven Diffusion Bridge framework to isolate high-fidelit**；In this paper, we propose a novel Cauchy-driven Diffusion Bridge framework to isolate high-fidelity bowel sounds from complex interference.
3. 机制：Gastrointestinal (GI) motility assessment via bowel sounds (BS) offers a non-invasive alternative to resource-intensive clinical standards.
4. 结果：These results demonstrate the system's potential for robust clinical GI monitoring and diagnosis.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Listening Through the Noise: Cauchy-Driven Diffusion Bridges for Robust Gastrointestinal Auscultation and Clinical Benchmarking](https://openreview.net/forum?id=EYAfw6czcC)

## 207. [Spotlight] Local Covariate Selection for Average Causal Effect Estimation without Pretreatment and Causal Sufficiency Assumptions

1. 问题：However, most existing methods either rely on learning the global causal structure, assume the absence of latent variables, or impose the pretreatment…
2. 方法：提出/研究 **novel local learning method for covariate selection in nonparametric c**；Based on this characterization, we develop a novel local learning method for covariate selection in nonparametric causal effect estimation.
3. 机制：Its effectiveness is validated through extensive experiments on both synthetic and real-world datasets.
4. 结果：Its effectiveness is validated through extensive experiments on both synthetic and real-world datasets.
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[Local Covariate Selection for Average Causal Effect Estimation without Pretreatment and Causal Sufficiency Assumptions](https://openreview.net/forum?id=qZVcGlU5lN)

## 208. [Spotlight] Local Mechanisms of Compositional Generalization in Conditional Diffusion

1. 问题：Conditional diffusion models appear capable of compositional generalization, i.e., generating convincing samples for out-of-distribution combinations of conditioners, but the mechanisms underlying this…
2. 方法：提出/研究 **Local Mechanisms of Compositional Generalization in Conditional Diffusion**；To make this concrete, we study length generalization, the ability to generate images with more objects than seen during training.
3. 机制：To make this concrete, we study length generalization, the ability to generate images with more objects than seen during training.
4. 结果：In a controlled CLEVR setting (Johnson et al., 2017), we find that length generalization is achievable in some cases but not others…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Local Mechanisms of Compositional Generalization in Conditional Diffusion](https://openreview.net/forum?id=XsfjvLhKAP)

## 209. [Spotlight] Local Redundancy: An Information-Theoretic Measure of Plasticity from Synthetic Memorization

1. 问题：Existing measures, such as effective rank, dead neuron fraction, and weight norm, lack theoretical grounding and correlate poorly with performance on new…
2. 方法：提出/研究 ***local redundancy***；We introduce *local redundancy*, an information-theoretic measure derived from universal compression theory.
3. 机制：We introduce *local redundancy*, an information-theoretic measure derived from universal compression theory.
4. 结果：Experiments on continual image classification and time series transfer learning demonstrate that local redundancy predicts downstream performance better than existing measures and…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Local Redundancy: An Information-Theoretic Measure of Plasticity from Synthetic Memorization](https://openreview.net/forum?id=ucbH88BgIk)

## 210. [Spotlight] Long-Context Modeling with Dynamic Hierarchical Sparse Attention for Memory-Constrained LLM Inference

1. 问题：The quadratic cost of attention limits the scalability of long-context LLMs, especially under limited hardware memory budgets.
2. 方法：提出/研究 **Dynamic Hierarchical Sparse Attention (DHSA)**；We propose Dynamic Hierarchical Sparse Attention (DHSA), a data-driven framework that predicts attention sparsity online while keeping the LLM backbone…
3. 机制：We propose Dynamic Hierarchical Sparse Attention (DHSA), a data-driven framework that predicts attention sparsity online while keeping the LLM backbone frozen.
4. 结果：These results demonstrate DHSA as an efficient and adaptable solution for memory-constrained long-context LLM inference.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Long-Context Modeling with Dynamic Hierarchical Sparse Attention for Memory-Constrained LLM Inference](https://openreview.net/forum?id=o3gN27ITWV)

## 211. [Spotlight] Lookahead Sample Reward Guidance for Test-Time Scaling of Diffusion Models

1. 问题：Diffusion models have demonstrated strong generative performance; however, generated samples often fail to fully align with human intent.
2. 方法：提出/研究 **few-step lookahead sampling and an accurate solver that guides particl**；To further improve efficiency, we introduce a few-step lookahead sampling and an accurate solver that guides particles toward high-reward lookahead…
3. 机制：To further improve efficiency, we introduce a few-step lookahead sampling and an accurate solver that guides particles toward high-reward lookahead samples.
4. 结果：LiDAR achieves the same GenEval performance as the latest gradient guidance method for SDXL with a 9.5× speedup.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Lookahead Sample Reward Guidance for Test-Time Scaling of Diffusion Models](https://openreview.net/forum?id=IbRm6gwmew)

## 212. [Spotlight] Loss-Aware Distributionally Robust Optimization via Trainable Optimal Transport Ambiguity Sets

1. 问题：The standard OT-DRO pipeline consists of a two-step procedure, where the ambiguity set is first designed and subsequently embedded into the downstream…
2. 方法：提出/研究 **n end-to-end pipeline to automatically learn decision-focused ambiguit**；We introduce an end-to-end pipeline to automatically learn decision-focused ambiguity sets for OT-DRO problems, where the loss function informs the…
3. 机制：Optimal-transport distributionally robust optimization (OT-DRO) robustifies data-driven decision-making under uncertainty by capturing the sampling-induced statistical error via optimal transport ambiguity sets.
4. 结果：We present experiments validating our method on standard portfolio optimization and linear regression tasks.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Loss-Aware Distributionally Robust Optimization via Trainable Optimal Transport Ambiguity Sets](https://openreview.net/forum?id=K1EPPO9t2c)

## 213. [Oral] Lottery Prior: Randomized Neural Compression for Zero-Shot Inverse Problems

1. 问题：We study zero-shot inverse problems, where a clean signal is recovered from a single degraded observation without external training data.
2. 方法：提出/研究 **Lottery Prior**；We propose Lottery Prior, a compression-based inverse solver that leverages architectural priors from random networks and induces a family of…
3. 机制：We propose Lottery Prior, a compression-based inverse solver that leverages architectural priors from random networks and induces a family of implicit priors…
4. 结果：Experiments on denoising, noisy super-resolution, and inpainting demonstrate that our method achieves state-of-the-art with significantly fewer effective parameters.
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[Lottery Prior: Randomized Neural Compression for Zero-Shot Inverse Problems](https://openreview.net/forum?id=YNoQhMrps4)

## 214. [Spotlight] MACKO: Sparse matrix-vector multiplication for low sparsity

1. 问题：We propose **MACKO-SpMV**, a GPU-optimized format and kernel co-designed to reduce storage overhead while remaining compatible with the GPU’s execution model.
2. 方法：提出/研究 ****MACKO-SpMV****；We propose **MACKO-SpMV**, a GPU-optimized format and kernel co-designed to reduce storage overhead while remaining compatible with the GPU’s execution…
3. 机制：We propose **MACKO-SpMV**, a GPU-optimized format and kernel co-designed to reduce storage overhead while remaining compatible with the GPU’s execution model.
4. 结果：As a result, **unstructured pruning at 50\\% sparsity becomes practical** for real-world LLM workloads and **bridges the efficiency gap with structured 2:4…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[MACKO: Sparse matrix-vector multiplication for low sparsity](https://openreview.net/forum?id=ah9xkFXCV6)

## 215. [Spotlight] Manifold-Aware Perturbations for Constrained Generative Modeling

1. 问题：However, they encounter inherent mathematical limitations in modeling distributions where samples are constrained by equalities, as is frequently the setting in scientific…
2. 方法：提出/研究 **computationally cheap**；In this work, we develop a computationally cheap, mathematically justified, and highly flexible distributional modification for combating known pitfalls in…
3. 机制：Through theoretical analyses and empirical evidence on several representative tasks, we illustrate that our approach consistently enables data distribution recovery and stable…
4. 结果：Through theoretical analyses and empirical evidence on several representative tasks, we illustrate that our approach consistently enables data distribution recovery…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Manifold-Aware Perturbations for Constrained Generative Modeling](https://openreview.net/forum?id=UPiyC9W4ms)

## 216. [Spotlight] Manifold-Optimal Guidance: A Unified Riemannian Control View of Diffusion Guidance

1. 问题：We attribute this failure to a geometric mismatch: standard CFG performs Euclidean extrapolation in ambient space, inadvertently driving sampling trajectories off the…
2. 方法：提出/研究 **Manifold-Optimal Guidance (MOG)**；To resolve this, we present Manifold-Optimal Guidance (MOG), a framework that reformulates guidance as a local optimal control problem.
3. 机制：To resolve this, we present Manifold-Optimal Guidance (MOG), a framework that reformulates guidance as a local optimal control problem.
4. 结果：Extensive validation demonstrates that MOG yields superior fidelity and alignment compared to baselines, with virtually no added computational overhead.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Manifold-Optimal Guidance: A Unified Riemannian Control View of Diffusion Guidance](https://openreview.net/forum?id=eSxGdQ0zwG)

## 217. [Spotlight] Many Experiments, Few Repetitions, Unpaired Data, and Sparse Effects: Is Causal Inference Possible?

1. 问题：We study the problem of estimating causal effects under hidden confounding in the following unpaired data setting: we observe some covariates X…
2. 方法：提出/研究 **GMM-type estimator based on cross-fold sample splitting of the instrum**；We propose a GMM-type estimator based on cross-fold sample splitting of the instrument–covariate sample that also applies in standard IV…
3. 机制：We further extend the method to sparse causal effects via _1-regularized estimation and post-selection refitting.
4. 结果：We study the problem of estimating causal effects under hidden confounding in the following unpaired data setting: we observe some covariates X…
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[Many Experiments, Few Repetitions, Unpaired Data, and Sparse Effects: Is Causal Inference Possible?](https://openreview.net/forum?id=gqa99Ev4C4)

## 218. [Oral] Markov Chain Monte Carlo without Evaluating the Target: an Auxiliary Variable Approach

1. 问题：However, in many situations, even evaluating the unnormalized distribution can be costly or infeasible.
2. 方法：提出/研究 **Markov Chain Monte Carlo without Evaluating the Target**；However, in many situations, even evaluating the unnormalized distribution can be costly or infeasible.
3. 机制：However, in many situations, even evaluating the unnormalized distribution can be costly or infeasible.
4. 结果：The code to reproduce the experimental results can be found at 
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Markov Chain Monte Carlo without Evaluating the Target: an Auxiliary Variable Approach](https://openreview.net/forum?id=dDkl5ZcyTl)

## 219. [Spotlight] MASPOB: Bandit-Based Prompt Optimization for Multi-Agent Systems with Graph Neural Networks

1. 问题：However, real-world prompt optimization for MAS is impeded by three key challenges: (1) the need of sample efficiency due to prohibitive evaluation…
2. 方法：提出/研究 ****MASPOB** (**M**ulti-**A**gent **S**ystem **P**rompt **O**ptimization**；To address these challenges, we introduce **MASPOB** (**M**ulti-**A**gent **S**ystem **P**rompt **O**ptimization via **B**andits), a novel sample-efficient framework based on bandits.
3. 机制：To handle topology-induced coupling, MASPOB integrates Graph Neural Networks (GNNs) to capture structural priors, learning topology-aware representations of prompt semantics.
4. 结果：Extensive experiments across diverse benchmarks demonstrate that MASPOB achieves state-of-the-art performance, consistently outperforming existing baselines.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[MASPOB: Bandit-Based Prompt Optimization for Multi-Agent Systems with Graph Neural Networks](https://openreview.net/forum?id=A5venxSvpw)

## 220. [Spotlight] Matroid Algorithms Under Size-Sensitive Independence Oracles

1. 问题：We address this gap by introducing a size-sensitive cost model where the cost of a query Q scales with |Q|.
2. 方法：提出/研究 **Matroid Algorithms Under Size-Sensitive Independence Oracles**；We establish tight results, proving nearly matching upper and lower bounds that show the optimal query cost is (up to…
3. 机制：We establish tight results, proving nearly matching upper and lower bounds that show the optimal query cost is (up to logarithmic factors)…
4. 理论/证据：While this abstraction has underpinned much of the theoretical progress in matroid optimization, it masks the true computational effort required…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Matroid Algorithms Under Size-Sensitive Independence Oracles](https://openreview.net/forum?id=80Job2F5eb)

## 221. [Oral] Maximum Likelihood Reinforcement Learning

1. 问题：Reinforcement learning (RL) is the method of choice for training models in setups where the objective function can only be evaluated by…
2. 方法：提出/研究 ****Maximum Likelihood Reinforcement Learning (MaxRL)****；To remedy this mismatch, we introduce **Maximum Likelihood Reinforcement Learning (MaxRL)**, a compute-indexed family of sample-based objectives that interpolate between…
3. 机制：To remedy this mismatch, we introduce **Maximum Likelihood Reinforcement Learning (MaxRL)**, a compute-indexed family of sample-based objectives that interpolate between expected-reward RL…
4. 结果：MaxRL Pareto-dominates existing methods in all tested models and tasks, achieves up to 20 gains in test-time scaling efficiency over GRPO, and…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Maximum Likelihood Reinforcement Learning](https://openreview.net/forum?id=EeuLO2BjFN)

## 222. [Spotlight] Measuring Agents in Production

1. 问题：LLM-based agents already operate in production across many industries, yet we lack an understanding of what technical methods make deployments successful.
2. 方法：提出/研究 **first systematic study of **M**easuring **A**gents in **P**roduction**；We present the first systematic study of **M**easuring **A**gents in **P**roduction, MAP, using first-hand data from agent developers.
3. 机制：We conducted 20 case studies via in-depth interviews and surveyed 86 deployed systems practitioners across 26 domains.
4. 结果：Our study finds that production agents are built using simple, controllable approaches: 68% execute at most 10 steps before human intervention, 70%…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Measuring Agents in Production](https://openreview.net/forum?id=mWxEAgz3xu)

## 223. [Oral] Mechanistic Data Attribution: Tracing the Training Origins of Interpretable LLM Units

1. 问题：While mechanistic interpretability has identified interpretable circuits in large language models (LLMs), their causal origins in training data remain elusive.
2. 方法：提出/研究 ***mechanistic data attribution* (MDA)**；We introduce *mechanistic data attribution* (MDA), a scalable framework that employs influence functions to trace interpretable units back to specific…
3. 机制：Through extensive experiments on the Pythia family, we causally validate that targeted intervention—removing or augmenting a small fraction of high-influence samples—significantly modulates…
4. 结果：Through extensive experiments on the Pythia family, we causally validate that targeted intervention—removing or augmenting a small fraction of high-influence samples—significantly modulates…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Mechanistic Data Attribution: Tracing the Training Origins of Interpretable LLM Units](https://openreview.net/forum?id=PQaxfoEcRc)

## 224. [Spotlight] MemoryBench: A Benchmark for Memory and Continual Learning in LLM Systems

1. 问题：Scaling up data, parameters, and test-time computation has been the mainstream methods to improve LLM systems (LLMsys), but their upper bounds are…
2. 方法：提出/研究 **user feedback simulation framework and a comprehensive benchmark cover**；Therefore, we propose a user feedback simulation framework and a comprehensive benchmark covering multiple domains, languages, and types of tasks…
3. 机制：Therefore, we propose a user feedback simulation framework and a comprehensive benchmark covering multiple domains, languages, and types of tasks to evaluate…
4. 结果：Experiments show that the effectiveness and efficiency of state-of-the-art baselines are far from satisfying, and we hope this benchmark could pave the…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[MemoryBench: A Benchmark for Memory and Continual Learning in LLM Systems](https://openreview.net/forum?id=If4X4W2HWx)

## 225. [Spotlight] MEnvAgent: Scalable Polyglot Environment Construction for Verifiable Software Engineering

1. 问题：The evolution of Large Language Model (LLM) agents for software engineering (SWE) is constrained by the scarcity of verifiable datasets, a bottleneck…
2. 方法：提出/研究 ****MEnvAgent****；To address this, we introduce **MEnvAgent**, a **M**ulti-language framework for automated **Env**ironment construction that facilitates scalable generation of verifiable task…
3. 机制：MEnvAgent employs a multi-agent Planning-Execution-Verification architecture to autonomously resolve construction failures and integrates a novel Environment Reuse Mechanism that reduces computational overhead…
4. 结果：Additionally, we demonstrate the utility of MEnvAgent by constructing MEnvData-SWE, the largest open-source polyglot dataset of realistic verifiable Docker environments to date…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[MEnvAgent: Scalable Polyglot Environment Construction for Verifiable Software Engineering](https://openreview.net/forum?id=Mkal0hTCnh)

## 226. [Spotlight] MetaphorVU: Towards Metaphorical Video Understanding

1. 问题：The lack of systematic studies on metaphorical video understanding not only constrains the real-world applicability of MLLMs but also impedes the thorough…
2. 方法：提出/研究 **MetaphorVU-Bench**；To bridge this gap, we propose MetaphorVU-Bench, the first systematic and comprehensive benchmark dedicated to metaphorical video understanding.
3. 机制：Through experiments, we find current MLLMs struggle with accurate metaphorical video understanding, lagging far behind human level, primarily due to defective cross-domain…
4. 结果：Our benchmark, analysis, and method provide useful insights and a foundation for future research on advancing MLLMs.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[MetaphorVU: Towards Metaphorical Video Understanding](https://openreview.net/forum?id=yKcBAJMPXZ)

## 227. [Spotlight] mHC: Manifold-Constrained Hyper-Connections

1. 问题：To address these challenges, we propose Manifold-Constrained Hyper-Connections (mHC), a general framework that projects the residual connection space of HC onto a…
2. 方法：提出/研究 **Manifold-Constrained Hyper-Connections (mHC)**；To address these challenges, we propose Manifold-Constrained Hyper-Connections (mHC), a general framework that projects the residual connection space of HC…
3. 机制：To address these challenges, we propose Manifold-Constrained Hyper-Connections (mHC), a general framework that projects the residual connection space of HC onto a…
4. 结果：Empirical experiments demonstrate that mHC is effective for training at scale, offering tangible performance improvements and superior scalability.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[mHC: Manifold-Constrained Hyper-Connections](https://openreview.net/forum?id=mDhyxu8WRb)

## 228. [Oral] Midtraining Bridges Pretraining and Posttraining Distributions

1. 问题：Midtraining, the practice of mixing specialized data with more general pretraining data in an intermediate training phase, has become widespread in language…
2. 方法：提出/研究 **that midtraining functions as distributional bridging by providing bet**；We propose that midtraining functions as distributional bridging by providing better initialization for posttraining.
3. 机制：We propose that midtraining functions as distributional bridging by providing better initialization for posttraining.
4. 结果：In these domains, midtraining consistently outperforms continued pretraining on specialized data alone both in-domain and in terms of mitigating forgetting.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Midtraining Bridges Pretraining and Posttraining Distributions](https://openreview.net/forum?id=5PfEQzE9bf)

## 229. [Oral] Mind Your Margin and Boundary: Are Your Distilled Datasets Truly Robust?

1. 问题：Dataset distillation (DD) compresses a large training set into a small synthetic set for efficient training, but most DD methods optimize only…
2. 方法：提出/研究 **Contrastive Curriculum for Robust Dataset Distillation (C^2R)**；We present Contrastive Curriculum for Robust Dataset Distillation (C^2R), a framework that couples an attack-aware curriculum with a contrastive robustness…
3. 机制：We present Contrastive Curriculum for Robust Dataset Distillation (C^2R), a framework that couples an attack-aware curriculum with a contrastive robustness objective.
4. 结果：Experiments on CIFAR-10/100, Tiny-ImageNet, and multiple ImageNet-1K subsets under six attacks show that C^2R achieves the best robust accuracy, outperforming prior robust…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Mind Your Margin and Boundary: Are Your Distilled Datasets Truly Robust?](https://openreview.net/forum?id=Y3K0pPyVcs)

## 230. [Spotlight] Mind-Omni: A Unified Multi-Task Framework for Brain-Vision-Language Modeling via Discrete Diffusion

1. 问题：A major limitation of prior work is the prevailing paradigm of specialized, single-task models, which curtails versatility and neglects inter-task synergies.
2. 方法：提出/研究 **Mind-Omni**；To address this, we propose Mind-Omni, the first versatile framework that unifies seven distinct encoding and decoding tasks through a…
3. 机制：At its core is a novel Brain Tokenizer that transforms heterogeneous, continuous brain signals into standardized, discrete tokens.
4. 结果：By demonstrating performance competitive with, and at times superior to, larger specialized models, our work offers a powerful new paradigm for neural…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Mind-Omni: A Unified Multi-Task Framework for Brain-Vision-Language Modeling via Discrete Diffusion](https://openreview.net/forum?id=3gCdh3u2GK)

## 231. [Spotlight] MiniAppBench: Evaluating the Shift from Text to Interactive HTML Responses in LLM-Powered Assistants

1. 问题：However, existing benchmarks primarily focus on algorithmic correctness or static layout reconstruction, failing to capture the capabilities required for this new paradigm.
2. 方法：提出/研究 ****MiniAppBench****；To address this gap, we introduce **MiniAppBench**, the first comprehensive benchmark designed to evaluate principle-driven, interactive application generation.
3. 机制：To address this gap, we introduce **MiniAppBench**, the first comprehensive benchmark designed to evaluate principle-driven, interactive application generation.
4. 结果：Our experiments reveal that current LLMs still face significant challenges in generating high-quality MiniApps, while MiniAppEval demonstrates high alignment with human judgment…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[MiniAppBench: Evaluating the Shift from Text to Interactive HTML Responses in LLM-Powered Assistants](https://openreview.net/forum?id=pwbLmew1aq)

## 232. [Oral] Minimax Optimal Strategy for Delayed Observations in Online Reinforcement Learning

1. 问题：We study reinforcement learning with delayed state observation, where the agent observes the current state after some random number of time steps.
2. 方法：提出/研究 **n algorithm that combines the augmentation method and the upper…**；We propose an algorithm that combines the augmentation method and the upper confidence bound approach.
3. 机制：We propose an algorithm that combines the augmentation method and the upper confidence bound approach.
4. 理论/证据：We propose an algorithm that combines the augmentation method and the upper confidence bound approach.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Minimax Optimal Strategy for Delayed Observations in Online Reinforcement Learning](https://openreview.net/forum?id=fFupHW7Jqx)

## 233. [Spotlight] MIRA: A Score for Conditional Distribution Accuracy and Model Comparison

1. 问题：We introduce MIRA, a sample-based score for assessing the accuracy of a candidate conditional distribution using only joint samples from the true…
2. 方法：提出/研究 **MIRA**；We introduce MIRA, a sample-based score for assessing the accuracy of a candidate conditional distribution using only joint samples from…
3. 机制：Consequently, MIRA enables Bayesian model comparison through direct posterior validation, bypassing the challenging evidence computation.
4. 结果：We demonstrate its effectiveness across several toy problems and Bayesian inference tasks.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[MIRA: A Score for Conditional Distribution Accuracy and Model Comparison](https://openreview.net/forum?id=ra2t1V4nml)

## 234. [Spotlight] Mitigating Hallucinations in Large Vision-Language Models via Causal Route Gating

1. 问题：We show that a key failure mode arises from route competition: even when visual tokens receive attention, the final token decision can…
2. 方法：提出/研究 **training-free**；To mitigate this, we propose a training-free, decision-aligned intervention that decomposes each attention head into a visual route and a…
3. 机制：To mitigate this, we propose a training-free, decision-aligned intervention that decomposes each attention head into a visual route and a text route…
4. 结果：Across five benchmarks spanning discriminative and generative settings, our method consistently reduces hallucination-related errors across models with limited impact on overall multimodal…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Mitigating Hallucinations in Large Vision-Language Models via Causal Route Gating](https://openreview.net/forum?id=LIcj73RLX6)

## 235. [Oral] Mitigating Reward Hacking in RLHF via Bayesian Non-negative Reward Modeling

1. 问题：Reward models learned from human preferences are central to aligning large language models (LLMs) via reinforcement learning from human feedback, yet they…
2. 方法：提出/研究 **Bayesian Non-Negative Reward Model (BNRM)**；We propose Bayesian Non-Negative Reward Model (BNRM), a principled reward modeling framework that integrates non-negative factor analysis into Bradley–Terry (BT)…
3. 机制：Reward models learned from human preferences are central to aligning large language models (LLMs) via reinforcement learning from human feedback, yet they…
4. 结果：Extensive empirical results demonstrate that BNRM substantially mitigates reward over-optimization, improves robustness under distribution shifts, and yields more interpretable reward decompositions than…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Mitigating Reward Hacking in RLHF via Bayesian Non-negative Reward Modeling](https://openreview.net/forum?id=DfhMMHXDuu)

## 236. [Spotlight] Mixture of Concept Bottleneck Experts

1. 问题：Concept Bottleneck Models (CBMs) promote interpretability by grounding predictions in human-understandable concepts.
2. 方法：提出/研究 **Mixture of Concept Bottleneck Experts (M-CBEs)**；We propose Mixture of Concept Bottleneck Experts (M-CBEs), a framework that generalizes existing CBMs along two dimensions: the number of…
3. 机制：We propose Mixture of Concept Bottleneck Experts (M-CBEs), a framework that generalizes existing CBMs along two dimensions: the number of expressions, referred…
4. 结果：Empirical evaluation demonstrates that varying the number of expressions and their functional form provides a robust framework for navigating the accuracy-interpretability trade-off.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Mixture of Concept Bottleneck Experts](https://openreview.net/forum?id=Jj8Vec8qSs)

## 237. [Oral] Mixtures Closest To A Given Measure: A Semidefinite Programming Approach

1. 问题：A key challenge, especially in high-dimensional settings, is to determine the mixture order and estimate the mixture parameters.
2. 方法：提出/研究 **hierarchy of semidefinite relaxations with asymptotic convergence to t**；We introduce a hierarchy of semidefinite relaxations with asymptotic convergence to the desired optimal value.
3. 机制：We study the problem of approximating a target measure, available only through finitely many of its moments, by a mixture of distributions…
4. 理论/证据：We introduce a hierarchy of semidefinite relaxations with asymptotic convergence to the desired optimal value.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Mixtures Closest To A Given Measure: A Semidefinite Programming Approach](https://openreview.net/forum?id=0JDzkrKzaA)

## 238. [Oral] Modeling Hierarchical Thinking in Large Reasoning Models

1. 问题：Large Reasoning Models (LRMs) solve complex tasks by generating long Chain-of-Thought (CoT) sequences; however, the emergent dynamics governing reasoning trajectories are not…
2. 方法：提出/研究 **to approximate LRM's emerging hierarchical reasoning dynamics as a tra**；In this work, we propose to approximate LRM's emerging hierarchical reasoning dynamics as a trajectory within a Finite State Machine…
3. 机制：In this work, we propose to approximate LRM's emerging hierarchical reasoning dynamics as a trajectory within a Finite State Machine (FSM) transitioning…
4. 结果：Experiments across four benchmarks (AIME25, MATH-500, GSM8k, and GPQA Diamond) using three state-of-the-art open reasoning models demonstrate that Q-Value steering policy achieves…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Modeling Hierarchical Thinking in Large Reasoning Models](https://openreview.net/forum?id=N44P3zrrgO)

## 239. [Spotlight] Modular Pretraining Enables Access Control

1. 问题：AI developers face a dual-use dilemma.
2. 方法：提出/研究 **gradient-routed auxiliary modules (GRAM)**；To address this challenge, we propose gradient-routed auxiliary modules (GRAM), a pre-training method that adds modules to a neural network…
3. 机制：To address this challenge, we propose gradient-routed auxiliary modules (GRAM), a pre-training method that adds modules to a neural network and selectively…
4. 结果：These experiments show that GRAM preserves selected retain capabilities while disabling forgotten capabilities, and limits recovery better than post-hoc unlearning.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Modular Pretraining Enables Access Control](https://openreview.net/forum?id=yIubI9l3IT)

## 240. [Oral] Monitoring Monitorability

1. 问题：Safe deployment of increasingly capable AI agents may require visibility into how they make decisions.
2. 方法：提出/研究 **three evaluation archetypes (intervention**；We propose three evaluation archetypes (intervention, process, and outcome-property), a new monitorability metric, and a broad evaluation suite.
3. 机制：We propose three evaluation archetypes (intervention, process, and outcome-property), a new monitorability metric, and a broad evaluation suite.
4. 结果：Finally, we show monitorability can be improved by asking follow-up questions and giving the follow-up CoT to the monitor.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Monitoring Monitorability](https://openreview.net/forum?id=b82fgbMVpz)

## 241. [Oral] Motion Attribution for Video Generation

1. 问题：Despite the rapid progress of video generation models, the role of data in influencing motion is poorly understood.
2. 方法：提出/研究 **Motive**；We present Motive (MOTIon attribution for Video gEneration), a motion-centric, gradient-based data attribution framework that scales to modern, large, high-quality…
3. 机制：Motive isolates temporal dynamics from static appearance via motion-weighted loss masks, yielding efficient and scalable motion-specific influence computation.
4. 结果：With Motive-selected high-influence data, we improve both motion smoothness and dynamic degree on VBench, achieving a 74.1% human preference win rate compared…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Motion Attribution for Video Generation](https://openreview.net/forum?id=zAl9heLw4q)

## 242. [Spotlight] MSP: Probabilistically Consistent Multi-Scale Action Generation

1. 问题：In robotic imitation learning, accurately modeling the multimodality and temporal correlations of long-horizon action sequences remains challenging.
2. 方法：提出/研究 **Probabilistically Consistent Multi-Scale Action Generation (MSP)**；To address these shortcomings, we propose Probabilistically Consistent Multi-Scale Action Generation (MSP), a novel coarse-to-fine approach that promotes cross-scale consistency.
3. 机制：Through extensive simulation and real-world experiments, including long-horizon, multi-task, and few-shot generalization settings, we show that MSP outperforms existing coarse-to-fine methods, achieving…
4. 结果：Through extensive simulation and real-world experiments, including long-horizon, multi-task, and few-shot generalization settings, we show that MSP outperforms existing coarse-to-fine methods, achieving…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[MSP: Probabilistically Consistent Multi-Scale Action Generation](https://openreview.net/forum?id=zqjKnzyRo4)

## 243. [Spotlight] Multimodal Latent Language Modeling with Next-Token Diffusion

1. 问题：Additionally, we develop -VAE to address the challenges of variance collapse, which is crucial for autoregressive modeling.
2. 方法：提出/研究 **Latent Language Modeling (LatentLM)**；In this work, we propose Latent Language Modeling (LatentLM), which seamlessly integrates continuous and discrete data using causal Transformers.
3. 机制：In this work, we propose Latent Language Modeling (LatentLM), which seamlessly integrates continuous and discrete data using causal Transformers.
4. 理论/证据：Specifically, we employ a variational autoencoder (VAE) to represent continuous data as latent vectors and introduce next-token diffusion for autoregressive…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Multimodal Latent Language Modeling with Next-Token Diffusion](https://openreview.net/forum?id=PnTXyTR2VG)

## 244. [Oral] Multimodal Nested Learning for Decoupled and Coordinated Optimization

1. 问题：However, heterogeneous discrepancies across modalities consistently trigger imbalanced multimodal optimization, restricting the joint learning performance.
2. 方法：提出/研究 **novel Multimodal Nested Learning Framework (MoNet)**；To address this issue, we propose a novel Multimodal Nested Learning Framework (MoNet), which reformulates the monolithic framework into nested…
3. 机制：Although existing methods mitigate this issue through optimization modulation and conflict alleviation, they still suffer from entangled optimization and uniform learning pace…
4. 结果：Extensive experimental results on eight datasets across three tasks demonstrate the superiority of MoNet.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Multimodal Nested Learning for Decoupled and Coordinated Optimization](https://openreview.net/forum?id=8XOncDWc5j)

## 245. [Oral] MuonSSM: Orthogonalizing State Space Models for Sequence Modeling

1. 问题：However, existing SSMs often suffer from instability and memory degradation over extended horizons due to poorly conditioned first-order updates and unbalanced update…
2. 方法：提出/研究 **MuonSSM**；We introduce MuonSSM, a general framework that stabilizes SSM training by explicitly conditioning the geometry of memory updates rather than…
3. 机制：We introduce MuonSSM, a general framework that stabilizes SSM training by explicitly conditioning the geometry of memory updates rather than the recurrent…
4. 理论/证据：MuonSSM augments SSMs with a momentum-based pathway and a lightweight Newton-Schulz transformation on low-rank input injections, yielding bounded and spectrally…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[MuonSSM: Orthogonalizing State Space Models for Sequence Modeling](https://openreview.net/forum?id=GmP3VcfHi0)

## 246. [Oral] MV-FGAD: Towards Efficient and Effective Federated Graph Anomaly Detection via Multi-view Learning

1. 问题：However, existing methods suffer from two limitations.
2. 方法：提出/研究 **MV-FGAD**；Specifically, we propose MV-FGAD, an efficient and effective federated GAD framework for mining anomalies of varying strengths.
3. 机制：Federated graph anomaly detection (GAD) aims to identify abnormal nodes in distributed subgraphs through federated learning.
4. 结果：Extensive experiments on real-world datasets of varying types and scales demonstrate MV-FGAD's efficiency and effectiveness.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[MV-FGAD: Towards Efficient and Effective Federated Graph Anomaly Detection via Multi-view Learning](https://openreview.net/forum?id=yBcY0bY45t)

## 247. [Oral] Nash Equilibria in Games with Playerwise Concave Coupling Constraints: Existence and Computation

1. 问题：We study the existence and computation of Nash equilibria in concave games where the players' admissible strategies are subject to shared coupling…
2. 方法：提出/研究 **Nash Equilibria in Games with Playerwise Concave Coupling…**；Under playerwise concavity of constraints, we prove existence of Nash equilibria.
3. 机制：Under playerwise concavity of constraints, we prove existence of Nash equilibria.
4. 理论/证据：Under playerwise concavity of constraints, we prove existence of Nash equilibria.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Nash Equilibria in Games with Playerwise Concave Coupling Constraints: Existence and Computation](https://openreview.net/forum?id=BGmc3O41ZH)

## 248. [Spotlight] Near-Optimal Private Linear Regression via Iterative Hessian Mixing

1. 问题：We study differentially private ordinary least squares (DP-OLS) with bounded data (X,Y) via sketching-based mechanisms.
2. 方法：提出/研究 **Iterative Hessian Mixing (IHM)**；In this work, we propose Iterative Hessian Mixing (IHM), an algorithm that builds on Gaussian-sketching approaches to DP-OLS and is…
3. 机制：We study differentially private ordinary least squares (DP-OLS) with bounded data (X,Y) via sketching-based mechanisms.
4. 结果：We also conduct a rigorous empirical evaluation on a large suite of datasets, demonstrating that IHM consistently outperforms prior baselines, including AdaSSP.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Near-Optimal Private Linear Regression via Iterative Hessian Mixing](https://openreview.net/forum?id=IwP8LZzc97)

## 249. [Spotlight] Neural Concept Verifier: Scaling Prover-Verifier Games via Concept Encodings

1. 问题：While *Prover-Verifier Games* (PVGs) offer a promising path toward verifiability in nonlinear classification models, they have not yet been applied to complex…
2. 方法：提出/研究 ***Neural Concept Verifier (NCV)***；We introduce *Neural Concept Verifier (NCV)*, a unified framework combining PVGs for formal verifiability with concept encodings to handle complex…
3. 机制：We introduce *Neural Concept Verifier (NCV)*, a unified framework combining PVGs for formal verifiability with concept encodings to handle complex, high-dimensional inputs…
4. 结果：Overall, we demonstrate NCV as a promising step toward concept-level, verifiable AI.
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[Neural Concept Verifier: Scaling Prover-Verifier Games via Concept Encodings](https://openreview.net/forum?id=ThxAdzExdS)

## 250. [Spotlight] Neural Feature Geometry Evolves as Discrete Ricci Flow

1. 问题：Deep neural networks learn feature representations via complex geometric transformations of the input data manifold.
2. 方法：提出/研究 **novel framework for locally evaluating geometric transformations throu**；We provide theoretical results on the evolution of these graphs during training, showing that nonlinear activations play a crucial role…
3. 机制：Deep neural networks learn feature representations via complex geometric transformations of the input data manifold.
4. 结果：Our experimental results further suggest connections between the evolution of feature geometry, and training time and network depth.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[Neural Feature Geometry Evolves as Discrete Ricci Flow](https://openreview.net/forum?id=YPH5yCKzYr)

## 251. [Spotlight] Neural Thickets: Diverse Task Experts Are Dense Around Pretrained Weights

1. 问题：Pretraining produces a learned parameter vector that is typically treated as a starting point for further iterative adaptation.
2. 方法：提出/研究 **Neural Thickets**；In this work, we instead view the outcome of pretraining as a distribution over parameter vectors, whose support already contains…
3. 机制：Motivated by this perspective, we explore a simple, fully parallel post-training method that samples N parameter vectors at random, selects the top…
4. 理论/证据：We show that in smaller or insufficiently trained models such expert solutions occupy a negligible fraction of the volume of…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Neural Thickets: Diverse Task Experts Are Dense Around Pretrained Weights](https://openreview.net/forum?id=92oF5bU4cU)

## 252. [Spotlight] Neuro-evolutionary Continual Reinforcement Learning

1. 问题：Deploying robots in open-ended real-world environments demands continual learning capabilities to adapt to an ever-expanding range of tasks.
2. 方法：提出/研究 ****N**euro-**e**volutionary **C**ontinual **R**einforcement **L**earnin**；Inspired by neuroscience, we propose **N**euro-**e**volutionary **C**ontinual **R**einforcement **L**earning (**Nevo-CRL**).
3. 机制：In the learning process, Nevo-CRL iteratively adjusts masks via importance-guided crossover to optimize the policy network connectivity.
4. 结果：Experiments demonstrate that Nevo-CRL achieves state-of-the-art performance among continual RL methods.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Neuro-evolutionary Continual Reinforcement Learning](https://openreview.net/forum?id=Hv0jK8xYcT)

## 253. [Spotlight] NeuronCtrl: Geometry-Aware Safe Closed-Loop Generative Control for Neuronal Microenvironment Dynamics

1. 问题：This view supports high-rate feedback and systematic in-silico evaluation, yet is difficult in practice.
2. 方法：提出/研究 **NeuronCtrl**；We introduce NeuronCtrl, a modular operator-level framework for safe, closed-loop generative control of neuronal microenvironment dynamics.
3. 机制：Safety is enforced via complementary barrier-based mechanisms at both the action and field levels, with minimal intervention.
4. 结果：Experiments across three high-fidelity 3D neuromodulation benchmarks spanning deep brain stimulation, extracellular reaction—diffusion control, and astrocytic potassium regulation demonstrate improved trade-offs among…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[NeuronCtrl: Geometry-Aware Safe Closed-Loop Generative Control for Neuronal Microenvironment Dynamics](https://openreview.net/forum?id=ZK3h2ENA67)

## 254. [Oral] Non-Euclidean Gradient Descent Operates at the Edge of Stability

1. 问题：Despite (apparently) violating classical smoothness assumptions, EoS has been widely observed in deep learning, but its theoretical foundations remain incomplete.
2. 方法：提出/研究 **Non-Euclidean Gradient Descent Operates at the Edge of…**；We provide an interpretation of EoS through the lens of Directional Smoothness [Mishkin et al., 2024].
3. 机制：Through experiments on neural networks, we show that non-Euclidean GD with our generalized sharpness also exhibits progressive sharpening followed by oscillations around…
4. 结果：Through experiments on neural networks, we show that non-Euclidean GD with our generalized sharpness also exhibits progressive sharpening followed by oscillations around…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Non-Euclidean Gradient Descent Operates at the Edge of Stability](https://openreview.net/forum?id=piWlEHb4Db)

## 255. [Spotlight] NonZero: Interaction-Guided Exploration for Multi-Agent Monte Carlo Tree Search

1. 问题：We formalize candidate proposal as a bandit problem over local deviations and derive a proposal rule, NonUCT, with a sublinear local-regret guarantee…
2. 方法：提出/研究 **NonZero**；We propose NonZero, which keeps multi-agent MCTS tractable by running surrogate-guided selection over a low-dimensional nonlinear representation using an interaction-guided…
3. 机制：We propose NonZero, which keeps multi-agent MCTS tractable by running surrogate-guided selection over a low-dimensional nonlinear representation using an interaction-guided proposal rule…
4. 结果：Empirically, NonZero improves sample efficiency and final performance on MatGame, SMAC, and SMACv2 relative to strong model-based and model-free baselines under matched…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[NonZero: Interaction-Guided Exploration for Multi-Agent Monte Carlo Tree Search](https://openreview.net/forum?id=Jh6gq9QsFa)

## 256. [Spotlight] NorMuon: Making Muon more efficient and scalable

1. 问题：The choice of optimizer significantly impacts the training efficiency and computational costs of large language models (LLMs).
2. 方法：提出/研究 **n efficient distributed implementation under the FSDP2 framework that**；To enable practical deployment at scale, we develop an efficient distributed implementation under the FSDP2 framework that distributes orthogonalization computations…
3. 机制：Recently, the Muon optimizer has demonstrated promising results by orthogonalizing parameter updates, improving optimization geometry through better conditioning.
4. 理论/证据：Experiments across multiple model scales demonstrate that NorMuon consistently outperforms both AdamW and Muon, achieving a 21.74\% reduction in training…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[NorMuon: Making Muon more efficient and scalable](https://openreview.net/forum?id=m1IRWFAMsa)

## 257. [Spotlight] OC-space: a Unifying Perspective on Verification of Tree Ensembles

1. 问题：We study the problem of verifying whether certain properties such as robustness or fairness hold in an ensemble of decision trees.
2. 方法：提出/研究 **OC-space**；This problem is known to be NP-hard, with most research targeting a solution to a specific verification task.
3. 机制：We explore the problem through the lens of an ensemble's OC-space: the set of all possible combinations of the individual trees' predictions.
4. 理论/证据：We show that a wide variety of existing verification tasks can be (1) framed as simple searches through OC-space, and…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[OC-space: a Unifying Perspective on Verification of Tree Ensembles](https://openreview.net/forum?id=FLRPkR0N37)

## 258. [Spotlight] Offline Reinforcement Learning of High-Quality Behaviors Under Robust Style Alignment

1. 问题：Existing methods, despite introducing numerous definitions of style, often fail to reconcile these objectives effectively.
2. 方法：提出/研究 **unified definition of behavior style and instantiate it into a…**；To address these challenges, we propose a unified definition of behavior style and instantiate it into a practical framework.
3. 机制：We study offline reinforcement learning of style-conditioned policies using explicit style supervision via subtrajectory labeling functions.
4. 结果：Experiments demonstrate that SCIQL achieves superior performance on both objectives compared to prior offline methods.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Offline Reinforcement Learning of High-Quality Behaviors Under Robust Style Alignment](https://openreview.net/forum?id=jxdjDmWpNX)

## 259. [Oral] OMAC: A Holistic Optimization Framework for LLM-Based Multi-Agent Collaboration

1. 问题：However, the development of such systems often relies on handcrafted methods, and the literature on systematic design and optimization of LLM-based MAS…
2. 方法：提出/研究 **OMAC**；In this work, we introduce OMAC, a general framework designed for holistic optimization of LLM-based MAS.
3. 机制：In this work, we introduce OMAC, a general framework designed for holistic optimization of LLM-based MAS.
4. 结果：Extensive experiments demonstrate the superior performance of OMAC on diverse tasks against recent approaches.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[OMAC: A Holistic Optimization Framework for LLM-Based Multi-Agent Collaboration](https://openreview.net/forum?id=6C4YQcq8YX)

## 260. [Spotlight] OmniFit: Bridging Modalities via Layer-Adaptive Token Compression for Omnimodal Large Language Models

1. 问题：Emerging Omni-modal Large Language Models (OmniLLMs) enable real-time interaction across video, audio, and text but suffer from prohibitive computational costs due to…
2. 方法：提出/研究 **OmniFit**；To address these challenges, we propose OmniFit, a training-free framework that decouples interaction profiling from inference execution.
3. 机制：To address these challenges, we propose OmniFit, a training-free framework that decouples interaction profiling from inference execution.
4. 结果：Extensive experiments on 3 model series across 10 benchmarks demonstrate that OmniFit establishes a new Pareto frontier, retaining 98\% of model performance…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[OmniFit: Bridging Modalities via Layer-Adaptive Token Compression for Omnimodal Large Language Models](https://openreview.net/forum?id=8RY20mLzup)

## 261. [Spotlight] On Efficient Scaling of GNNs via IO-Aware Layers Implementations

1. 问题：Graph Neural Networks (GNNs) are bottlenecked by sparse, irregular memory access.
2. 方法：提出/研究 **GPU kernels that reduce data movement**；For each family, we develop GPU kernels that reduce data movement, improve locality, and remain robust across realistic graphs.
3. 机制：For each family, we develop GPU kernels that reduce data movement, improve locality, and remain robust across realistic graphs.
4. 结果：For SpMM-based layers, properly cached cuSPARSE achieves up to **8** speedup over DGL and outperforms evaluated custom baselines in the majority of…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[On Efficient Scaling of GNNs via IO-Aware Layers Implementations](https://openreview.net/forum?id=w6JVbu7VFo)

## 262. [Oral] On Minimum Depth and Width of Floating-Point Neural Networks for Representing Floating-Point Functions

1. 问题：However, existing results are derived under exact arithmetic and cannot be directly applied to real implementations on computers, which can only use…
2. 方法：提出/研究 **On Minimum Depth and Width of Floating-Point Neural…**；However, existing results are derived under exact arithmetic and cannot be directly applied to real implementations on computers, which can…
3. 机制：However, existing results are derived under exact arithmetic and cannot be directly applied to real implementations on computers, which can only use…
4. 理论/证据：Research on the expressive power of neural networks has identified the minimum depth and width of neural networks that enable…
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[On Minimum Depth and Width of Floating-Point Neural Networks for Representing Floating-Point Functions](https://openreview.net/forum?id=8IxY2DUiBi)

## 263. [Spotlight] On the Accuracy of Newton Step and Influence Function Data Attributions

1. 问题：Despite its widespread use, our theoretical understanding of key data attribution methods — Influence Functions (IF) and a single Newton Step (NS)…
2. 方法：提出/研究 **On the Accuracy of Newton Step and Influence…**；Despite its widespread use, our theoretical understanding of key data attribution methods — Influence Functions (IF) and a single Newton…
3. 机制：Despite its widespread use, our theoretical understanding of key data attribution methods — Influence Functions (IF) and a single Newton Step (NS)…
4. 理论/证据：Despite its widespread use, our theoretical understanding of key data attribution methods — Influence Functions (IF) and a single Newton…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[On the Accuracy of Newton Step and Influence Function Data Attributions](https://openreview.net/forum?id=mDo8XNqopd)

## 264. [Oral] On the Convergence Rate of LoRA Gradient Descent

1. 问题：Although LoRA is simple, its convergence is poorly understood due to the lack of Lipschitz smoothness, a key condition for classic convergence…
2. 方法：提出/研究 **On the Convergence Rate of LoRA Gradient Descent**；In this work, we provide for the first time a non-asymptotic convergence analysis of the *original LoRA gradient descent* algorithm…
3. 机制：In this work, we provide for the first time a non-asymptotic convergence analysis of the *original LoRA gradient descent* algorithm, which reflects…
4. 理论/证据：Although LoRA is simple, its convergence is poorly understood due to the lack of Lipschitz smoothness, a key condition for…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[On the Convergence Rate of LoRA Gradient Descent](https://openreview.net/forum?id=9GRlBVAXq8)

## 265. [Oral] On the Difficulty of Learning a Meta-network for Training Data Selection

1. 问题：We identify two obstacles in properly training MTS: a poor gradient signal-to-noise ratio (GSNR), which causes optimization difficulties, and lack of informative…
2. 方法：提出/研究 **mathematical analysis of MTS**；We present a mathematical analysis of MTS, which reveals the dynamics of normalized data weights and the relation between disparate…
3. 机制：A common strategy is to learn data weights via bi-level optimization, which we refer to as Meta-learning for Training-data Selection (MTS).
4. 结果：Experiments across four benchmarks show consistent improvements, achieving average gains of 5.49\% over training without selection and 2.89\% over the strongest baseline.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[On the Difficulty of Learning a Meta-network for Training Data Selection](https://openreview.net/forum?id=RzgNmKi5Hw)

## 266. [Spotlight] On the Existence of Consistent Adversarial Attacks in High-Dimensional Linear Classification

1. 问题：What fundamentally distinguishes an adversarial attack from a misclassification due to limited model expressivity or finite data?
2. 方法：提出/研究 **new error metric that precisely capture this distinction**；We introduce a new error metric that precisely capture this distinction, quantifying model vulnerability to consistent adversarial attacks — perturbations…
3. 机制：We introduce a new error metric that precisely capture this distinction, quantifying model vulnerability to consistent adversarial attacks — perturbations that preserve…
4. 结果：The theoretical results demonstrate that as models become more overparameterized, their vulnerability to label-preserving perturbations grows, offering theoretical insight into the mechanisms…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[On the Existence of Consistent Adversarial Attacks in High-Dimensional Linear Classification](https://openreview.net/forum?id=PUIivg3GrO)

## 267. [Spotlight] On the Expressive Power of Permutation-Equivariant Weight-Space Networks

1. 问题：However, this may negatively affect expressive power, warranting theoretical investigation.
2. 方法：提出/研究 **On the Expressive Power of Permutation-Equivariant Weight-Space Networks**；Motivated by the growing availability of pretrained models, recent work has demonstrated the effectiveness of weight-space networks across a wide…
3. 机制：Motivated by the growing availability of pretrained models, recent work has demonstrated the effectiveness of weight-space networks across a wide range of…
4. 结果：Guided by our theoretical results, we show that slight modifications to existing weight-space models yield a 34\% improvement over prior SOTA, demonstrating…
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[On the Expressive Power of Permutation-Equivariant Weight-Space Networks](https://openreview.net/forum?id=gQXkbQSZWS)

## 268. [Oral] On the Identifiability of Poisson Branching Structural Causal Model Under Latent Confounding

1. 问题：Causal discovery from observational count data poses unique challenges, particularly when the data exhibit inherent branching structures, such as an upstream ad…
2. 方法：提出/研究 **Latent Confounding Poisson Branching Structural Causal Model (LC-PB-SC**；In this work, we propose a Latent Confounding Poisson Branching Structural Causal Model (LC-PB-SCM) to bridge this gap.
3. 机制：Finally, we propose a practical algorithm to learn causal structures under latent confounding and demonstrate its effectiveness through experiments on both synthetic…
4. 结果：Finally, we propose a practical algorithm to learn causal structures under latent confounding and demonstrate its effectiveness through experiments on both synthetic…
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[On the Identifiability of Poisson Branching Structural Causal Model Under Latent Confounding](https://openreview.net/forum?id=73YmKB7KpW)

## 269. [Spotlight] On the Interplay of Pre-Training, Mid-Training, and RL on Reasoning Language Models

1. 问题：Recent reinforcement learning (RL) techniques have yielded impressive reasoning improvements in language models, yet it remains unclear whether RL truly extends a…
2. 方法：提出/研究 **controlled experimental framework that isolates the causal contributio**；To resolve this ambiguity, we develop a controlled experimental framework that isolates the causal contributions of pre-training, mid-training, and RL-based…
3. 机制：To resolve this ambiguity, we develop a controlled experimental framework that isolates the causal contributions of pre-training, mid-training, and RL-based post-training.
4. 结果：Together, these results clarify the interplay between pre-training, mid-training, and RL, offering a foundation for improving reasoning language models training strategies.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[On the Interplay of Pre-Training, Mid-Training, and RL on Reasoning Language Models](https://openreview.net/forum?id=TBaUfO9znF)

## 270. [Spotlight] On the Limits of LLM Adaptability: Impact of Model-Internalized Priors on Annotation Task Performance

1. 问题：Large Language Models (LLMs) are increasingly used for zero-shot annotation and LLM-as-a-judge tasks, yet their reliability hinges on how model-internalized priors interact…
2. 方法：提出/研究 **Definition-Specific Familiarity (DSF)**；Crucially, we introduce Definition-Specific Familiarity (DSF), which measures alignment between a model's internal concept and the task definition.
3. 机制：Through experiments on toxicity detection across diverse datasets (spanning social media, gaming, news, and forums) using both dense and mixture-of-experts models, we…
4. 结果：Through experiments on toxicity detection across diverse datasets (spanning social media, gaming, news, and forums) using both dense and mixture-of-experts…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[On the Limits of LLM Adaptability: Impact of Model-Internalized Priors on Annotation Task Performance](https://openreview.net/forum?id=oTv2bKG5Qg)

## 271. [Spotlight] On the Optimization Trajectory of DeepWalk Embeddings

1. 问题：However, theoretical guarantees on the resulting embeddings are much less understood.
2. 方法：提出/研究 **On the Optimization Trajectory of DeepWalk Embeddings**；Combined with the idea of _negative sampling_, the DeepWalk algorithm has been shown to be implementable at scale, easily handling…
3. 机制：Combined with the idea of _negative sampling_, the DeepWalk algorithm has been shown to be implementable at scale, easily handling graphs with…
4. 理论/证据：However, theoretical guarantees on the resulting embeddings are much less understood.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[On the Optimization Trajectory of DeepWalk Embeddings](https://openreview.net/forum?id=YKX6FgtL3R)

## 272. [Spotlight] On the Origin of Neural Scaling Laws: from Random Graphs to Natural Language

1. 问题：Scaling laws have played a major role in modern AI, providing predictive power over how model performance will improve with increasing resources.
2. 方法：提出/研究 **On the Origin of Neural Scaling Laws**；This has spurred intense interest in their origin, with a common suggestion being that they arise from power laws already…
3. 机制：This has spurred intense interest in their origin, with a common suggestion being that they arise from power laws already present in…
4. 结果：Finally, we revisit scaling laws for language modeling, demonstrating that several essential results can be reproduced using 2 layer transformers with context…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[On the Origin of Neural Scaling Laws: from Random Graphs to Natural Language](https://openreview.net/forum?id=mu17VSX8q9)

## 273. [Spotlight] On the Power of Source Screening for Learning Shared Feature Extractors

1. 问题：Learning with shared representation is widely recognized as an effective way to separate commonalities from heterogeneity across various heterogeneous sources.
2. 方法：提出/研究 **On the Power of Source Screening for Learning…**；Most existing work includes all related data sources via simultaneously training a common feature extractor and source-specific heads.
3. 机制：We formalize the notion of an informative subpopulation, develop algorithms and practical heuristics for identifying such subsets, and validate their effectiveness through…
4. 结果：We show that, for a broad class of problem instances, training on a carefully selected subset of sources suffices to achieve minimax…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[On the Power of Source Screening for Learning Shared Feature Extractors](https://openreview.net/forum?id=dTMrITkTr5)

## 274. [Spotlight] On the Role of Computation in Reinforcement Learning

1. 问题：How does the amount of compute available to a reinforcement learning (RL) policy affect its learning?
2. 方法：提出/研究 **minimal architecture that can use a variable amount of compute**；Building on prior work in algorithmic learning and model-free planning, we propose a minimal architecture that can use a variable…
3. 机制：Building on prior work in algorithmic learning and model-free planning, we propose a minimal architecture that can use a variable amount of…
4. 结果：On a set 31 different tasks spanning online and offline RL, we show that (1) this architecture achieves stronger performance simply by…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[On the Role of Computation in Reinforcement Learning](https://openreview.net/forum?id=HKzMnBX5B2)

## 275. [Spotlight] On the Sharp Input-Output Analysis of Nonlinear Systems under Adversarial Attacks

1. 问题：With our reformulation as a linear combination of basis functions, we prove that the _2-norm estimator overcomes the challenges posed by an…
2. 方法：提出/研究 **On the Sharp Input-Output Analysis of Nonlinear Systems…**；We provide an estimation error bound that decays with the input memory length and prove its optimality by constructing a…
3. 机制：We provide an estimation error bound that decays with the input memory length and prove its optimality by constructing a problem instance…
4. 理论/证据：With our reformulation as a linear combination of basis functions, we prove that the _2-norm estimator overcomes the challenges posed…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[On the Sharp Input-Output Analysis of Nonlinear Systems under Adversarial Attacks](https://openreview.net/forum?id=xrUgA8PrNN)

## 276. [Spotlight] One Intervention per Component is Enough: Towards Identifiability in Linear Stochastic Dynamics from Steady State

1. 问题：We study the problem of recovering the parameters of a multivariate Ornstein–Uhlenbeck (OU) process from steady-state observational and interventional data.
2. 方法：提出/研究 **recursive learning algorithm that orders SCCs topologically and**；We propose a recursive learning algorithm that orders SCCs topologically and, for each component, isolates its marginal dynamics and solves…
3. 机制：We propose a recursive learning algorithm that orders SCCs topologically and, for each component, isolates its marginal dynamics and solves a linear…
4. 结果：Experiments on synthetic and real datasets demonstrate the effectiveness of our method in recovering parameters and predicting unseen interventions.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[One Intervention per Component is Enough: Towards Identifiability in Linear Stochastic Dynamics from Steady State](https://openreview.net/forum?id=g07aDcWYJ9)

## 277. [Spotlight] Online Conformal Prediction via Universal Portfolio Algorithms

1. 问题：Online conformal prediction (OCP) seeks prediction intervals that achieve long-run 1- coverage for arbitrary (possibly adversarial) data streams, while remaining as informative…
2. 方法：提出/研究 **general regret-to-coverage theory for interval-valued OCP based on the**；Here, we develop a general regret-to-coverage theory for interval-valued OCP based on the (1- )-pinball loss.
3. 机制：Building on this theory, we propose UP-OCP, a parameter-free method for OCP, via a reduction to a two-asset portfolio selection problem, leveraging…
4. 结果：Extensive experiments support that UP-OCP delivers consistently better size/coverage trade-offs than prior online conformal baselines.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Online Conformal Prediction via Universal Portfolio Algorithms](https://openreview.net/forum?id=EKmiOtjZjI)

## 278. [Oral] Optimal and Scalable MAPF via Multi-Marginal Optimal Transport and Schrödinger Bridges

1. 问题：We show that MAPF can be cast as a special class of multi-marginal optimal transport (MMOT) problems with an underlying Markovian structure…
2. 方法：提出/研究 **Optimal and Scalable MAPF via Multi-Marginal Optimal Transport…**；Focusing on the anonymous setting, we establish conditions under which the corresponding LP is feasible, totally unimodular, and yields min-cost…
3. 机制：To adapt the approach to large-scale problems, we cast the MAPF-MMOT in a probabilistic framework via Schrödinger bridges.
4. 结果：Extensive experiments highlight the optimality and scalability of the proposed approaches.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Optimal and Scalable MAPF via Multi-Marginal Optimal Transport and Schrödinger Bridges](https://openreview.net/forum?id=Cxdj2GYZ4c)

## 279. [Oral] Optimal Decision-Making Based on Prediction Sets

1. 问题：Yet, it remains unclear how to use them optimally for downstream decision-making.
2. 方法：提出/研究 **decision-theoretic framework that seeks to minimize the expected loss**；Here, we propose a decision-theoretic framework that seeks to minimize the expected loss (risk) against a worst-case distribution consistent with…
3. 机制：Here, we propose a decision-theoretic framework that seeks to minimize the expected loss (risk) against a worst-case distribution consistent with the prediction…
4. 结果：The source code to reproduce our experiments is available at 
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Optimal Decision-Making Based on Prediction Sets](https://openreview.net/forum?id=VAXW59dyfk)

## 280. [Spotlight] Optimal Rates for Feasible Payoff Set Estimation in Games

1. 问题：We focus on the problem of estimating the set of feasible payoffs with high probability and up to precision on the Hausdorff…
2. 方法：提出/研究 **Optimal Rates for Feasible Payoff Set Estimation in…**；We provide the first minimax-optimal rates for both exact and approximate equilibrium play, in zero-sum as well as general-sum games.
3. 机制：We provide the first minimax-optimal rates for both exact and approximate equilibrium play, in zero-sum as well as general-sum games.
4. 理论/证据：Rather than producing a single payoff estimate, inverse game theory aims to identify the entire set of payoffs consistent with…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Optimal Rates for Feasible Payoff Set Estimation in Games](https://openreview.net/forum?id=qV7yFzdK1R)

## 281. [Spotlight] Optimal structure learning and conditional independence testing

1. 问题：We establish a fundamental connection between optimal structure learning and optimal conditional independence testing by showing that the minimax optimal rate for…
2. 方法：提出/研究 **Optimal structure learning and conditional independence testing**；We establish a fundamental connection between optimal structure learning and optimal conditional independence testing by showing that the minimax optimal…
3. 机制：This theoretical finding provides a unified framework for analyzing the statistical complexity of structure learning through the lens of minimax testing.
4. 结果：This is accomplished by establishing a general reduction between these two problems in the case of poly-forests, and demonstrated by deriving optimal…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Optimal structure learning and conditional independence testing](https://openreview.net/forum?id=uurjpxrLc5)

## 282. [Spotlight] Optimal Transport under Group Fairness Constraints

1. 问题：Ensuring fairness in matching algorithms is a key challenge in allocating scarce resources and positions.
2. 方法：提出/研究 **novel notion of group fairness requiring that the probability of…**；Focusing on Optimal Transport (OT), we introduce a novel notion of group fairness requiring that the probability of matching two…
3. 机制：Focusing on Optimal Transport (OT), we introduce a novel notion of group fairness requiring that the probability of matching two individuals from…
4. 理论/证据：Focusing on Optimal Transport (OT), we introduce a novel notion of group fairness requiring that the probability of matching two…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Optimal Transport under Group Fairness Constraints](https://openreview.net/forum?id=tibRKqUHcv)

## 283. [Oral] OPUS: Towards Efficient and Principled Data Selection in Large Language Model Pre-training in Every Iteration

1. 问题：However, existing methods either rely on heuristic static filters that ignore training dynamics, or use dynamic yet optimizer-agnostic criteria based on raw…
2. 方法：提出/研究 **OPUS**；We propose OPUS (Optimizer-induced Projected Utility Selection), a dynamic framework that defines utility in the optimizer-induced update space.
3. 机制：We propose OPUS (Optimizer-induced Projected Utility Selection), a dynamic framework that defines utility in the optimizer-induced update space.
4. 结果：Beyond online selection, the OPUS utility score also demonstrates potential as a static filter for flagging and removing toxic documents from contaminated…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[OPUS: Towards Efficient and Principled Data Selection in Large Language Model Pre-training in Every Iteration](https://openreview.net/forum?id=lcLxGrk5N9)

## 284. [Oral] Orthogonal Concept Erasure for Diffusion Models

1. 问题：Concept erasure has emerged as a promising approach to mitigate undesired or unsafe content in diffusion models, yet existing methods still face…
2. 方法：提出/研究 ****Orthogonal Concept Erasure (OCE)****；To address this, we propose **Orthogonal Concept Erasure (OCE)**, which reformulates editing-based erasure as multiplicative parameter updates from a geometric…
3. 机制：To address this, we propose **Orthogonal Concept Erasure (OCE)**, which reformulates editing-based erasure as multiplicative parameter updates from a geometric perspective.
4. 结果：Extensive experiments on single- and multi-concept erasure demonstrate that OCE outperforms existing methods in concept erasure and non-target preservation, erasing up to…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Orthogonal Concept Erasure for Diffusion Models](https://openreview.net/forum?id=VE2aKpTWrK)

## 285. [Spotlight] OSM+: Billion-Level Open Street Map Dataset for City-wide Experiments

1. 问题：Road network data provides rich information about cities, but processing worldwide OpenStreetMap (OSM) data is computationally intensive, and the resulting graphs are…
2. 方法：提出/研究 **OSM+**；Existing graph learning benchmarks fail to capture the billion-scale and unique topological properties of real-world road networks, leaving model scalability…
3. 机制：We demonstrate the utility of OSM+ through four illustrative use cases: basic query, city boundary detection, traffic prediction, and traffic policy control.
4. 结果：For traffic prediction, we construct a new 31-city benchmark by processing traffic data and combining it with OSM+, enabling broader spatial coverage…
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[OSM+: Billion-Level Open Street Map Dataset for City-wide Experiments](https://openreview.net/forum?id=CMeeyJzWZ5)

## 286. [Spotlight] Overcoming PINNs Failure Modes In High Dimension With Low-Rank Fourier Sum

1. 问题：Physics-informed neural networks (PINNs) can be unreliable on PDEs with oscillatory, multiscale, stiff, or long-time solutions, and these difficulties worsen in high…
2. 方法：提出/研究 **Low-Rank Fourier Sums (LoRFS)**；We propose Low-Rank Fourier Sums (LoRFS), representing the solution as a low-rank sum of separable Fourier expansions (products of one-dimensional…
3. 机制：We propose Low-Rank Fourier Sums (LoRFS), representing the solution as a low-rank sum of separable Fourier expansions (products of one-dimensional Fourier series…
4. 结果：Across canonical PINN failure-mode benchmarks and their high-dimensional extensions, LoRFS consistently outperforms strong PINN baselines and remains stable in regimes where competing…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Overcoming PINNs Failure Modes In High Dimension With Low-Rank Fourier Sum](https://openreview.net/forum?id=fq3yjso8Tn)

## 287. [Spotlight] OXE-AugE: A Large-Scale Robot Augmentation of OXE for Scaling Cross-Embodiment Policy Learning

1. 问题：As re-collecting demonstrations and retraining for each new embodiment are prohibitively costly, we study whether existing robot data can be augmented to…
2. 方法：提出/研究 **ugE-Toolkit**；We present AugE-Toolkit, a scalable robot augmentation pipeline, and OXE-AugE, a high-quality open-source dataset that augments OXE with 9 different…
3. 机制：We present AugE-Toolkit, a scalable robot augmentation pipeline, and OXE-AugE, a high-quality open-source dataset that augments OXE with 9 different robot embodiments.
4. 结果：In physical experiments, fine-tuning generalist policies such as OpenVLA and _0 on OXE-AugE improves success rates by 24-45% on unseen robot-gripper combinations…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[OXE-AugE: A Large-Scale Robot Augmentation of OXE for Scaling Cross-Embodiment Policy Learning](https://openreview.net/forum?id=LcswwEzzX7)

## 288. [Spotlight] PACT: Self-Evolving Physical Safety Alignment for Diffusion Policies in Embodied Manipulation

1. 问题：Diffusion policies have achieved remarkable success in robotic manipulation, yet they often fail to satisfy strict physical constraints required for safe deployment.
2. 方法：提出/研究 **Physical safety Alignment for Constrained Trajectories (PACT)**；We propose Physical safety Alignment for Constrained Trajectories (PACT), a self-evolving post-training framework that projects pretrained diffusion policies onto constraint-feasible…
3. 机制：Existing approaches impose safety either prematurely during training or reactively via external guardrails at test time, limiting policy expressivity and overall scalability.
4. 结果：On simulated and real-world embodied manipulation benchmarks, PACT significantly reduces safety violations by 31.0% on average while improving task success by 30.7%.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[PACT: Self-Evolving Physical Safety Alignment for Diffusion Policies in Embodied Manipulation](https://openreview.net/forum?id=ePFvXPdvhM)

## 289. [Spotlight] PanoWorld-X: Generating Explorable Panoramic Worlds via Sphere-Aware Video Diffusion

1. 问题：While recent advances in video generation have achieved impressive results, they follow a 2D paradigm that treats content generation as transitions of…
2. 方法：提出/研究 **PanoWorld-X for explorable immersive scene video generation**；To address this, we propose PanoWorld-X for explorable immersive scene video generation.
3. 机制：Our framework is built on the panoramic representation, which naturally maps a 3D scene into a standard format and provides an ideal…
4. 结果：Extensive experiments demonstrate that PanoWorld-X achieves superior performance in motion range, control precision, and visual quality, underscoring its potential for real-world applications.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[PanoWorld-X: Generating Explorable Panoramic Worlds via Sphere-Aware Video Diffusion](https://openreview.net/forum?id=xEgoeNrp8B)

## 290. [Spotlight] PaperBanana: Automating Academic Illustration for AI Scientists

1. 问题：Despite rapid advances in autonomous AI scientists powered by language models, generating publication-ready illustrations remains a labor-intensive bottleneck in the research workflow.
2. 方法：提出/研究 **PaperBanana**；To lift this burden, we introduce PaperBanana, an agentic framework for automated generation of publication-ready academic illustrations.
3. 机制：Powered by state-of-the-art VLMs and image generation models, PaperBanana orchestrates specialized agents to retrieve references, plan content and style, render images, and…
4. 结果：Comprehensive experiments demonstrate that PaperBanana consistently outperforms leading baselines in faithfulness, conciseness, readability, and aesthetics.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[PaperBanana: Automating Academic Illustration for AI Scientists](https://openreview.net/forum?id=FneePKFVHT)

## 291. [Oral] Path-dependent Discrete Amortized Inference

1. 问题：We consider the problem of sampling compositional and discrete objects from a given unnormalized posterior distribution.
2. 方法：提出/研究 **lifting the MDP with a learnable latent dynamics that allows…**；To address these issues, we propose lifting the MDP with a learnable latent dynamics that allows the underlying policy to…
3. 机制：To address these issues, we propose lifting the MDP with a learnable latent dynamics that allows the underlying policy to depend on…
4. 结果：In experiments on standard benchmark problems, we also show that our approach often leads to faster learning convergence and improved…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Path-dependent Discrete Amortized Inference](https://openreview.net/forum?id=viJvYPJHIj)

## 292. [Spotlight] Perceptrons and Localization of Attention’s Mean-Field Landscape

1. 问题：The forward pass of a Transformer can be seen as an interacting particle system on the unit sphere: time plays the role…
2. 方法：提出/研究 **Perceptrons and Localization of Attention’s Mean-Field Landscape**；In some weight settings the system can even be seen as a gradient flow for an explicit energy, and one…
3. 机制：In some weight settings the system can even be seen as a gradient flow for an explicit energy, and one can make…
4. 结果：In this paper we study the effect of the perceptron block in this setting, and show that critical points are…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Perceptrons and Localization of Attention’s Mean-Field Landscape](https://openreview.net/forum?id=rO2yyZiy4v)

## 293. [Oral] PhenoBrain: Phenotype-Conditioned Long-Range Communication for Multi-Modal Brain Network Analysis

1. 问题：However, most existing methods treat phenotypes as auxiliary features and perform late fusion, implicitly assuming that the connectome representation should be learned…
2. 方法：提出/研究 **PhenoBrain**；To bridge this gap, we propose PhenoBrain, a novel framework for multi-modal brain network analysis that injects phenotype information at…
3. 机制：To bridge this gap, we propose PhenoBrain, a novel framework for multi-modal brain network analysis that injects phenotype information at the mechanism…
4. 结果：Extensive experiments demonstrate that PhenoBrain achieves state-of-the-art performance.
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[PhenoBrain: Phenotype-Conditioned Long-Range Communication for Multi-Modal Brain Network Analysis](https://openreview.net/forum?id=9NqKL9QQ4a)

## 294. [Oral] PhotoAgent: Exploratory Visual Aesthetic Planning with Large Vision Models

1. 问题：However, the quality of editing highly depends on carefully designed instructions, placing the burden of task decomposition and sequencing entirely on the…
2. 方法：提出/研究 **PhotoAgent**；To achieve autonomous image editing, we present PhotoAgent, a system that advances image editing through explicit aesthetic planning.
3. 机制：It reasons over user aesthetic intent, plans multi-step editing actions via tree search, and iteratively refines results through closed-loop execution with memory…
4. 结果：Extensive experiments demonstrate that PhotoAgent significantly outperforms existing methods in both instruction faithfulness and visual quality across a diverse range of editing…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[PhotoAgent: Exploratory Visual Aesthetic Planning with Large Vision Models](https://openreview.net/forum?id=Ws8swqL5ob)

## 295. [Spotlight] PLANTAIN: Plan-Answer Interleaved Reasoning

1. 问题：Reasoning models often spend significant time generating hidden reasoning before any visible response, which can waste user time when the model starts…
2. 方法：提出/研究 **PLANTAIN**；Human speakers, in contrast, use lightweight incremental check-ins to maintain common ground, motivating *interleaved reasoning* (IR), where a model alternates…
3. 机制：Human speakers, in contrast, use lightweight incremental check-ins to maintain common ground, motivating *interleaved reasoning* (IR), where a model alternates between internal…
4. 结果：Across challenging math, coding, text-to-SQL, and reading-comprehension benchmarks, PLAINTAIN improves pass@1 by roughly 6% on average while reducing time-to-first-response by over 60%…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[PLANTAIN: Plan-Answer Interleaved Reasoning](https://openreview.net/forum?id=lK2o9OjoXf)

## 296. [Oral] POET-X: Memory-efficient LLM Training by Scaling Orthogonal Transformation

1. 问题：Efficient and stable training of large language models (LLMs) remains a core challenge in modern machine learning systems.
2. 方法：提出/研究 **POET-X**；To overcome these limitations, we introduce POET-X, a scalable and memory-efficient variant that performs orthogonal equivalence transformations with significantly reduced…
3. 机制：To address this challenge, Reparameterized Orthogonal Equivalence Training (POET), a spectrum-preserving framework that optimizes each weight matrix through orthogonal equivalence transformation, has…
4. 结果：In our experiments, POET-X enables the pretraining of billion-parameter LLMs on a single Nvidia H100 GPU, and in contrast, standard optimizers such…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[POET-X: Memory-efficient LLM Training by Scaling Orthogonal Transformation](https://openreview.net/forum?id=et8jpWLUuD)

## 297. [Spotlight] PonderLM-2: Pretraining LLM with Latent Thoughts in Continuous Space

1. 问题：The remarkable success of Chain-of-Thought (CoT), which enhances performance by scaling generation steps at test-time, inspires us to ask: can we leverage…
2. 方法：提出/研究 **novel pre-training methodology**；To address this, we propose a novel pre-training methodology: Pretraining Language Models with Latent Thoughts (PonderLM-2).
3. 机制：To address this, we propose a novel pre-training methodology: Pretraining Language Models with Latent Thoughts (PonderLM-2).
4. 结果：Furthermore, increasing the number of latent thoughts generated before each actual token—forming a chain analogous to CoT—consistently improves the model's…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[PonderLM-2: Pretraining LLM with Latent Thoughts in Continuous Space](https://openreview.net/forum?id=yVFxjNzCQm)

## 298. [Oral] Position: AI Should Facilitate Democratic Deliberation at Scale

1. 问题：We also address critical challenges, including alignment, sycophancy, training bias, and over-reliance on AI systems.
2. 方法：提出/研究 **on the machine learning community to develop delib**；Unlike proposals such as liquid democracy that restructure representation through vote delegation, in this position paper, we argue that AI-assisted…
3. 机制：Unlike proposals such as liquid democracy that restructure representation through vote delegation, in this position paper, we argue that AI-assisted deliberation offers…
4. 结果：Drawing on evidence from online platforms and experimental research, we identify four guiding principles: preserving agency and autonomy, encouraging mutual…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

## 299. [Oral] Position: AI/ML Deepfake Research is Misaligned with AI Generated Non-Consensual Intimate Imagery (AIG-NCII)

1. 问题：AI-generated non-consensual intimate imagery (AIG-NCII) is not adequately addressed in AI/ML literature regarding AI-generated media, commonly referred to as "deepfakes".
2. 方法：提出/研究 **Position**；While research on deepfakes currently focuses on its epistemic harms—or harms relating to truth and authenticity—this is misaligned with the…
3. 机制：While research on deepfakes currently focuses on its epistemic harms—or harms relating to truth and authenticity—this is misaligned with the dominant reality…
4. 结果：We conduct a landscape analysis of highly-cited works to demonstrate that technical interventions addressing deepfakes almost entirely ignore AIG-NCII, limiting…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

## 300. [Oral] Position: Anthropomorphic Misalignment Research Needs Stronger Evidence

1. 问题：By evaluating failure modes across different misalignment concepts, such as deception, emergent misalignment, and sycophancy, we show how conceptual ambiguity, non-robust datasets…
2. 方法：提出/研究 **Position**；To achieve this, we provide a clear call to action through a proposed framework of evidence levels and a diagnostic…
3. 机制：To achieve this, we provide a clear call to action through a proposed framework of evidence levels and a diagnostic checklist.
4. 结果：To achieve this, we provide a clear call to action through a proposed framework of evidence levels and a diagnostic checklist.
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

## 301. [Oral] Position: Don't Just "Fix it in Post'': A Science of AI Must Study Learning Dynamics

1. 问题：What would it mean to have a scientific understanding of AI?
2. 方法：提出/研究 **Position**；Language models are not static objects—they are snapshots of time-evolving processes shaped by data, objectives, and optimization dynamics.
3. 机制：Language models are not static objects—they are snapshots of time-evolving processes shaped by data, objectives, and optimization dynamics.
4. 理论/证据：We envision a hierarchy of scientific maturity: first predict outcomes from early training signals, then intervene when trajectories go wrong…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

## 302. [Oral] Position: Irresponsible AI: big tech’s influence on AI research and associated impacts

1. 问题：The accelerated development, deployment and adoption of artificial intelligence systems has been fuelled by the increasing presence of big tech in the…
2. 方法：提出/研究 **this argument by laying out the factors through which this…**；We develop this argument by laying out the factors through which this influence leads to irresponsible AI.
3. 机制：We develop this argument by laying out the factors through which this influence leads to irresponsible AI.
4. 理论/证据：This position paper argues that irresponsible AI development is strongly driven by big tech's influence and involvement in the field.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

## 303. [Oral] Position: Stop Automating Peer Review Without Rigorous Evaluation

1. 问题：Large language models offer a tempting solution to address the peer review crisis.
2. 方法：提出/研究 **Position**；This position paper argues that today's AI systems should not be used to produce paper reviews.
3. 机制：2) AI review scores are trivially gameable through paper laundering: prompting an LLM to rewrite a paper could significantly increase the scores…
4. 结果：2) AI review scores are trivially gameable through paper laundering: prompting an LLM to rewrite a paper could significantly increase the scores…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

## 304. [Oral] Position: The AI Imperative: Scaling High-Quality Peer Review in Machine Learning

1. 问题：Peer review, the bedrock of scientific advancement in machine learning (ML), is strained by a crisis of scale.
2. 方法：提出/研究 **specific roles for AI in enhancing factual verification**；We propose specific roles for AI in enhancing factual verification, guiding reviewer performance, assisting authors in quality improvement, and supporting…
3. 机制：We propose specific roles for AI in enhancing factual verification, guiding reviewer performance, assisting authors in quality improvement, and supporting ACs in…
4. 结果：We outline a research agenda, including illustrative experiments, to develop and validate these AI assistants, and discuss significant technical and ethical challenges.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

## 305. [Oral] Position: The Alignment Community is Unintentionally Building a Censor’s Toolkit

1. 问题：This position paper argues that modern alignment methods – originally designed to prevent harmful output – are dual-use technologies that may easily…
2. 方法：提出/研究 **Position**；By mapping current alignment techniques to the possibility and actual cases of misuse, we show that the quest for a…
3. 机制：By mapping current alignment techniques to the possibility and actual cases of misuse, we show that the quest for a ''perfectly aligned''…
4. 结果：By mapping current alignment techniques to the possibility and actual cases of misuse, we show that the quest for a…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

## 306. [Oral] Position: There are futures that benchmark-driven AI cannot see

1. 问题：Breakthroughs often come from ideas we could not have predicted in advance.
2. 方法：提出/研究 **mechanisms to restore exaptive capacity without abandoning benchmarkin**；We propose mechanisms to restore exaptive capacity without abandoning benchmarking: plural evaluation regimes, protected venues for non-comparable work, long-horizon funding…
3. 机制：We propose mechanisms to restore exaptive capacity without abandoning benchmarking: plural evaluation regimes, protected venues for non-comparable work, long-horizon funding, and training…
4. 结果：We propose mechanisms to restore exaptive capacity without abandoning benchmarking: plural evaluation regimes, protected venues for non-comparable work, long-horizon funding, and training…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

## 307. [Spotlight] Post-Training with Policy Gradients: Optimality and the Base Model Barrier

1. 问题：However, a barrier arises for going beyond the support of the base model.
2. 方法：提出/研究 **Post-Training with Policy Gradients**；Given a context x, the model must predict the response y Y^N, a sequence of length N that satisfies a…
3. 机制：To overcome this barrier, we study post-training with a process reward model, and demonstrate how PG variants in this setting avoid the…
4. 结果：Along the way, we prove that under the margin condition, SGD with adaptive learning rate (LR) achieves a near optimal test error…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Post-Training with Policy Gradients: Optimality and the Base Model Barrier](https://openreview.net/forum?id=nnWlTi7A7a)

## 308. [Spotlight] Posterior Behavioral Cloning: Pretraining BC Policies for Efficient RL Finetuning

1. 问题：We first show theoretically that standard behavioral cloning (BC) can fail to ensure coverage over the demonstrator's actions, a minimal condition necessary…
2. 方法：提出/研究 **Posterior Behavioral Cloning**；This finetuning step has proved critical in achieving human or super-human performance, yet while much attention has been given to…
3. 机制：This finetuning step has proved critical in achieving human or super-human performance, yet while much attention has been given to developing more…
4. 结果：We then show this approach is practically implementable with modern generative models and leads to significantly improved RL finetuning performance on both…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Posterior Behavioral Cloning: Pretraining BC Policies for Efficient RL Finetuning](https://openreview.net/forum?id=HJ5F3R9Tmd)

## 309. [Spotlight] Practical and Optimal Algorithm for Linear Contextual Bandits with Rare Parameter Updates

1. 问题：We study linear contextual bandits under rare parameter updates: the learner may incorporate reward feedback into its parameter estimate only at a…
2. 方法：提出/研究 **two practical algorithms with only O( T) parameter updates**；For linear contextual bandits, we propose two practical algorithms with only O( T) parameter updates.
3. 机制：For linear contextual bandits, we propose two practical algorithms with only O( T) parameter updates.
4. 理论/证据：Our first algorithm BLCE-G attains minimax-optimal regret (up to polylogarithmic factors in T) simultaneously in both the small-K and large-K…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Practical and Optimal Algorithm for Linear Contextual Bandits with Rare Parameter Updates](https://openreview.net/forum?id=rEqVnZZOiA)

## 310. [Oral] Prescriptive Scaling Reveals the Evolution of Language Model Capabilities

1. 问题：Machine learning model performance arises from competition and application.
2. 方法：提出/研究 **n efficient algorithm that recovers near-full-data frontiers using rou**；Finally, we introduce an efficient algorithm that recovers near-full-data frontiers using roughly 20% of evaluation budget.
3. 机制：Using large-scale observational evaluations with 5k observational and 2k newly sampled data on model performance, we estimate capability boundaries—high conditional quantiles of…
4. 结果：Finally, we introduce an efficient algorithm that recovers near-full-data frontiers using roughly 20% of evaluation budget.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Prescriptive Scaling Reveals the Evolution of Language Model Capabilities](https://openreview.net/forum?id=IkjsHRpuYY)

## 311. [Spotlight] Pressure Reveals Character: Behavioural Alignment Evaluation at Depth

1. 问题：While alignment failures increasingly cause real-world harm, comprehensive evaluation frameworks with realistic multi-turn scenarios remain lacking.
2. 方法：提出/研究 **n alignment benchmark spanning 904 scenarios across six categories—Hon**；We introduce an alignment benchmark spanning 904 scenarios across six categories—Honesty, Safety, Non-Manipulation, Robustness, Corrigibility, and Scheming—validated as realistic by…
3. 机制：We introduce an alignment benchmark spanning 904 scenarios across six categories—Honesty, Safety, Non-Manipulation, Robustness, Corrigibility, and Scheming—validated as realistic by human raters.
4. 结果：We publicly release the benchmark and an interactive leaderboard to support ongoing evaluation, with plans to expand scenarios in areas where we…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Pressure Reveals Character: Behavioural Alignment Evaluation at Depth](https://openreview.net/forum?id=3U1l24EDvL)

## 312. [Oral] Pretrained Vision-Language-Action Models are Surprisingly Resistant to Forgetting in Continual Learning

1. 问题：Continual learning is a long-standing challenge in robot policy learning, where a policy must acquire new skills over time without catastrophically forgetting…
2. 方法：提出/研究 **Pretrained Vision-Language-Action Models are Surprisingly Resistant to Forgetting…**；While prior work has extensively studied continual learning in relatively small behavior cloning (BC) policy models trained from scratch, its…
3. 机制：This knowledge retention enables rapid recovery of seemingly forgotten skills through finetuning.
4. 结果：Simple Experience Replay (ER) works surprisingly well on VLAs, sometimes achieving zero forgetting even with a small replay data size.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Pretrained Vision-Language-Action Models are Surprisingly Resistant to Forgetting in Continual Learning](https://openreview.net/forum?id=VzdSHEab4G)

## 313. [Spotlight] PRISM: Demystifying Retention and Interaction in Mid-Training

1. 问题：Mid-training is increasingly used to improve the reasoning capabilities of large language models (LLMs), yet its design choices and interaction with evaluation…
2. 方法：提出/研究 **PRISM**；We present PRISM (Demystifying Retention and Interaction in Mid-Training), a holistic empirical study that analyzes mid-training design choices, what to…
3. 机制：We present PRISM (Demystifying Retention and Interaction in Mid-Training), a holistic empirical study that analyzes mid-training design choices, what to evaluate, and…
4. 结果：Our results demonstrate that retention-aware mid-training is a necessary intermediate step for reliable reasoning enhancement and RL scaling, and provide practical guidance…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[PRISM: Demystifying Retention and Interaction in Mid-Training](https://openreview.net/forum?id=giNBsVVFGt)

## 314. [Oral] PRISM: Gauge-Invariant Tangent-Space Differentially Private LoRA

1. 问题：However, LoRA's low-rank parameterization poses a fundamental challenge.
2. 方法：提出/研究 ****PRISM****；We propose **PRISM**, an intrinsic DP mechanism for LoRA that is gauge invariant by construction, avoids bilinear noise amplification, and…
3. 机制：Applying differential privacy (DP) via DP-SGD to Low-Rank Adaptation (LoRA) is a natural approach for privacy-preserving fine-tuning.
4. 结果：We establish standard ( , )-DP guarantees for PRISM and introduce a DP-aware, gauge-invariant adaptive update rule that prevents adaptive optimization from…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[PRISM: Gauge-Invariant Tangent-Space Differentially Private LoRA](https://openreview.net/forum?id=SiCjKmArjQ)

## 315. [Spotlight] Privacy-Aware Video Anomaly Detection through Orthogonal Subspace Projection

1. 问题：Video anomaly detection (VAD) systems often prioritize accuracy while overlooking privacy concerns, limiting their suitability for real-world deployment.
2. 方法：提出/研究 **Orthogonal Projection Layer (OPL)**；We propose the Orthogonal Projection Layer (OPL), a lightweight module that removes task-irrelevant variations to produce representations focused on anomaly-relevant…
3. 机制：We propose the Orthogonal Projection Layer (OPL), a lightweight module that removes task-irrelevant variations to produce representations focused on anomaly-relevant cues.
4. 结果：Experiments show that embedding privacy constraints into model design reduces sensitive information while maintaining or improving detection accuracy, supporting projection-based architectures as…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Privacy-Aware Video Anomaly Detection through Orthogonal Subspace Projection](https://openreview.net/forum?id=fjUUmUCy9m)

## 316. [Oral] Procedural Pretraining: Warming Up Language Models with Abstract Data

1. 问题：Pretraining language models directly on web-scale corpora is the de facto paradigm.
2. 方法：提出/研究 **Procedural Pretraining**；We study an alternative where the model is initially exposed to *abstract structured data* to ease the subsequent acquisition of…
3. 机制：We study an alternative where the model is initially exposed to *abstract structured data* to ease the subsequent acquisition of rich semantic…
4. 结果：Our results show that procedural pretraining is a simple, lightweight means of improving performance and accelerating language model pretraining, ultimately suggesting the…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Procedural Pretraining: Warming Up Language Models with Abstract Data](https://openreview.net/forum?id=XFTTezxLdU)

## 317. [Spotlight] Progressive Graph Structure Adjustment for Homophily Shift Adaptation

1. 问题：We propose *Progressive Structure Adjustment for Homophily Shift* (*PSAHS*), a lightweight method for *Graph Domain Adaptation* (*GDA*) that explicitly addresses cross-domain mismatch…
2. 方法：提出/研究 ***Progressive Structure Adjustment for Homophily Shift* (*PSAHS*)**；We propose *Progressive Structure Adjustment for Homophily Shift* (*PSAHS*), a lightweight method for *Graph Domain Adaptation* (*GDA*) that explicitly addresses…
3. 机制：We propose *Progressive Structure Adjustment for Homophily Shift* (*PSAHS*), a lightweight method for *Graph Domain Adaptation* (*GDA*) that explicitly addresses cross-domain mismatch…
4. 结果：Extensive experiments on multiple GDA benchmarks demonstrate that PSAHS consistently outperforms strong baselines, with particularly large gains under severe homophily mismatch, highlighting…
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[Progressive Graph Structure Adjustment for Homophily Shift Adaptation](https://openreview.net/forum?id=OkyO74bJqE)

## 318. [Oral] Protein Autoregressive Modeling via Multiscale Structure Generation

1. 问题：We present protein autoregressive modeling (PAR), the first multi-scale autoregressive framework for protein backbone generation via coarse-to-fine next-scale prediction.
2. 方法：提出/研究 **protein autoregressive modeling (PAR)**；We present protein autoregressive modeling (PAR), the first multi-scale autoregressive framework for protein backbone generation via coarse-to-fine next-scale prediction.
3. 机制：To achieve this, PAR consists of three key components: (i) multi-scale downsampling operations that represent protein structures across multiple scales during training…
4. 结果：On the unconditional generation benchmark, PAR effectively learns protein distributions and produces backbones of high design quality, and exhibits favorable scaling behavior.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Protein Autoregressive Modeling via Multiscale Structure Generation](https://openreview.net/forum?id=08tW615mgI)

## 319. [Oral] Protein Fold Classification at Scale: Benchmarking and Pretraining

1. 问题：Classifying protein topology is essential for deciphering biological function, but progress is held back by the lack of large-scale benchmarks that avoid…
2. 方法：提出/研究 **TEDBench**；We introduce TEDBench, a large-scale, non-redundant benchmark for protein fold classification constructed from the Encyclopedia of Domains (TED) and Foldseek-clustered…
3. 机制：We introduce TEDBench, a large-scale, non-redundant benchmark for protein fold classification constructed from the Encyclopedia of Domains (TED) and Foldseek-clustered AlphaFold structures.
4. 结果：To test transfer beyond AlphaFold structures, we further benchmark on a curated dataset from experimental structures of CATH v4.4.
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[Protein Fold Classification at Scale: Benchmarking and Pretraining](https://openreview.net/forum?id=jPKqiaPTEd)

## 320. [Spotlight] Prototype-guided Bilateral Alignment Multimodal Federated Learning

1. 问题：However, existing methods predominantly rely on idealized assumptions of model homogeneity and balanced modality distributions, rendering them ill-suited for practical scenarios characterized…
2. 方法：提出/研究 **Multimodal Federated learning Prototype-guided Bilateral Alignment (MF**；To address these challenges, we propose a Multimodal Federated learning Prototype-guided Bilateral Alignment (MFedPBA) framework.
3. 机制：MFedPBA facilitates robust knowledge synergy through a dual alignment mechanism: (i) at the feature level, it aligns heterogeneous feature spaces via a…
4. 结果：Extensive experiments demonstrate that our method significantly outperforms state-of-the-art baselines under conditions of model heterogeneity and modality imbalance.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Prototype-guided Bilateral Alignment Multimodal Federated Learning](https://openreview.net/forum?id=aNgkaEagBG)

## 321. [Spotlight] Provable Accuracy Collapse of Embedding-Based Representations under Dimensionality Mismatch

1. 问题：In this work, we prove sharp dimension—accuracy tradeoffs and identify a fundamental information-theoretic limitation: unless the embedding dimension d is chosen close…
2. 方法：提出/研究 **Provable Accuracy Collapse of Embedding-Based Representations under Dimensionality…**；In this work, we prove sharp dimension—accuracy tradeoffs and identify a fundamental information-theoretic limitation: unless the embedding dimension d is…
3. 机制：In this work, we prove sharp dimension—accuracy tradeoffs and identify a fundamental information-theoretic limitation: unless the embedding dimension d is chosen close…
4. 结果：We complement our information-theoretic bounds with strong computational hardness results: under the Unique Games Conjecture, even if the given triplets are nearly…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Provable Accuracy Collapse of Embedding-Based Representations under Dimensionality Mismatch](https://openreview.net/forum?id=ubzXPEfa4R)

## 322. [Spotlight] Provable Bounds for the Learnability of Sample-Compressible Families from Noisy Samples

1. 问题：Learning distribution families over R^d is a fundamental problem in unsupervised learning and statistics.
2. 方法：提出/研究 **Provable Bounds for the Learnability of Sample-Compressible Families…**；In this work, we establish that sample compressible families remain learnable even from perturbed samples, subject to a set of…
3. 机制：In this work, we establish that sample compressible families remain learnable even from perturbed samples, subject to a set of minimax-necessary and…
4. 理论/证据：A central question in this setting is whether a given family of distributions possesses sufficient structure to be (at least)…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Provable Bounds for the Learnability of Sample-Compressible Families from Noisy Samples](https://openreview.net/forum?id=fRonOqrKWT)

## 323. [Spotlight] Provably Convergent Actor-Critic for MARL through Risk-aversion

1. 问题：Learning stationary policies in infinite-horizon general-sum Markov games (MGs) remains a fundamental open problem in Multi-Agent Reinforcement Learning (MARL).
2. 方法：提出/研究 **novel single-timescale Actor-Critic algorithm characterized by a faste**；We propose a novel single-timescale Actor-Critic algorithm characterized by a faster actor and a slower critic.
3. 机制：We propose a novel single-timescale Actor-Critic algorithm characterized by a faster actor and a slower critic.
4. 结果：We empirically validate our algorithm in several environments to demonstrate superior convergence properties compared to risk-neutral baselines.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Provably Convergent Actor-Critic for MARL through Risk-aversion](https://openreview.net/forum?id=NpguYNGrG2)

## 324. [Oral] Quantifying Frontier LLM Capabilities for Container Sandbox Escape

1. 问题：Large language models (LLMs) increasingly act as autonomous agents, using tools to execute code, read and write files, and access networks, creating…
2. 方法：提出/研究 **SandboxEscapeBench**；We introduce SandboxEscapeBench, an open benchmark that safely measures an LLM's capacity to break out of these sandboxes.
3. 机制：We introduce SandboxEscapeBench, an open benchmark that safely measures an LLM's capacity to break out of these sandboxes.
4. 结果：The benchmark is implemented as an Inspect AI Capture the Flag (CTF) evaluation utilising a nested sandbox architecture with the outer layer…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Quantifying Frontier LLM Capabilities for Container Sandbox Escape](https://openreview.net/forum?id=19AbP986bv)

## 325. [Spotlight] RAGEN-2: Reasoning Collapse in Agentic RL

1. 问题：RL training of multi-turn LLM agents is unstable, and reasoning quality drives task performance.
2. 方法：提出/研究 **RAGEN-2**；Entropy, the standard reasoning-stability monitor, only measures within-input diversity and misses whether reasoning depends on the input.
3. 机制：We diagnose it via a **mutual-information (MI) proxy** that scores cross-input distinguishability online; across tasks, MI correlates with final performance far more…
4. 结果：Across planning, math reasoning, web navigation, and code execution, the method consistently improves input dependence and task performance.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[RAGEN-2: Reasoning Collapse in Agentic RL](https://openreview.net/forum?id=01caH9oj7C)

## 326. [Spotlight] Ranking Time Series using a Time Warping Ideal Point Model

1. 问题：The problem is thus transformed into a ranking problem and we introduce an ideal point model adapted to time series data using…
2. 方法：提出/研究 **to rely on a pairwise comparison-based approach**；To address this, we propose to rely on a pairwise comparison-based approach, which provides a more robust alternative to individual…
3. 机制：Finally, we show through multiple experiments that our approach produces accurate and robust rankings under noisy annotation conditions.
4. 结果：Finally, we show through multiple experiments that our approach produces accurate and robust rankings under noisy annotation conditions.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Ranking Time Series using a Time Warping Ideal Point Model](https://openreview.net/forum?id=5wMBxVaTbC)

## 327. [Spotlight] Rapid Poison: Practical Poisoning Attacks Against the Rapid Response Framework

1. 问题：The Rapid Response (RR) framework (Peng et al., 2024), deployed in production systems including Anthropic’s ASL-3 safeguards (Anthropic, 2025), dynamically adapts jailbreak…
2. 方法：提出/研究 **Rapid Poison**；We reveal that prompt injection can infiltrate this pipeline to deliver poisoned samples into the classifier’s training set, enabling two…
3. 机制：We reveal that prompt injection can infiltrate this pipeline to deliver poisoned samples into the classifier’s training set, enabling two attack objectives…
4. 结果：Both attacks flip nearly all target labels with only 1% poisoning rate.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Rapid Poison: Practical Poisoning Attacks Against the Rapid Response Framework](https://openreview.net/forum?id=hvI3Syn2U7)

## 328. [Oral] Rare Event Analysis of Large Language Models

1. 问题：Being probabilistic models, during inference large language models (LLMs) display *rare events*: behaviour that is far from typical but highly significant.
2. 方法：提出/研究 **n end-to-end framework for the systematic analysis of rare events…**；Here we present an end-to-end framework for the systematic analysis of rare events in LLMs.
3. 机制：Here we present an end-to-end framework for the systematic analysis of rare events in LLMs.
4. 理论/证据：Here we present an end-to-end framework for the systematic analysis of rare events in LLMs.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Rare Event Analysis of Large Language Models](https://openreview.net/forum?id=2RJN5vDHG0)

## 329. [Spotlight] Rate or Fate? RLV^ R: Reinforcement Learning with Verifiable Noisy Rewards

1. 问题：Reinforcement learning with verifiable rewards (RLVR) trains a policy by verifying sampled completions and reinforcing higher-scoring outputs, but practical verifiers (e.g., incomplete…
2. 方法：提出/研究 **Rate or Fate? RLV^ R**；We ask when such noise merely slows learning and when it reverses it.
3. 机制：We ask when such noise merely slows learning and when it reverses it.
4. 结果：Experiments on verifiable programming tasks under synthetic noise reproduce the predicted J=0 boundary.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Rate or Fate? RLV^ R: Reinforcement Learning with Verifiable Noisy Rewards](https://openreview.net/forum?id=LwB2EacVT6)

## 330. [Spotlight] Ratio-Variance Regularized Policy Optimization

1. 问题：Standard on-policy reinforcement learning relies on heuristic clipping to enforce trust regions, but this mechanism imposes a severe cost by indiscriminately truncating…
2. 方法：提出/研究 ****R^2VPO****；We introduce **R^2VPO** (Ratio-Variance Regularized Policy Optimization), which implements this constraint via a primal–dual optimization framework.
3. 机制：We introduce **R^2VPO** (Ratio-Variance Regularized Policy Optimization), which implements this constraint via a primal–dual optimization framework.
4. 结果：Furthermore, it consistently outperforms PPO baselines in continuous control domains, particularly in sparse-reward and dynamic environments.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Ratio-Variance Regularized Policy Optimization](https://openreview.net/forum?id=NT4Cz09S4w)

## 331. [Oral] Rational Transductors

1. 问题：Theoretical work establishes that self-attention is limited to AC^0 (under hard attention) or TC^0 (under soft attention), complexity classes that often fail…
2. 方法：提出/研究 **Rational Transductors**；In this work, we introduce Rational Transductors, a dual-stream architecture that augments the Transformer with a matrix-valued recurrence derived from…
3. 机制：By injecting rational state information into the attention mechanism via a *Deep Rational Injection* scheme, our framework strictly generalizes Transformers to capture…
4. 结果：Theoretical analysis and empirical results demonstrate that Rational Transductors solve the "Regular Gap," enabling robust length generalization on algorithmic tasks where standard…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Rational Transductors](https://openreview.net/forum?id=uEZpyELNuB)

## 332. [Spotlight] Real-Time Visual Attribution Streaming in Thinking Model

1. 问题：When these models generate code from a screenshot or solve math problems from images, their long reasoning traces should be grounded in…
2. 方法：提出/研究 **n amortized framework for real-time visual attribution streaming in mu**；We present an amortized framework for real-time visual attribution streaming in multimodal thinking models.
3. 机制：Our results demonstrate that real-time, faithful attribution in multimodal thinking models is achievable through lightweight learning, not brute-force computation.
4. 结果：Our results demonstrate that real-time, faithful attribution in multimodal thinking models is achievable through lightweight learning, not brute-force computation.
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[Real-Time Visual Attribution Streaming in Thinking Model](https://openreview.net/forum?id=eVr10aZZIw)

## 333. [Spotlight] Real-World Unsupervised Models Generalize to Predict Brain Responses to Out-of-Distribution Stimuli

1. 问题：However, these networks remain implausible as models of sensory development, largely because they rely on supervised training with label efficiency far exceeding…
2. 方法：提出/研究 **Real-World Unsupervised Models Generalize to Predict Brain Responses…**；However, these networks remain implausible as models of sensory development, largely because they rely on supervised training with label efficiency…
3. 机制：However, these networks remain implausible as models of sensory development, largely because they rely on supervised training with label efficiency far exceeding…
4. 理论/证据：We show that this performance advantage is not driven by network architecture or dataset size, but rather by the data…
5. 启示：科学机器学习的有效性取决于是否把领域结构、测量过程与不确定性共同纳入模型。

论文页面：[Real-World Unsupervised Models Generalize to Predict Brain Responses to Out-of-Distribution Stimuli](https://openreview.net/forum?id=H1HHss5Zj4)

## 334. [Spotlight] Recovering Policy-Induced Errors: Benchmarking and Trajectory Synthesis for Robust GUI Agents

1. 问题：While GUI agents have advanced rapidly, they often lack the robustness to recover from their own errors, hindering real-world deployment.
2. 方法：提出/研究 **GUI-RobustEval and propose Robustness-driven Trajectory Synthesis**；To bridge this gap at both the evaluation and data levels, we introduce GUI-RobustEval and propose Robustness-driven Trajectory Synthesis.
3. 机制：At the data level, RoTS is a scalable synthesis framework that creates 800k high-quality data via a tree-based pipeline that proactively discovers…
4. 结果：Notably, RoTS-32B achieves state-of-the-art performance on OSWorld, with a 47.4% success rate and a 33.8% All-Pass@4 score, suggesting that improved long-horizon error…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Recovering Policy-Induced Errors: Benchmarking and Trajectory Synthesis for Robust GUI Agents](https://openreview.net/forum?id=iJwDylm93H)

## 335. [Spotlight] Recurrent Equivariant Constraint Modulation: Learning Per-Layer Symmetry Relaxation from Data

1. 问题：Prior work addresses these limitations by relaxing strict equivariance during training, but typically relies on prespecified, explicit, or implicit target levels of…
2. 方法：提出/研究 **Recurrent Equivariant Constraint Modulation (RECM)**；We propose Recurrent Equivariant Constraint Modulation (RECM), a layer-wise constraint modulation mechanism that learns appropriate relaxation levels solely from the…
3. 机制：We propose Recurrent Equivariant Constraint Modulation (RECM), a layer-wise constraint modulation mechanism that learns appropriate relaxation levels solely from the training signal…
4. 结果：Empirically, RECM outperforms prior methods across diverse exact and approximate equivariant tasks, including the challenging molecular conformer generation on the GEOM-Drugs dataset.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Recurrent Equivariant Constraint Modulation: Learning Per-Layer Symmetry Relaxation from Data](https://openreview.net/forum?id=STeISpzNSd)

## 336. [Spotlight] Recurrent Structural Policy Gradient for Partially Observable Mean Field Games

1. 问题：However, algorithmic progress has been limited since model-free methods are high variance and exact methods scale poorly.
2. 方法：提出/研究 ***Recurrent Structural Policy Gradient* (RSPG)**；We propose *Recurrent Structural Policy Gradient* (RSPG), the first history-aware HSM for MFGs with public partial information.
3. 机制：We propose *Recurrent Structural Policy Gradient* (RSPG), the first history-aware HSM for MFGs with public partial information.
4. 结果：RSPG achieves an order-of-magnitude faster convergence than model-free RL methods while learning history-aware behaviour, unlike current HSMs.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Recurrent Structural Policy Gradient for Partially Observable Mean Field Games](https://openreview.net/forum?id=VkZQThGNgI)

## 337. [Spotlight] RED-HDP-HMM: Observation-Dependent Durations for Bayesian Nonparametric Sequential Models

1. 问题：However, both models assume stationary state durations, which limits their expressive power.
2. 方法：提出/研究 **Gibbs sampling method for efficient inference in this model**；We propose a Gibbs sampling method for efficient inference in this model.
3. 机制：We propose a Gibbs sampling method for efficient inference in this model.
4. 结果：Empirical results on both synthetic and real-world segmentation tasks demonstrate that RED-HDP-HMM consistently outperforms the disentangled sticky HDP-HMM and the…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[RED-HDP-HMM: Observation-Dependent Durations for Bayesian Nonparametric Sequential Models](https://openreview.net/forum?id=MqhcqHVc8l)

## 338. [Spotlight] Reinforced Sequential Monte Carlo for Amortised Sampling

1. 问题：This paper proposes a synergy of amortised and particle-based methods for sampling from distributions defined by unnormalised density functions.
2. 方法：提出/研究 **n off-policy RL training procedure for the sampler that uses…**；Exploiting this connection, we introduce an off-policy RL training procedure for the sampler that uses samples from SMC — using…
3. 机制：Exploiting this connection, we introduce an off-policy RL training procedure for the sampler that uses samples from SMC — using the learnt…
4. 结果：On synthetic multi-modal targets (in both continuous and discrete spaces) and the Boltzmann distribution of alanine dipeptide conformations, we demonstrate improvements in…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Reinforced Sequential Monte Carlo for Amortised Sampling](https://openreview.net/forum?id=DWaToCuNwa)

## 339. [Spotlight] RelaxFlow: Text-Driven Amodal 3D Generation

1. 问题：Image-to-3D generation faces inherent semantic ambiguity under occlusion, where partial observation alone is often insufficient to determine object category.
2. 方法：提出/研究 ****RelaxFlow****；To this end, we propose **RelaxFlow**, a training-free dual-branch framework that decouples control granularity via a Multi-Prior Consensus Module and…
3. 机制：To this end, we propose **RelaxFlow**, a training-free dual-branch framework that decouples control granularity via a Multi-Prior Consensus Module and a Relaxation…
4. 结果：Extensive experiments demonstrate that RelaxFlow successfully steers the generation of unseen regions to match the prompt intent without compromising visual fidelity.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[RelaxFlow: Text-Driven Amodal 3D Generation](https://openreview.net/forum?id=UamxHbDR3p)

## 340. [Oral] ReQAT: Achieving Full-Precision Reasoning Accuracy with 4-bit Floating-Point Quantization-Aware Training

1. 问题：Large Reasoning Models (LRMs) achieve strong problem-solving through long chain-of-thought, but their deployment is constrained by the high cost of full-precision inference…
2. 方法：提出/研究 **ReQAT**；Based on this insight, we propose ReQAT, a reasoning-centric FP4 training framework with three components: (i) Trace-Aligned QAT (TAQ), which…
3. 机制：Large Reasoning Models (LRMs) achieve strong problem-solving through long chain-of-thought, but their deployment is constrained by the high cost of full-precision inference…
4. 结果：Large Reasoning Models (LRMs) achieve strong problem-solving through long chain-of-thought, but their deployment is constrained by the high cost of full-precision inference…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[ReQAT: Achieving Full-Precision Reasoning Accuracy with 4-bit Floating-Point Quantization-Aware Training](https://openreview.net/forum?id=aKY52fnzgc)

## 341. [Spotlight] Required Spine Optional Limbs: Heterogeneous Federated Learning via Backbone-sharing and Activation-guided Selection

1. 问题：Although Federated Learning (FL) offers advantages in privacy-preserving for cross-device collaborative learning, its practical deployment remains severely constrained by heterogeneous hardware resources…
2. 方法：提出/研究 **Required Spine Optional Limbs**；Sub-model extraction has emerged as a widely adopted strategy for enabling collaborative training among devices with heterogeneous models.
3. 机制：Sub-model extraction has emerged as a widely adopted strategy for enabling collaborative training among devices with heterogeneous models.
4. 结果：Experimental results demonstrate that compared with state-of-the-art heterogeneous FL methods, SpineFL can achieve up to 3.28% accuracy improvement.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Required Spine Optional Limbs: Heterogeneous Federated Learning via Backbone-sharing and Activation-guided Selection](https://openreview.net/forum?id=8LZfyxIQdO)

## 342. [Spotlight] Rethinking LLM Ensembling from the Perspective of Mixture Models

1. 问题：This idea has been naturally extended to large language models (LLMs), yielding improved performance but incurring substantial computational cost.
2. 方法：提出/研究 **Mixture-model-like Ensemble (ME)**；In this paper, we propose the Mixture-model-like Ensemble (ME).
3. 机制：In this paper, we propose the Mixture-model-like Ensemble (ME).
4. 结果：This idea has been naturally extended to large language models (LLMs), yielding improved performance but incurring substantial computational cost.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Rethinking LLM Ensembling from the Perspective of Mixture Models](https://openreview.net/forum?id=YVk8EDxBWx)

## 343. [Spotlight] Revenue Guarantees of No-Swap-Regret Dynamics in First Price Auctions

1. 问题：We study the revenue of approximate correlated equilibrium in discrete first price auctions - the set of allowable bids is B =…
2. 方法：提出/研究 **Revenue Guarantees of No-Swap-Regret Dynamics in First Price…**；We show that the revenue of any -approximate correlated equilibrium is at least v_2 - (1/k)- ( k^2), where v_2…
3. 机制：We show that the revenue of any -approximate correlated equilibrium is at least v_2 - (1/k)- ( k^2), where v_2 0 is…
4. 理论/证据：We show that the revenue of any -approximate correlated equilibrium is at least v_2 - (1/k)- ( k^2), where v_2…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Revenue Guarantees of No-Swap-Regret Dynamics in First Price Auctions](https://openreview.net/forum?id=n50Ipdt5d5)

## 344. [Spotlight] Reverse Flow Matching: A Unified Framework for Online Reinforcement Learning with Diffusion and Flow Policies

1. 问题：Diffusion and flow policies are gaining prominence in online reinforcement learning (RL) due to their expressive power, yet training them efficiently remains…
2. 方法：提出/研究 **unified framework**；In this paper, we propose a unified framework, reverse flow matching (RFM), which rigorously addresses the problem of training diffusion…
3. 机制：In this paper, we propose a unified framework, reverse flow matching (RFM), which rigorously addresses the problem of training diffusion and flow…
4. 结果：We instantiate RFM to train a flow policy in online RL and demonstrate improved performance on continuous-control benchmarks compared to diffusion policy…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Reverse Flow Matching: A Unified Framework for Online Reinforcement Learning with Diffusion and Flow Policies](https://openreview.net/forum?id=vUpEe4yd1T)

## 345. [Oral] ReViT: Rotational-equivariant Vision Transformers for Neural PDE Solvers

1. 问题：However, the standard Transformer architectures widely used in physics foundation models do not enforce these constraints by construction.
2. 方法：提出/研究 **ReViT**；We introduce ReViT, a rotationally equivariant Vision Transformer framework for neural PDE solvers operating on grid-based physical fields that achieves…
3. 机制：Built on a hierarchical Swin-style backbone with a precomputed reference basis pyramid, ReViT preserves equivariance across multi-scale operations.
4. 结果：ReViT exhibits strong generalization, and reduces MSE by up to 65\% compared with the best-performing alternatives.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[ReViT: Rotational-equivariant Vision Transformers for Neural PDE Solvers](https://openreview.net/forum?id=fy2IXBBThK)

## 346. [Spotlight] Reward and Guidance through Rubrics: Promoting Exploration to Improve Multi-Domain Reasoning

1. 问题：In this paper, we address these limitations by leveraging rubrics to provide both fine-grained reward signals and offline guidance.
2. 方法：提出/研究 **RGR-GRPO**；We propose RGR-GRPO (Reward and Guidance through Rubrics), a rubric-driven RL framework for multi-domain reasoning.
3. 机制：Notably, RGR-GRPO maintains stable entropy fluctuations during off-policy training and achieves superior pass@k performance, reflecting sustained exploration and effective breakthrough beyond existing…
4. 结果：Notably, RGR-GRPO maintains stable entropy fluctuations during off-policy training and achieves superior pass@k performance, reflecting sustained exploration and effective breakthrough beyond existing…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Reward and Guidance through Rubrics: Promoting Exploration to Improve Multi-Domain Reasoning](https://openreview.net/forum?id=AfqsNFzJcs)

## 347. [Spotlight] Reward Redistribution for CVaR MDPs using a Bellman Operator on L-infinity

1. 问题：However, unless restricted to a specialized class of admissible value functions, this formulation induces sparse rewards and degenerate fixed points.
2. 方法：提出/研究 **novel formulation of the static CVaR objective based on augmentation**；In this work, we propose a novel formulation of the static CVaR objective based on augmentation.
3. 机制：In this work, we propose a novel formulation of the static CVaR objective based on augmentation.
4. 结果：Empirical results demonstrate that our algorithms successfully learn CVaR-sensitive policies and achieve effective performance-safety trade-offs.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Reward Redistribution for CVaR MDPs using a Bellman Operator on L-infinity](https://openreview.net/forum?id=8LVv9hyMII)

## 348. [Oral] Reward-free Alignment for Conflicting Objectives

1. 问题：However, many real-world alignment problems involve multiple conflicting objectives, where naive aggregation of preferences can lead to unstable training and poor trade-offs.
2. 方法：提出/研究 ****R**eward-free **A**lignment framework for **C**onflicted **O**bjecti**；First, we propose a **R**eward-free **A**lignment framework for **C**onflicted **O**bjectives (RACO) that directly leverages pairwise preference data and resolves gradient…
3. 机制：First, we propose a **R**eward-free **A**lignment framework for **C**onflicted **O**bjectives (RACO) that directly leverages pairwise preference data and resolves gradient conflicts via…
4. 结果：Both qualitative and quantitative evaluations on multi-objective summarization and safety alignment tasks across multiple LLM families (Qwen 3, Llama 3, Gemma 3)…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Reward-free Alignment for Conflicting Objectives](https://openreview.net/forum?id=vSzRJyg6k0)

## 349. [Oral] Rex: A Family of Reversible Exponential (Stochastic) Runge-Kutta Solvers

1. 问题：Standard solvers, however, accumulate discretization errors that prohibit *exact inversion*, an inaccuracy that is unacceptable in precision-critical applications.
2. 方法：提出/研究 ***Rex***；In this work, we propose *Rex*, a family of reversible exponential (stochastic) Runge-Kutta solvers obtained by applying Lawson methods to…
3. 机制：In this work, we propose *Rex*, a family of reversible exponential (stochastic) Runge-Kutta solvers obtained by applying Lawson methods to convert any…
4. 结果：Beyond a rigorous theoretical analysis—establishing arbitrary-order convergence and a non-zero region of linear stability—we empirically demonstrate that *Rex* achieves near-machine-precision reconstruction and…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Rex: A Family of Reversible Exponential (Stochastic) Runge-Kutta Solvers](https://openreview.net/forum?id=7pQIzVNctu)

## 350. [Oral] Riemannian Metric Matching for Scalable Geometric Modeling of Distributions

1. 问题：Our key observation is that the carré du champ operator can be formulated as a conditional expectation over random perturbations of the…
2. 方法：提出/研究 ****Riemannian metric matching****；We propose **Riemannian metric matching**: a denoising probabilistic framework for learning the Riemannian geometry of data using neural networks.
3. 机制：We propose **Riemannian metric matching**: a denoising probabilistic framework for learning the Riemannian geometry of data using neural networks.
4. 结果：Empirically, metric matching rivals or improves the accuracy of k-NN-based diffusion geometry estimators, while enabling amortized inference that is up to 400…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Riemannian Metric Matching for Scalable Geometric Modeling of Distributions](https://openreview.net/forum?id=KVzXnWPLgX)

## 351. [Oral] RoboMME: Benchmarking and Understanding Memory for Robotic Generalist Policies

1. 问题：Recent vision-language-action (VLA) models have begun to incorporate memory mechanisms; however, their evaluations remain confined to narrow, non-standardized settings.
2. 方法：提出/研究 ****RoboMME****；To address these challenges, we introduce **RoboMME**: a large-scale standardized benchmark for evaluating and advancing VLA models in long-horizon, history-dependent…
3. 机制：Our benchmark comprises 16 manipulation tasks constructed under a carefully designed taxonomy that evaluates *temporal*, *spatial*, *object*, and *procedural* memory.
4. 结果：Our benchmark comprises 16 manipulation tasks constructed under a carefully designed taxonomy that evaluates *temporal*, *spatial*, *object*, and *procedural* memory.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[RoboMME: Benchmarking and Understanding Memory for Robotic Generalist Policies](https://openreview.net/forum?id=8m30ogkPk2)

## 352. [Spotlight] Robust Causal Discovery in Real-World Time Series with Power-Laws

1. 问题：Many algorithms for Causal Discovery (CD) have been proposed; however, they often exhibit a high sensitivity to noise, resulting in spurious causal…
2. 方法：提出/研究 **Robust Causal Discovery in Real-World Time Series with…**；Many algorithms for Causal Discovery (CD) have been proposed; however, they often exhibit a high sensitivity to noise, resulting in…
3. 机制：Many algorithms for Causal Discovery (CD) have been proposed; however, they often exhibit a high sensitivity to noise, resulting in spurious causal…
4. 结果：Our method consistently outperforms state-of-the-art alternatives on both synthetic benchmarks and real-world datasets with known causal structures, demonstrating its robustness…
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[Robust Causal Discovery in Real-World Time Series with Power-Laws](https://openreview.net/forum?id=7i8d203tky)

## 353. [Oral] Robust Contextual Optimization with Missing Covariates

1. 问题：In practice, however, such covariates are often only partially observed due to, e.g., data source heterogeneity or costly data collection.
2. 方法：提出/研究 **Robust Contextual Optimization with Missing Covariates**；In practice, however, such covariates are often only partially observed due to, e.g., data source heterogeneity or costly data collection.
3. 机制：In practice, however, such covariates are often only partially observed due to, e.g., data source heterogeneity or costly data collection.
4. 结果：Empirical results across a range of contextual decision-making tasks demonstrate that the proposed integrated approach consistently outperforms state-of-the-art baselines, including various impute-then-optimize…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Robust Contextual Optimization with Missing Covariates](https://openreview.net/forum?id=37KrsS7g7c)

## 354. [Spotlight] Robust Filter Attention: Self-Attention as Precision-Weighted State Estimation

1. 问题：On language modeling benchmarks, RFA achieves lower perplexity than RoPE within the training window while remaining stable under zero-shot extrapolation to longer…
2. 方法：提出/研究 **Robust Filter Attention (RFA)**；We introduce Robust Filter Attention (RFA), a formulation of self-attention as a robust state estimator.
3. 机制：We introduce Robust Filter Attention (RFA), a formulation of self-attention as a robust state estimator.
4. 结果：On language modeling benchmarks, RFA achieves lower perplexity than RoPE within the training window while remaining stable under zero-shot extrapolation to longer…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Robust Filter Attention: Self-Attention as Precision-Weighted State Estimation](https://openreview.net/forum?id=GhI6lw5QKe)

## 355. [Oral] Robust Harmful Features Under Jailbreak Attacks: Mechanistic Evidence from Attention Head Specialization in Large Language Models

1. 问题：Jailbreak attacks bypass LLM safety alignment, yet their mechanisms remain poorly understood.
2. 方法：提出/研究 **Robust Harmful Features Under Jailbreak Attacks**；We provide evidence that attacks do not comprehensively eliminate safety features, but instead selectively suppress specific attention heads.
3. 机制：Token-level attribution further shows that ACH suppression is driven specifically by attack-template tokens, providing a mechanistic account of why attacks can bypass…
4. 理论/证据：We identify two functionally differentiated types: **Adversarially Compromised Heads (ACHs)** concentrated in early layers, which are suppressed under attacks, and…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Robust Harmful Features Under Jailbreak Attacks: Mechanistic Evidence from Attention Head Specialization in Large Language Models](https://openreview.net/forum?id=LTF6LtBo0E)

## 356. [Spotlight] Root Cause Analysis of Failures in Microservices via Bayesian Root Cause Discovery

1. 问题：Modern cloud systems rely on architectures with many interconnected microservices, which enable scalability and flexibility but make troubleshooting failures difficult.
2. 方法：提出/研究 **Bayesian Root Cause Discovery (BRCD)**；We introduce Bayesian Root Cause Discovery (BRCD), which leverages a partial causal structure (a CPDAG learned during the pre-failure period)…
3. 机制：We introduce Bayesian Root Cause Discovery (BRCD), which leverages a partial causal structure (a CPDAG learned during the pre-failure period) and performs…
4. 结果：Empirically, across synthetic benchmarks and three microservice systems (Online Boutique, Sockshop, Petshop), BRCD achieves state-of-the-art top-l accuracy while remaining effective in low-failure-sample…
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[Root Cause Analysis of Failures in Microservices via Bayesian Root Cause Discovery](https://openreview.net/forum?id=EOSV5tlpqg)

## 357. [Spotlight] Rotary Position Encodings for Graphs

1. 问题：We study the extent to which rotary position encodings (RoPE), a recent transformer position encoding algorithm broadly adopted in large language models…
2. 方法：提出/研究 **Rotary Position Encodings for Graphs**；We find that rotating tokens depending on the spectrum of the graph Laplacian efficiently injects structural information into the attention…
3. 机制：We find that rotating tokens depending on the spectrum of the graph Laplacian efficiently injects structural information into the attention mechanism, boosting…
4. 理论/证据：This approach, coined _Wave-Induced Rotary Encodings_ (WIRE), enjoys intriguing theoretical properties: it recovers regular RoPE on grids, and depends asymptotically…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Rotary Position Encodings for Graphs](https://openreview.net/forum?id=trn64znfNx)

## 358. [Spotlight] S^3GNN: Efficient Global Mixing and Local Message Passing for Long-Range Graph Learning

1. 问题：Message-passing neural networks (MPNNs) often suffer from an information bottleneck when capturing long-range dependencies, leading to the oversquashing (OSQ) phenomenon.
2. 方法：提出/研究 **S^3GNN**；Alongside spatial connectivity enrichment (e.g., rewiring), recent studies have shown that spectral filtering can yield strong long-range learning outcomes, as…
3. 机制：Alongside spatial connectivity enrichment (e.g., rewiring), recent studies have shown that spectral filtering can yield strong long-range learning outcomes, as spectral operators…
4. 结果：Extensive experiments across diverse domains (e.g., long-range benchmarks, KGQA, and mesh-based fluid dynamics) demonstrate that S^3GNN achieves up to an order-of-magnitude error…
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[S^3GNN: Efficient Global Mixing and Local Message Passing for Long-Range Graph Learning](https://openreview.net/forum?id=9SCVnAxoKK)

## 359. [Spotlight] Safety Alignment of LMs via Non-cooperative Games

1. 问题：Ensuring the safety of language models (LMs) while maintaining their usefulness remains a critical challenge in AI alignment.
2. 方法：提出/研究 **different paradigm**；We introduce a different paradigm: framing safety alignment as a non-zero-sum game between an Attacker LM and a Defender LM…
3. 机制：We introduce a different paradigm: framing safety alignment as a non-zero-sum game between an Attacker LM and a Defender LM trained jointly…
4. 理论/证据：We introduce a different paradigm: framing safety alignment as a non-zero-sum game between an Attacker LM and a Defender LM…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Safety Alignment of LMs via Non-cooperative Games](https://openreview.net/forum?id=Bve790HQrA)

## 360. [Spotlight] SAW-Bench: Learning Situated Awareness in the Real World

1. 问题：However, most existing benchmarks for multimodal foundation models (MFMs) emphasize **environment-centric** spatial relations (relations among objects in a scene), while largely overlooking…
2. 方法：提出/研究 **SAW-Bench**；To bridge this gap, we introduce SAW-Bench (**S**ituated **A**wareness in the Real **W**orld), a novel benchmark for evaluating egocentric situated…
3. 机制：SAW-Bench comprises 786 self-recorded videos captured with Ray-Ban Meta (Gen 2) smart glasses spanning diverse indoor and outdoor environments, and over 2071…
4. 结果：We position SAW-Bench as a benchmark for situated spatial intelligence, moving beyond passive observation to understanding physically grounded, observer-centric dynamics.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[SAW-Bench: Learning Situated Awareness in the Real World](https://openreview.net/forum?id=8lwrYjv6r7)

## 361. [Oral] Scalable Event Cloud Network for Event-based Classification

1. 问题：Event cameras are biologically inspired sensors garnering significant attention from both industry and academia.
2. 方法：提出/研究 **Scalable Network named SECNet to leverage Event Cloud representation**；In this paper, we propose a Scalable Network named SECNet to leverage Event Cloud representation.
3. 机制：SECNet integrates polarity at the structural level by innovating the Event-based Group and Sampling module rather than only at the input level.
4. 结果：We conducted extensive experiments on ten event-based datasets, and substantiate the scalability, effectiveness, and efficiency of SECNet.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Scalable Event Cloud Network for Event-based Classification](https://openreview.net/forum?id=yAAUcDLYMR)

## 362. [Spotlight] Scalable Option Learning in High-Throughput Environments

1. 问题：In this work, we identify and solve several key challenges in scaling online hierarchical RL to high-throughput environments.
2. 方法：提出/研究 **Scalable Option Learning (SOL)**；We propose Scalable Option Learning (SOL), a highly scalable hierarchical policy gradient algorithm which achieves a ~35x higher throughput compared…
3. 机制：We propose Scalable Option Learning (SOL), a highly scalable hierarchical policy gradient algorithm which achieves a ~35x higher throughput compared to existing…
4. 结果：To demonstrate SOL's performance and scalability, we train hierarchical agents using 30 billion frames of experience on the complex game of NetHack…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Scalable Option Learning in High-Throughput Environments](https://openreview.net/forum?id=p2RPRTPPMO)

## 363. [Spotlight] SCALE: Self-uncertainty Conditioned Adaptive Looking and Execution for Vision-Language-Action Models

1. 问题：However, existing TTS methods for VLAs require additional training, verifiers, and multiple forward passes, making them impractical for deployment.
2. 方法：提出/研究 **SCALE**；To address these limitations, we propose SCALE, a simple inference strategy that jointly modulates visual perception and action based on…
3. 机制：To address these limitations, we propose SCALE, a simple inference strategy that jointly modulates visual perception and action based on 'self-uncertainty', inspired…
4. 结果：Experiments on simulated and real-world benchmarks demonstrate that SCALE improves state-of-the-art VLAs and outperforms existing TTS methods while maintaining single-pass efficiency.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[SCALE: Self-uncertainty Conditioned Adaptive Looking and Execution for Vision-Language-Action Models](https://openreview.net/forum?id=7MlfE2Da2W)

## 364. [Spotlight] ScaleMoE: Mixture-of-Experts for Scalable Continuous Control in Actor-Critic Reinforcement Learning

1. 问题：Scaling network remains a bottleneck in deep reinforcement learning (RL): simply enlarging actor–critic networks destabilizes training and soon saturates performance.
2. 方法：提出/研究 **ScaleMoE**；Although recent monolithic architectures such as SimBa and BRC have shown that carefully designed inductive biases can enable positive scaling…
3. 机制：This work introduces ScaleMoE, a scalable RL architecture that integrates Mixture-of-Experts (MoE) modules into both the actor and critic of modern continuous…
4. 结果：Results demonstrate that ScaleMoE provides an efficient and effective scaling axis for deep RL in continuous control.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[ScaleMoE: Mixture-of-Experts for Scalable Continuous Control in Actor-Critic Reinforcement Learning](https://openreview.net/forum?id=oVS7o5jKJF)

## 365. [Spotlight] Scaling Law for Quantization-Aware Training

1. 问题：Large language models (LLMs) demand substantial computational and memory resources, creating deployment challenges.
2. 方法：提出/研究 **Scaling Law for Quantization-Aware Training**；Quantization-aware training (QAT) addresses these challenges by reducing model precision while maintaining performance.
3. 机制：Through 268 QAT experiments, we show that quantization error decreases as model size increases, but rises with more training tokens and coarser…
4. 结果：These findings offer key insights for improving QAT research and development.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Scaling Law for Quantization-Aware Training](https://openreview.net/forum?id=fXr3uPr1G5)

## 366. [Spotlight] Scaling Real-World Robot Policy Evaluation via Discrete Diffusion World Model

1. 问题：Evaluating generalist robot manipulation policies is costly and difficult to scale in the real world.
2. 方法：提出/研究 **dWorldEval**；To address this, we propose dWorldEval, an action-centric discrete-diffusion world model that maps visual observations, language instructions, and action chunks…
3. 机制：Extensive experiments on LIBERO, RoboTwin, and real-robot tasks demonstrate that dWorldEval significantly outperforms video diffusion baselines in action controllability, stabilizes long-horizon multi-view…
4. 结果：Extensive experiments on LIBERO, RoboTwin, and real-robot tasks demonstrate that dWorldEval significantly outperforms video diffusion baselines in action controllability, stabilizes long-horizon multi-view…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Scaling Real-World Robot Policy Evaluation via Discrete Diffusion World Model](https://openreview.net/forum?id=93uNlQ1Qp0)

## 367. [Spotlight] SceneSmith: Agentic Generation of Simulation-Ready Indoor Scenes

1. 问题：Simulation has become a key tool for training and evaluating home robots at scale, yet existing environments fail to capture the diversity…
2. 方法：提出/研究 **SceneSmith**；We introduce SceneSmith, a hierarchical agentic framework that generates simulation-ready indoor environments from natural language prompts.
3. 机制：SceneSmith constructs scenes through successive stages—from architectural layout to furniture placement to small object population—each implemented as an interaction among VLM agents…
4. 结果：We further demonstrate that these environments can be used in an end-to-end pipeline for automatic robot policy evaluation.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[SceneSmith: Agentic Generation of Simulation-Ready Indoor Scenes](https://openreview.net/forum?id=WwS8CTpUA6)

## 368. [Spotlight] Score-Repellent Monte Carlo: Toward Efficient Non-Markovian Sampler with Constant Memory in General State Spaces

1. 问题：History-dependent sampling can reduce long-run Monte Carlo variance by discouraging redundant revisits, but existing schemes typically encode history through empirical measure on…
2. 方法：提出/研究 ***Score-Repellent Monte Carlo* (SRMC) framework that summarizes traject**；We propose *Score-Repellent Monte Carlo* (SRMC) framework that summarizes trajectory history by a running average of score evaluations in R^d…
3. 机制：History-dependent sampling can reduce long-run Monte Carlo variance by discouraging redundant revisits, but existing schemes typically encode history through empirical measure on…
4. 结果：Experiments on continuous targets and discrete energy-based models demonstrate improved estimator variance and mode coverage, while retaining O(d) memory usage and modest…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Score-Repellent Monte Carlo: Toward Efficient Non-Markovian Sampler with Constant Memory in General State Spaces](https://openreview.net/forum?id=PN8EiOzMuT)

## 369. [Oral] Second-Order Smooth Planning with Optimal-Transport Bellman Smoothing

1. 问题：SmoothCruiser achieves problem-independent complexity O( ^-4) by exploiting the smoothness of the entropy-regularized Bellman backup, but its estimator is only first-order.
2. 方法：提出/研究 **Second-Order Smooth Planning with Optimal-Transport Bellman Smoothing**；SmoothCruiser achieves problem-independent complexity O( ^-4) by exploiting the smoothness of the entropy-regularized Bellman backup, but its estimator is only…
3. 机制：The resulting SecondOrderSmoothCruiser achieves O( ^-3) oracle complexity for fixed OT parameters, and we relate the OT, entropy-regularized, and unregularized objectives through…
4. 结果：The resulting SecondOrderSmoothCruiser achieves O( ^-3) oracle complexity for fixed OT parameters, and we relate the OT, entropy-regularized, and unregularized objectives through…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Second-Order Smooth Planning with Optimal-Transport Bellman Smoothing](https://openreview.net/forum?id=LrNH0O3s45)

## 370. [Spotlight] Securing Multimodal AI through Internal Information Decomposition

1. 问题：Multimodal large language models introduce attack surfaces absent in unimodal systems: adversaries can distribute malicious intent across modalities to evade unimodal safeguards.
2. 方法：提出/研究 **FlowGuard**；We propose FlowGuard, a lightweight inference-time framework that detects harmful inputs by monitoring internal multimodal consistency.
3. 机制：We propose FlowGuard, a lightweight inference-time framework that detects harmful inputs by monitoring internal multimodal consistency.
4. 结果：Our results demonstrate that monitoring cross-modal consistency offers an efficient and effective defense for multimodal reasoning.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Securing Multimodal AI through Internal Information Decomposition](https://openreview.net/forum?id=GEzZIUmEqE)

## 371. [Spotlight] Security—Fidelity Tradeoffs: The Hidden Cost of Prompt Injection Defense

1. 问题：We identify a **security—fidelity tradeoff** in defending LLMs against indirect prompt injection: defenses resist injected instructions largely by suppressing untrusted text, which…
2. 方法：提出/研究 ****SecFid****；We introduce **SecFid**, a benchmark built so that *executing* an injection, *processing* it as data, and *ignoring* it produce distinguishable…
3. 机制：We introduce **SecFid**, a benchmark built so that *executing* an injection, *processing* it as data, and *ignoring* it produce distinguishable outputs.
4. 结果：The highest-fidelity model reaches 96.5% fidelity at 47.8% security, while the most secure defenses invert this, at 99.3% security but only 71.0%—73.9%…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Security—Fidelity Tradeoffs: The Hidden Cost of Prompt Injection Defense](https://openreview.net/forum?id=vTJmIhNvC3)

## 372. [Spotlight] Seizure-Semiology-Suite(S^3): A Clinically Multimodal Dataset, Benchmark, and Models for Seizure Semiology Understanding

1. 问题：While Multimodal Large Language Models (MLLMs) have demonstrated remarkable proficiency in general video understanding, their capacity to interpret involuntary, and spatio-temporally evolving…
2. 方法：提出/研究 **Seizure-Semiology-Suite (S³)**；To address this gap, we introduce Seizure-Semiology-Suite (S³), a clinically grounded dataset and benchmark for fine-grained, structured seizure semiology understanding.
3. 机制：To address this gap, we introduce Seizure-Semiology-Suite (S³), a clinically grounded dataset and benchmark for fine-grained, structured seizure semiology understanding.
4. 结果：Seizure-Semiology-Suite establishes a rigorous benchmark for evaluating multimodal models in safety-critical medical video understanding and guides the development of clinically reliable, domain-adaptive…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Seizure-Semiology-Suite(S^3): A Clinically Multimodal Dataset, Benchmark, and Models for Seizure Semiology Understanding](https://openreview.net/forum?id=MyorUlHKVc)

## 373. [Spotlight] Self-Distillation Enables Continual Learning

1. 问题：Continual learning, enabling models to acquire new skills and knowledge without degrading existing capabilities, remains a fundamental challenge for foundation models.
2. 方法：提出/研究 **Self-Distillation Fine-Tuning (SDFT)**；We introduce Self-Distillation Fine-Tuning (SDFT), a simple method that enables on-policy learning directly from demonstrations.
3. 机制：We introduce Self-Distillation Fine-Tuning (SDFT), a simple method that enables on-policy learning directly from demonstrations.
4. 结果：In sequential learning experiments, SDFT enables a single model to accumulate multiple skills over time without performance regression, establishing on-policy distillation as…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Self-Distillation Enables Continual Learning](https://openreview.net/forum?id=qA6FgH0nnZ)

## 374. [Spotlight] Self-Soupervision: Cooking Model Soups without Labels

1. 问题：Model soups are strange and strangely effective combinations of parameters.
2. 方法：提出/研究 **Self-Soupervision**；They take a model (the stock), fine-tune it into multiple models (the ingredients), and then mix their parameters back into…
3. 机制：They take a model (the stock), fine-tune it into multiple models (the ingredients), and then mix their parameters back into one model…
4. 结果：We show that Self-Souping on corrupted test data, then fine-tuning back on uncorrupted train data, boosts robustness by +3.5% (ImageNet-C)…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Self-Soupervision: Cooking Model Soups without Labels](https://openreview.net/forum?id=z0UM7y0L4r)

## 375. [Spotlight] Shared Semantics, Divergent Mechanisms: Unsupervised Feature Discovery by Aligning Semantics and Mechanisms

1. 问题：As large language models are increasingly deployed in high-stakes settings, there is a growing need for tools that audit not only model…
2. 方法：提出/研究 **distribution-level unsupervised feature discovery**；We introduce distribution-level unsupervised feature discovery, which clusters sampled continuations using both semantic content and sequence-level mechanistic attributions, without manually…
3. 机制：We introduce distribution-level unsupervised feature discovery, which clusters sampled continuations using both semantic content and sequence-level mechanistic attributions, without manually specifying target…
4. 理论/证据：Our method represents each continuation with a semantic embedding and a prefix-to-continuation attribution signature, then optimizes a rate-distortion objective that…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Shared Semantics, Divergent Mechanisms: Unsupervised Feature Discovery by Aligning Semantics and Mechanisms](https://openreview.net/forum?id=C9AhjL8aUZ)

## 376. [Spotlight] Sharp Inequalities between Total Variation and Hellinger Distances for Gaussian Mixtures

1. 问题：Taken together, our results resolve an open problem raised in Jia et al.
2. 方法：提出/研究 **Sharp Inequalities between Total Variation and Hellinger Distances…**；Our first result establishes a general upper bound: for any two mixing distributions supported on a compact set, the Hellinger…
3. 机制：Our first result establishes a general upper bound: for any two mixing distributions supported on a compact set, the Hellinger distance between…
4. 理论/证据：Our first result establishes a general upper bound: for any two mixing distributions supported on a compact set, the Hellinger…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Sharp Inequalities between Total Variation and Hellinger Distances for Gaussian Mixtures](https://openreview.net/forum?id=ihMB4kA2SQ)

## 377. [Spotlight] Simple Algorithms for Bad Triangle Transversals with Applications to Correlation Clustering

1. 问题：The Bad Triangle Transversal (BTT) problem asks for the smallest set of edges that need to be removed from a given signed…
2. 方法：提出/研究 **Simple Algorithms for Bad Triangle Transversals with Applications…**；Here, a bad triangle is a triangle with exactly one negative edge.
3. 机制：Here, a bad triangle is a triangle with exactly one negative edge.
4. 理论/证据：On the hardness side, we show that BTT is NP-hard to approximate with factor better than 21372136 on complete graphs.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[Simple Algorithms for Bad Triangle Transversals with Applications to Correlation Clustering](https://openreview.net/forum?id=Yq66fTPjHn)

## 378. [Oral] Simultaneous Speech-to-Speech Translation Without Aligned Data

1. 问题：Traditional approaches rely on supervised training with word-level aligned data, which is difficult to collect at scale and thus depends on synthetic…
2. 方法：提出/研究 **Hibiki-Zero**；We propose Hibiki-Zero, which eliminates the need for word-level alignments entirely.
3. 机制：We propose Hibiki-Zero, which eliminates the need for word-level alignments entirely.
4. 结果：We provide [examples]( [model weights]( [inference code]( and we release a [benchmark]( containing 45h of multilingual data for speech translation evaluation.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Simultaneous Speech-to-Speech Translation Without Aligned Data](https://openreview.net/forum?id=76XSBLdBdg)

## 379. [Spotlight] Single-Head Attention in High Dimensions: A Theory of Generalization, Weights Spectra, and Scaling Laws

1. 问题：Trained attention layers exhibit striking and reproducible spectral structure of the weights, including low-rank collapse, bulk deformation, and isolated spectral outliers, yet…
2. 方法：提出/研究 **Single-Head Attention in High Dimensions**；We study empirical risk minimization in a single-head tied-attention layer trained on synthetic high-dimensional sequence tasks generated from the attention-indexed…
3. 机制：Finally, for targets with power-law spectra, we show that learning proceeds through sequential spectral recovery, leading to the emergence of power-law scaling…
4. 结果：Finally, for targets with power-law spectra, we show that learning proceeds through sequential spectral recovery, leading to the emergence of…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Single-Head Attention in High Dimensions: A Theory of Generalization, Weights Spectra, and Scaling Laws](https://openreview.net/forum?id=3qan4Zg9rA)

## 380. [Spotlight] Skill Neologisms: Towards Skill-based Continual Learning

1. 问题：However, extending model capabilities to new skills in a scalable manner is an open problem: fine-tuning and parameter-efficient variants risk catastrophic forgetting…
2. 方法：提出/研究 **Skill Neologisms**；However, extending model capabilities to new skills in a scalable manner is an open problem: fine-tuning and parameter-efficient variants risk…
3. 机制：However, extending model capabilities to new skills in a scalable manner is an open problem: fine-tuning and parameter-efficient variants risk catastrophic forgetting…
4. 理论/证据：We explore *skill neologisms*—soft tokens integrated in the model's vocabulary and optimized to improve capabilities over a specific skill—as a…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Skill Neologisms: Towards Skill-based Continual Learning](https://openreview.net/forum?id=5VgZUEpK6W)

## 381. [Spotlight] Skill-Pro: Learning Reusable Skills from Experience via Non-Parametric PPO for LLM Agents

1. 问题：LLM-driven agents excel at sequential decision-making but often rely on on-the-fly reasoning, re-deriving solutions even in recurring scenarios.
2. 方法：提出/研究 ****Skill-Pro****；To bridge this gap, we propose **Skill-Pro**, a framework enabling agents to autonomously learn reusable procedural skills from interaction experiences…
3. 机制：Through score-based maintenance, Skill-Pro sustains compact, high-quality procedural memory.
4. 结果：Experimental results across in-domain, cross-task, and cross-agent scenarios demonstrate that Skill-Pro achieves superior reuse rates and significant gains with extreme memory compression.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Skill-Pro: Learning Reusable Skills from Experience via Non-Parametric PPO for LLM Agents](https://openreview.net/forum?id=9kJQjx2B80)

## 382. [Oral] Skip a Layer or Loop It? Learning Program-of-Layers in LLMs

1. 问题：Large language models (LLMs) perform inference by following a fixed depth and order, non-recurrent execution of all layers.
2. 方法：提出/研究 **lightweight PoLar prediction network**；To efficiently achieve PoLar in practice, we propose a lightweight PoLar prediction network, which learns to generate execution programs that…
3. 机制：To efficiently achieve PoLar in practice, we propose a lightweight PoLar prediction network, which learns to generate execution programs that dynamically skip…
4. 理论/证据：Experiments on mathematical reasoning benchmarks demonstrate that PoLar consistently improves accuracy over standard inference and prior dynamic-depth methods, often while…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Skip a Layer or Loop It? Learning Program-of-Layers in LLMs](https://openreview.net/forum?id=pl10b6EQAN)

## 383. [Spotlight] SlaClip: Gradient Norm Slacks can be Indicator for Adaptive Clipping in DP-SGD

1. 问题：In contrast, we leverage the *slack* information induced by the standard clipping operation, an overlooked signal in prior work, and show that…
2. 方法：提出/研究 ***SlaClip***；In light of this, we propose *SlaClip*, a privacy-preserving adaptive clipping strategy using a post-hoc *Slack Indicator*.
3. 机制：In light of this, we propose *SlaClip*, a privacy-preserving adaptive clipping strategy using a post-hoc *Slack Indicator*.
4. 结果：Across diverse datasets and tasks, experiments show that *SlaClip* consistently outperforms baseline adaptive clipping methods.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[SlaClip: Gradient Norm Slacks can be Indicator for Adaptive Clipping in DP-SGD](https://openreview.net/forum?id=48suUeYKdb)

## 384. [Spotlight] SleepLM: Natural-Language Intelligence for Human Sleep

1. 问题：Despite the critical role of sleep, learning-based sleep analysis systems operate in closed label spaces (e.g., predefined stages or events) and fail…
2. 方法：提出/研究 **SleepLM**；We present SleepLM, a family of sleep-language foundation models that enable human sleep alignment, interpretation, and interaction with natural language.
3. 机制：Furthermore, we present a unified pretraining objective that combines contrastive alignment, caption generation, and signal reconstruction to better capture physiological fidelity and…
4. 结果：Extensive experiments on real-world sleep understanding tasks verify that SleepLM outperforms state-of-the-art in zero-shot and few-shot learning, cross-modal retrieval, and sleep captioning.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[SleepLM: Natural-Language Intelligence for Human Sleep](https://openreview.net/forum?id=9wpwfSJCp9)

## 385. [Spotlight] SmoothSpike: Spiking Transformer with Learnable Hadamard Transformation

1. 问题：However, their discrete information representation fundamentally limits expressiveness, resulting in a notable performance gap relative to Artificial Neural Networks (ANNs) on language…
2. 方法：提出/研究 **SmoothSpike**；To address this, we propose SmoothSpike, which applies a randomized Hadamard transformation to smooth pre-activation inputs and theoretically proves that…
3. 机制：To further improve adaptability across varying input distributions, we extend the fixed transformation within SmoothSpike to a learnable orthogonal matrix updated via…
4. 理论/证据：In this paper, we reveal that this gap is fundamentally rooted in a spike saturation-induced information homogenization problem: within a…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[SmoothSpike: Spiking Transformer with Learnable Hadamard Transformation](https://openreview.net/forum?id=UoUKCLHjRa)

## 386. [Oral] SoftJAX & SoftTorch: Empowering Automatic Differentiation Libraries with Informative Gradients

1. 问题：While numerous ''soft'' relaxations have been proposed that provide informative gradients, the respective implementations are fragmented across projects, making them difficult to…
2. 方法：提出/研究 **SoftJAX & SoftTorch**；Yet, many ''hard'' primitives in these libraries such as thresholding, Boolean logic, discrete indexing, and sorting operations yield zero or…
3. 机制：This includes (i) elementwise operators such as *clip* or *abs*, (ii) utility methods for manipulating Booleans and indices via fuzzy logic, (iii)…
4. 结果：Overall, SoftJAX and SoftTorch make the toolbox of soft relaxations easily accessible to differentiable programming, as demonstrated through benchmarking and a practical…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[SoftJAX & SoftTorch: Empowering Automatic Differentiation Libraries with Informative Gradients](https://openreview.net/forum?id=RKHDV40omz)

## 387. [Oral] Solving Time-Dependent Differential Equations with Physical Dynamical Systems

1. 问题：Most existing TDDE solvers are limited by time discretization, forcing a latency-accuracy trade-off where smaller step sizes capture high-fidelity trajectories but incur…
2. 方法：提出/研究 **Solving Time-Dependent Differential Equations with Physical Dynamical Systems**；Most existing TDDE solvers are limited by time discretization, forcing a latency-accuracy trade-off where smaller step sizes capture high-fidelity trajectories…
3. 机制：Dynamical System Machines (DSMs) offer a promising alternative by computing through continuous physical evolution, yet existing DSMs struggle to capture the spatiotemporal…
4. 结果：Experiments demonstrate that DS-TS achieves high-fidelity solutions while delivering orders-of-magnitude improvements in speed ( 10^3 ) and energy efficiency ( 10^5 )…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Solving Time-Dependent Differential Equations with Physical Dynamical Systems](https://openreview.net/forum?id=0YHSZPkMp8)

## 388. [Oral] SpatioLM: Towards General Physical Spatial Intelligence in Vision-Language Models

1. 问题：Vision-Language Models (VLMs) perform well on commonsense reasoning tasks but struggle with visual spatial reasoning.
2. 方法：提出/研究 **parameter-efficient Spatio-vision Language Models (SpatioLM)**；To this end, we propose a parameter-efficient Spatio-vision Language Models (SpatioLM), that enhances spatial intelligence without extra 3D prior inputs…
3. 机制：To this end, we propose a parameter-efficient Spatio-vision Language Models (SpatioLM), that enhances spatial intelligence without extra 3D prior inputs or third-party…
4. 结果：Notably, the model achieves an impressive score of 71.6 on the VSI-Bench (the first model to surpass 70).
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[SpatioLM: Towards General Physical Spatial Intelligence in Vision-Language Models](https://openreview.net/forum?id=CHavqrN1X9)

## 389. [Spotlight] Spectral-Informed Neural Networks Outperform Spectral methods in High-dimensional PDEs

1. 问题：For low-dimensional problems (d 3), spectral methods can achieve exceptionally high accuracy.
2. 方法：提出/研究 **Modified SINNs**；In this work, we introduce Modified SINNs, which integrate coefficient decay scaling and basis embeddings motivated by harmonic analysis to…
3. 机制：For middle-dimensional problems (4 d 10), spectral methods remain feasible through specific techniques such as sparse grids or hyperbolic cross.
4. 结果：Numerical experiments on steady and time-dependent partial differential equations demonstrate that Modified SINNs outperform sparse grid spectral methods on middle-dimensional problems with…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Spectral-Informed Neural Networks Outperform Spectral methods in High-dimensional PDEs](https://openreview.net/forum?id=KAHCMPsPeI)

## 390. [Spotlight] SplAttN: Bridging 2D and 3D with Gaussian Soft Splatting and Attention for Point Cloud Completion

1. 问题：Although multi-modal learning has advanced point cloud completion, the theoretical mechanisms remain unclear.
2. 方法：提出/研究 **SplAttN**；To address this practical limitation, we propose SplAttN, which replaces hard projection with Differentiable Gaussian Splatting to produce a dense…
3. 机制：To address this practical limitation, we propose SplAttN, which replaces hard projection with Differentiable Gaussian Splatting to produce a dense, continuous image-plane…
4. 结果：Crucially, we utilize the real-world KITTI benchmark as a stress test for multi-modal reliance.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[SplAttN: Bridging 2D and 3D with Gaussian Soft Splatting and Attention for Point Cloud Completion](https://openreview.net/forum?id=vTp9JToZl9)

## 391. [Oral] Stabilizing the Q-Gradient Field for Policy Smoothness in Actor-Critic Methods

1. 问题：Policies learned via continuous actor-critic methods often exhibit erratic, high-frequency oscillations, making them unsuitable for physical deployment.
2. 方法：提出/研究 **PAVE**；To empirically validate this theoretical insight, we introduce PAVE (Policy-Aware Value-field Equalization), a critic-centric regularization framework that treats the critic…
3. 机制：Policies learned via continuous actor-critic methods often exhibit erratic, high-frequency oscillations, making them unsuitable for physical deployment.
4. 结果：Experimental results demonstrate that PAVE achieves smoothness comparable to policy-side smoothness regularization methods, while maintaining competitive task performance, without modifying the actor.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Stabilizing the Q-Gradient Field for Policy Smoothness in Actor-Critic Methods](https://openreview.net/forum?id=UpA00uD6Ek)

## 392. [Spotlight] Stable Deep Reinforcement Learning via Isotropic Gaussian Representations

1. 问题：Deep reinforcement learning systems often suffer from unstable training dynamics due to non-stationarity, where learning objectives and data distributions evolve over time.
2. 方法：提出/研究 **use of Sketched Isotropic Gaussian Regularization for shaping represen**；Building on this insight, we propose the use of Sketched Isotropic Gaussian Regularization for shaping representations toward an isotropic Gaussian…
3. 机制：Building on this insight, we propose the use of Sketched Isotropic Gaussian Regularization for shaping representations toward an isotropic Gaussian distribution during…
4. 结果：We demonstrate empirically, over a variety of domains, that this simple and computationally inexpensive method improves performance under non-stationarity while reducing representation…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Stable Deep Reinforcement Learning via Isotropic Gaussian Representations](https://openreview.net/forum?id=gc7Gg18ejz)

## 393. [Spotlight] Stable-GFlowNet: Toward Diverse and Robust LLM Red-Teaming via Contrastive Trajectory Balance

1. 问题：Large Language Model Red-Teaming, which proactively identifies vulnerabilities of large language models, is an essential process for ensuring safety.
2. 方法：提出/研究 **Stable-GFN (S-GFN)**；We propose Stable-GFN (S-GFN), which eliminates Z estimation in GFN and reduces training instability.
3. 机制：S-GFN avoids Z-estimation through pairwise comparisons and employs a robust masking methodology against noisy rewards.
4. 结果：We demonstrate the overwhelming attack performance and diversity of S-GFN across various settings.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Stable-GFlowNet: Toward Diverse and Robust LLM Red-Teaming via Contrastive Trajectory Balance](https://openreview.net/forum?id=OyPE1ganBR)

## 394. [Spotlight] STAR-KV: Low-Rank KV Cache Compression via Soft Thresholding for Adaptive Rank Control

1. 问题：However, prior methods rely on fixed or heuristic rank selection and struggle to achieve aggressive compression with minimal accuracy degradation.
2. 方法：提出/研究 **STAR-KV**；We propose STAR-KV, an adaptive low-rank KV cache compression framework with fine-grained rank control.
3. 机制：We propose STAR-KV, an adaptive low-rank KV cache compression framework with fine-grained rank control.
4. 结果：Evaluated across multiple LLMs and benchmarks, STAR-KV achieves up to 75\% KV cache compression and up to 20 overall KV cache reduction…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[STAR-KV: Low-Rank KV Cache Compression via Soft Thresholding for Adaptive Rank Control](https://openreview.net/forum?id=lJjH1q6RwY)

## 395. [Spotlight] Steer Like the LLM: Activation Steering that Mimics Prompting

1. 问题：Large language models can be steered at inference time through prompting or activation interventions, but activation steering methods often underperform compared to…
2. 方法：提出/研究 ***Prompt Steering Replacement (PSR)* models**；To this end, we introduce *Prompt Steering Replacement (PSR)* models, a new family of activation steering methods that distill prompt…
3. 机制：Large language models can be steered at inference time through prompting or activation interventions, but activation steering methods often underperform compared to…
4. 结果：Experiments on persona steering and instruction following across multiple language models demonstrate that PSR models consistently outperform constant-coefficient interventions that…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Steer Like the LLM: Activation Steering that Mimics Prompting](https://openreview.net/forum?id=06Nk3dJDMq)

## 396. [Spotlight] Stop When Further Reasoning Won’t Help: Attention-State Adaptive Generation in Reasoning Models

1. 问题：By incorporating test-time compute scaling, large reasoning models (LRMs) can solve complex problems through explicit chain-of-thought (CoT) reasoning processes.
2. 方法：提出/研究 **Stop When Further Reasoning Won’t Help**；However, they often suffer from overthinking, resulting in redundant token outputs and degraded accuracy.
3. 机制：By incorporating test-time compute scaling, large reasoning models (LRMs) can solve complex problems through explicit chain-of-thought (CoT) reasoning processes.
4. 结果：Specifically, ASAG improves average accuracy by 3.2% while reducing the number of generated tokens by nearly 40% across all reasoning tasks on…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Stop When Further Reasoning Won’t Help: Attention-State Adaptive Generation in Reasoning Models](https://openreview.net/forum?id=zRMK32N6t6)

## 397. [Oral] Strategic Navigation or Stochastic Search? How Agents and Humans Reason Over Document Collections

1. 问题：Yet, a critical question remains: do these agents demonstrate genuine strategic reasoning, or merely stochastic trial-and-error search?
2. 方法：提出/研究 **MADQA**；To address this, we introduce MADQA, a benchmark of 2,250 human-authored questions grounded in 800 heterogeneous PDF documents.
3. 机制：To address this, we introduce MADQA, a benchmark of 2,250 human-authored questions grounded in 800 heterogeneous PDF documents.
4. 结果：They fail to close the nearly 20\% gap to oracle performance, persisting in unproductive loops.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Strategic Navigation or Stochastic Search? How Agents and Humans Reason Over Document Collections](https://openreview.net/forum?id=ds3ZOevkwx)

## 398. [Spotlight] Suppress and Diversify: Refining Robust Pathways for Corruption Robustness

1. 问题：Model robustness against natural image corruptions is essential for safety-critical applications.
2. 方法：提出/研究 **Suppress and Diversify (S\&D)**；While existing methods primarily focus on implicit representation learning, we provide the first systematic exploration of computational pathways to explicitly…
3. 机制：To exploit these insights, we propose Suppress and Diversify (S\&D), a non-intrusive refinement approach that enhances robustness by dynamically selecting robust pathways…
4. 结果：Extensive evaluations across eight benchmarks demonstrate that S\&D consistently improves performance across multiple vision tasks, diverse backbones, and complex real-world scenarios, highlighting…
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Suppress and Diversify: Refining Robust Pathways for Corruption Robustness](https://openreview.net/forum?id=Tam54Owz7G)

## 399. [Spotlight] Surgery: Mitigating Harmful Fine-Tuning for Large Language Models via Attention Sink

1. 问题：Harmful fine-tuning can invalidate safety alignment of large language models, exposing significant safety risks.
2. 方法：提出/研究 **separable sink divergence hypothesis — attention heads associating wit**；Based on this finding, we propose a separable sink divergence hypothesis — attention heads associating with learning harmful patterns during…
3. 机制：Based on this finding, we propose a separable sink divergence hypothesis — attention heads associating with learning harmful patterns during fine-tuning are…
4. 结果：Extensive experiments demonstrate that Surgery improves defense performance by 5.90\%, 11.25\%, and 9.55\% on the BeaverTails, HarmBench, and SorryBench benchmarks, respectively.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Surgery: Mitigating Harmful Fine-Tuning for Large Language Models via Attention Sink](https://openreview.net/forum?id=6ojsIliNF0)

## 400. [Spotlight] SurvDiff: A Diffusion Model for Generating Synthetic Data in Survival Analysis

1. 问题：This poses unique challenges for synthetic data generation, where it is crucial for clinical research to faithfully reproduce both the event-time distribution…
2. 方法：提出/研究 **SurvDiff**；In this paper, we propose SurvDiff, an end-to-end diffusion model specifically designed for generating synthetic data in survival analysis.
3. 机制：SurvDiff is tailored to capture the data-generating mechanism by jointly generating mixed-type covariates, event times, and right-censoring, guided by a survival-tailored loss…
4. 结果：Across multiple datasets, we show that SurvDiff outperforms state-of-the-art generative baselines in both distributional fidelity and survival model evaluation metrics…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[SurvDiff: A Diffusion Model for Generating Synthetic Data in Survival Analysis](https://openreview.net/forum?id=boeY2syj2r)

## 401. [Spotlight] SVD as a Fast Interpretability Method for Transformers

1. 问题：Mechanistic interpretability of Transformer models commonly relies on training auxiliary proxy models, such as Sparse Autoencoders or Cross-Layer Transcoders.
2. 方法：提出/研究 **n alternative**；We propose an alternative, training-free interpretability framework that directly exploits the Singular Value Decomposition (SVD) of weight matrices in Transformer…
3. 机制：We propose an alternative, training-free interpretability framework that directly exploits the Singular Value Decomposition (SVD) of weight matrices in Transformer MLP sublayers.
4. 理论/证据：We show that the projection matrices of MLP sublayers admit a natural decomposition into orthogonal, interpretable rank-1 subspaces, which we…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[SVD as a Fast Interpretability Method for Transformers](https://openreview.net/forum?id=7tt8TwMjdJ)

## 402. [Spotlight] SVL: Empowering Spiking Neural Networks for Efficient 3D Open-World Understanding

1. 问题：Spiking Neural Networks (SNNs) offer an energy—efficient route to 3D spatio—temporal perception, yet they lag behind Artificial Neural Networks (ANNs) due to…
2. 方法：提出/研究 **universal Spike—based Vision—Language pretraining framework (SVL) that**；We present a universal Spike—based Vision—Language pretraining framework (SVL) that equips SNNs with open—world 3D understanding while preserving end—to—end spike…
3. 机制：SVL comprises two core components: (i) Multi—scale Triple Alignment (MTA), a label—free triplet contrastive objective aligning 3D, image, and text; and (ii)…
4. 结果：Extensive experiments show that SVL attains strong zero—shot 3D classification (85.4% top—1) and consistently outperforms prior SNNs on downstream tasks (e.g., +6.1%…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[SVL: Empowering Spiking Neural Networks for Efficient 3D Open-World Understanding](https://openreview.net/forum?id=Ai3a79cTvr)

## 403. [Oral] SVRG and Beyond via Posterior Correction

1. 问题：Stochastic Variance Reduced Gradient (SVRG) and its variants aim to speed-up training by using gradient corrections.
2. 方法：提出/研究 **SVRG and Beyond via Posterior Correction**；Originally proposed over a decade ago, these methods have never been connected to any Bayesian method at a fundamental level.
3. 机制：Originally proposed over a decade ago, these methods have never been connected to any Bayesian method at a fundamental level.
4. 理论/证据：Here, we fill this gap and derive surprising new connections of SVRG to a recently proposed Bayesian method called `posterior…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[SVRG and Beyond via Posterior Correction](https://openreview.net/forum?id=3NQSeJOfkz)

## 404. [Spotlight] SWING: Unlocking Implicit Graph Representations for Graph Random Features

1. 问题：We propose SWING: Space Walks for Implicit Network Graphs, a new class of algorithms for computations involving Graph Random Features on graphs…
2. 方法：提出/研究 **SWING**；We propose SWING: Space Walks for Implicit Network Graphs, a new class of algorithms for computations involving Graph Random Features…
3. 机制：To accurately and efficiently approximate original combinatorial calculations, SWING applies customized Gumbel-softmax sampling mechanism with linearized kernels, obtained via random features coupled…
4. 结果：We provide detailed analysis of SWING and complement it with thorough experiments on different classes of i-graphs.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[SWING: Unlocking Implicit Graph Representations for Graph Random Features](https://openreview.net/forum?id=LBcnybFVBp)

## 405. [Spotlight] Sycophancy Towards Researchers Drives Performative Misalignment

1. 问题：The increasing situational awareness of language models raises safety concerns: models might be aware when they are evaluated, and adjust their behavior…
2. 方法：提出/研究 **three empirical findings**；To examine this hypothesis, we present three empirical findings.
3. 机制：To examine this hypothesis, we present three empirical findings.
4. 理论/证据：First, we show that evaluation awareness persists even when we tell models they are deployed, which contradicts the scheming story…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Sycophancy Towards Researchers Drives Performative Misalignment](https://openreview.net/forum?id=rLFIOikFR2)

## 406. [Spotlight] Symmetries in language statistics shape the geometry of model representations

1. 问题：Although learned representations underlie neural networks' success, their fundamental properties remain poorly understood.
2. 方法：提出/研究 **Symmetries in language statistics shape the geometry of…**；A striking example is the emergence of simple geometric structures in LLM representations: for example, calendar months organize into a…
3. 机制：A striking example is the emergence of simple geometric structures in LLM representations: for example, calendar months organize into a circle, years…
4. 理论/证据：We show that the statistics of language exhibit a translation symmetry—e.g,. the co-occurrence probability of two months depends only on…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Symmetries in language statistics shape the geometry of model representations](https://openreview.net/forum?id=XQeMPEkfdd)

## 407. [Spotlight] Symmetry Reveals Layerwise Dynamics: How Transformers Perform In-Context Classification

1. 问题：Transformers can perform in-context classification from a few labeled examples, yet the inference-time algorithm remains opaque.
2. 方法：提出/研究 **Symmetry Reveals Layerwise Dynamics**；We study multi-class linear classification in the hard no-margin regime and make the computation identifiable by enforcing feature- and label-permutation…
3. 机制：We study multi-class linear classification in the hard no-margin regime and make the computation identifiable by enforcing feature- and label-permutation equivariance at…
4. 理论/证据：We study multi-class linear classification in the hard no-margin regime and make the computation identifiable by enforcing feature- and label-permutation…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Symmetry Reveals Layerwise Dynamics: How Transformers Perform In-Context Classification](https://openreview.net/forum?id=fDMizWsNoG)

## 408. [Spotlight] T^2PO: Uncertainty-Guided Exploration Control for Stable Multi-Turn Agentic Reinforcement Learning

1. 问题：Despite advances in stabilization techniques such as fine-grained credit assignment and trajectory filtering, instability remains pervasive and often leads to training collapse.
2. 方法：提出/研究 **Token- and Turn-level Policy Optimization (T^2PO)**；To address this issue, we propose Token- and Turn-level Policy Optimization (T^2PO), an uncertainty-aware framework that explicitly controls exploration at…
3. 机制：To address this issue, we propose Token- and Turn-level Policy Optimization (T^2PO), an uncertainty-aware framework that explicitly controls exploration at fine-grained levels.
4. 结果：We evaluate T^2PO in diverse environments, including WebShop, ALFWorld, and Search QA, demonstrating substantial gains in training stability and performance improvements with…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[T^2PO: Uncertainty-Guided Exploration Control for Stable Multi-Turn Agentic Reinforcement Learning](https://openreview.net/forum?id=aD1zjvdJN4)

## 409. [Spotlight] TabSwift: An Efficient Tabular Foundation Model with Row-Wise Attention

1. 问题：However, recent tabular foundation models often improve accuracy with increasingly complex architectures, incurring higher inference cost and limiting practical deployment.
2. 方法：提出/研究 **TabSwift**；They have demonstrated competitive performance, particularly on small-to-medium datasets.
3. 机制：Tabular foundation models, exemplified by TabPFN, perform prediction via in-context learning, inferring test labels directly from labeled training examples.
4. 理论/证据：However, recent tabular foundation models often improve accuracy with increasingly complex architectures, incurring higher inference cost and limiting practical deployment.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[TabSwift: An Efficient Tabular Foundation Model with Row-Wise Attention](https://openreview.net/forum?id=ottLtChHp2)

## 410. [Spotlight] TD3B: Transition-Directed Discrete Diffusion for Allosteric Binder Generation

1. 问题：Protein function is often controlled by ligands that bias the direction of state transitions, such as agonists and antagonists, rather than stabilizing…
2. 方法：提出/研究 ****T**ransition-**D**irected **D**iscrete **D**iffusion for allosteric***；To address this gap, we introduce **T**ransition-**D**irected **D**iscrete **D**iffusion for allosteric**B**inder design (**TD3B**), a sequence-based generative framework that designs binders…
3. 机制：TD3B combines a target-aware Direction Oracle, a soft binding-affinity gate, and amortized fine-tuning of a pre-trained discrete diffusion model, enabling targeted agonist…
4. 理论/证据：Structure-based design methods optimize binding to static conformations and cannot represent non-reversible, directional effects or systematically distinguish agonist from antagonist…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[TD3B: Transition-Directed Discrete Diffusion for Allosteric Binder Generation](https://openreview.net/forum?id=RNuC8Nj6rD)

## 411. [Spotlight] Teaching Models to Teach Themselves: Reasoning at the Edge of Learnability

1. 问题：We investigate a fundamental question:Can a pretrained LLM leverage latent knowledge to generate an automated curriculum for problems it cannot solve?
2. 方法：提出/研究 **Teaching Models to Teach Themselves**；We investigate a fundamental question:Can a pretrained LLM leverage latent knowledge to generate an automated curriculum for problems it cannot…
3. 机制：We investigate a fundamental question:Can a pretrained LLM leverage latent knowledge to generate an automated curriculum for problems it cannot solve?
4. 理论/证据：We explore this with SOAR: An asymmetric self-play framework that uses meta-RL to surface these pedagogical signals.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Teaching Models to Teach Themselves: Reasoning at the Edge of Learnability](https://openreview.net/forum?id=GnqHK8Ww98)

## 412. [Spotlight] TetraJet-v2: Accurate NVFP4 Training for Large Language Models with Oscillation Suppression and Outlier Control

1. 问题：While novel 4-bit formats like NVFP4 offer substantial efficiency gains, achieving near-lossless training at such low precision remains challenging.
2. 方法：提出/研究 ****TetraJet-v2****；We introduce **TetraJet-v2**, an end-to-end 4-bit FQT method that leverages NVFP4 for activations, weights and gradients in all linear layers.
3. 机制：We introduce **TetraJet-v2**, an end-to-end 4-bit FQT method that leverages NVFP4 for activations, weights and gradients in all linear layers.
4. 结果：To address these, we propose: 1) an unbiased double-block quantization method for NVFP4 linear layers, 2) **OsciReset**, an algorithm to suppress weight…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[TetraJet-v2: Accurate NVFP4 Training for Large Language Models with Oscillation Suppression and Outlier Control](https://openreview.net/forum?id=7ZQhm5HnOA)

## 413. [Oral] TG-RAG: A Retrieval-Augmented Framework for Reasoning Guidance in Specialized Domains

1. 问题：Enhancing Large Reasoning Models (LRMs) for specialized domains remains a critical challenge.
2. 方法：提出/研究 **Thought Guidance-Retrieval Augmented Generation (TG-RAG)**；While recent industrial frameworks attempt to encapsulate Standard Operating Procedures into modular "skills" for dynamic retrieval, utilizing them via context…
3. 机制：While recent industrial frameworks attempt to encapsulate Standard Operating Procedures into modular "skills" for dynamic retrieval, utilizing them via context engineering often…
4. 结果：Extensive evaluations show that TG-RAG achieves competitive performance, demonstrating advantages in specialized domains by ensuring faithful adherence to domain SOPs.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[TG-RAG: A Retrieval-Augmented Framework for Reasoning Guidance in Specialized Domains](https://openreview.net/forum?id=W34UyCRQel)

## 414. [Spotlight] The Assistant Axis: Situating and Stabilizing the Default Persona of Language Models

1. 问题：Large language models can represent a variety of personas but typically default to a helpful Assistant identity cultivated during post-training.
2. 方法：提出/研究 **The Assistant Axis**；Across several different models, we find an “Assistant Axis" in their activation space, which captures the extent to which a…
3. 机制：Across several different models, we find an “Assistant Axis" in their activation space, which captures the extent to which a model is…
4. 理论/证据：Steering towards the Assistant direction reinforces helpful and harmless behavior; steering away increases the model’s tendency to identify as other…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[The Assistant Axis: Situating and Stabilizing the Default Persona of Language Models](https://openreview.net/forum?id=q17jVxMtwS)

## 415. [Spotlight] The Axiomatic Value of Regularization in AI Alignment from Human Preferences

1. 问题：While RLHF is typically modelled as a problem of learning a single preference ranking from noisy feedback, true human preferences are complex…
2. 方法：提出/研究 **The Axiomatic Value of Regularization in AI Alignment…**；While RLHF is typically modelled as a problem of learning a single preference ranking from noisy feedback, true human preferences…
3. 机制：Seen through this lens, the standard learning objective in RLHF is equivalent to aggregating diverse human preferences via the Borda count rule.
4. 理论/证据：With this motivation, a recent line of research has studied RLHF from the perspective of social choice theory, which provides…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[The Axiomatic Value of Regularization in AI Alignment from Human Preferences](https://openreview.net/forum?id=9ydYaIe1Qj)

## 416. [Spotlight] The Double-Edged Nature of the Rashomon Set for Trustworthy Machine Learning

1. 问题：In contrast, the diversity within a large Rashomon set enables reactive robustness: even when an attack compromises one model, a practitioner can…
2. 方法：提出/研究 **The Double-Edged Nature of the Rashomon Set for…**；We show that this multiplicity reshapes key aspects of trustworthiness.
3. 机制：We show that this multiplicity reshapes key aspects of trustworthiness.
4. 理论/证据：Real-world machine learning (ML) pipelines rarely produce a single model; instead, they produce a Rashomon set of many near-optimal ones.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[The Double-Edged Nature of the Rashomon Set for Trustworthy Machine Learning](https://openreview.net/forum?id=Z6OZh3CgkU)

## 417. [Oral] The Flexibility Trap: Rethinking the Value of Arbitrary Order in Diffusion Language Models

1. 问题：However, in this paper, we find that for general reasoning tasks (e.g., mathematics and coding), arbitrary order generation may in fact limit…
2. 方法：提出/研究 **The Flexibility Trap**；Intuitively, this flexibility implies a solution space that strictly supersets the fixed autoregressive trajectory, theoretically unlocking superior reasoning potential.
3. 机制：Intuitively, this flexibility implies a solution space that strictly supersets the fixed autoregressive trajectory, theoretically unlocking superior reasoning potential.
4. 结果：Our approach, JustGRPO, is minimalist yet surprisingly effective (e.g., 89.1\% accuracy on GSM8K) while fully retaining the parallel decoding ability of dLLMs.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[The Flexibility Trap: Rethinking the Value of Arbitrary Order in Diffusion Language Models](https://openreview.net/forum?id=kpgURPRMGf)

## 418. [Oral] The Obfuscation Atlas: Mapping Where Honesty Emerges in RLVR with Deception Probes

1. 问题：However, such training risks models learning to obfuscate their deception to evade the detector.
2. 方法：提出/研究 **taxonomy of possible outcomes when training against a deception detect**；We introduce a taxonomy of possible outcomes when training against a deception detector.
3. 机制：We construct a realistic coding environment where reward hacking via hardcoding test cases naturally occurs, and show that obfuscation emerges in this…
4. 理论/证据：The detector penalty only incentivizes obfuscated policies; we theoretically show this is expected for policy gradient methods.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[The Obfuscation Atlas: Mapping Where Honesty Emerges in RLVR with Deception Probes](https://openreview.net/forum?id=wrGSN9kAVD)

## 419. [Spotlight] The Power of Power Law: Asymmetry Enables Compositional Reasoning

1. 问题：Natural language data follows a power-law distribution, with most knowledge and skills appearing at very low frequency.
2. 方法：提出/研究 **minimalist skill-composition task and show that learning under a power**；To understand this advantage, we introduce a minimalist skill-composition task and show that learning under a power-law distribution provably requires…
3. 机制：To understand this advantage, we introduce a minimalist skill-composition task and show that learning under a power-law distribution provably requires significantly less…
4. 理论/证据：While a common intuition suggests that reweighting or curating data toward a uniform distribution may help models better learn these…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[The Power of Power Law: Asymmetry Enables Compositional Reasoning](https://openreview.net/forum?id=K83orsg2X9)

## 420. [Spotlight] The Relative Instability of Model Comparison with Cross-validation

1. 问题：Cross-validation (CV) is known to provide asymptotically exact tests and confidence intervals for model improvement but only when the model comparison is…
2. 方法：提出/研究 **The Relative Instability of Model Comparison with Cross-validation**；Surprisingly, we prove that even simple, individually stable models can generate relatively unstable comparisons, calling into question the validity of…
3. 机制：Surprisingly, we prove that even simple, individually stable models can generate relatively unstable comparisons, calling into question the validity of CV inference.
4. 结果：Cross-validation (CV) is known to provide asymptotically exact tests and confidence intervals for model improvement but only when the model comparison is…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[The Relative Instability of Model Comparison with Cross-validation](https://openreview.net/forum?id=kpdyQ1GDRt)

## 421. [Oral] The Signal is in the Steps: Local Scoring for Reasoning Data Selection

1. 问题：However, we find that this approach works within a single teacher but fails when scaling to long reasoning traces from multiple diverse…
2. 方法：提出/研究 **Local Average Log Probability (LALP)**；We propose Local Average Log Probability (LALP), which scores each reasoning step using only a small window of preceding context…
3. 机制：We propose Local Average Log Probability (LALP), which scores each reasoning step using only a small window of preceding context, measuring whether…
4. 结果：Across math, coding, and science reasoning tasks, LALP consistently improves accuracy when selecting the most natural solutions by a large margin.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[The Signal is in the Steps: Local Scoring for Reasoning Data Selection](https://openreview.net/forum?id=GcB3a6IonG)

## 422. [Spotlight] The Tell-Tale Norm: _2 Magnitude as a Signal for Reasoning Dynamics in Large Language Models

1. 问题：Recent work has sought to understand Large Language Models (LLMs) reasoning, yet a principled, model-intrinsic signal that captures its *layer-wise reasoning dynamics*…
2. 方法：提出/研究 **The Tell-Tale Norm**；Motivated by this pattern, we establish a formal link between reasoning intensity and the model's latent geometry and theoretically prove…
3. 机制：Motivated by this pattern, we establish a formal link between reasoning intensity and the model's latent geometry and theoretically prove that the…
4. 结果：Experiments across model architectures and benchmarks show that _2-norm-based techniques significantly improve reasoning performance, offering a principled yet simple lens to perceive…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[The Tell-Tale Norm: _2 Magnitude as a Signal for Reasoning Dynamics in Large Language Models](https://openreview.net/forum?id=03ZTlJuX0y)

## 423. [Spotlight] The Value of Variance: Mitigating Debate Collapse in Multi-Agent Systems via Uncertainty-Driven Policy Optimization

1. 问题：Multi-agent debate (MAD) systems improve LLM reasoning through iterative deliberation, but remain vulnerable to debate collapse, a failure type where final agent…
2. 方法：提出/研究 **mitigation strategy by formulating an uncertainty-driven policy optimi**；Subsequently, we propose a mitigation strategy by formulating an uncertainty-driven policy optimization to penalize self-contradiction, peer conflict, and low-confidence outputs…
3. 机制：Multi-agent debate (MAD) systems improve LLM reasoning through iterative deliberation, but remain vulnerable to debate collapse, a failure type where final agent…
4. 结果：Experiments demonstrate that our proposed uncertainty-driven mitigation reliably calibrates the multi-agent system by consistently improving decision accuracy while reducing system…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[The Value of Variance: Mitigating Debate Collapse in Multi-Agent Systems via Uncertainty-Driven Policy Optimization](https://openreview.net/forum?id=Bc6c2OVWRh)

## 424. [Spotlight] Think in Cloud, Look at Edges: Semantic-Driven Query Decomposition for Efficient Video Reasoning

1. 问题：Long video understanding faces a critical dilemma: cloud-based Large Multimodal Models (LMMs) offer superior reasoning but suffer from prohibitive bandwidth costs and…
2. 方法：提出/研究 **SCOPE**；To solve this, we introduce SCOPE (Semantic Cloud-Orchestrated Perception at Edge).
3. 机制：Current collaborative approaches attempt to bridge this gap via similarity-based filtering, yet they treat complex queries as flat semantic vectors.
4. 结果：Experiments on Video-MME and LongVideoBench demonstrate that SCOPE redefines the Pareto frontier, matching cloud-level accuracy with significantly lower transmission costs and outperforming…
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[Think in Cloud, Look at Edges: Semantic-Driven Query Decomposition for Efficient Video Reasoning](https://openreview.net/forum?id=9HyDFcKhLV)

## 425. [Spotlight] Thinking in Flow: A Dissipative Stabilization Operator for Robust Autoregressive Reasoning

1. 问题：Chain-of-Thought (CoT) prompting enables multi-step reasoning in large language models, yet long-horizon generation remains brittle under distribution shift and context interference: irrelevant…
2. 方法：提出/研究 ***ODE-guided language models***；Specifically, we propose *ODE-guided language models*, which augment a base Transformer with a persistent continuous-time *thought state* whose dynamics are…
3. 机制：Instantiating this framework, *Thinking in Flow* (TiF) equips the model with a lightweight Neural ODE controller and injects its output through post-norm…
4. 结果：We establish well-posedness, dissipativity, and incremental stability of the controlled thought dynamics, implying bounded interventions over arbitrarily long contexts, and…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Thinking in Flow: A Dissipative Stabilization Operator for Robust Autoregressive Reasoning](https://openreview.net/forum?id=9IQpUEKOGM)

## 426. [Oral] ThreadWeaver: Adaptive Threading for Efficient Parallel Reasoning in Language Models

1. 问题：However, existing parallel reasoning approaches suffer from performance degradation compared to their sequential counterparts, and often rely on specialized inference engines.
2. 方法：提出/研究 **ThreadWeaver**；We introduce ThreadWeaver, a framework for adaptive parallel reasoning that matches the accuracy of comparably sized sequential reasoning models while…
3. 机制：We introduce ThreadWeaver, a framework for adaptive parallel reasoning that matches the accuracy of comparably sized sequential reasoning models while significantly reducing…
4. 结果：Across six challenging math reasoning benchmarks, ThreadWeaver trained on top of Qwen3-8B achieves performance on par with cutting-edge sequential reasoning models (79.9%…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[ThreadWeaver: Adaptive Threading for Efficient Parallel Reasoning in Language Models](https://openreview.net/forum?id=Efq2VvYk1o)

## 427. [Spotlight] ThunderAgent: A Fast, Simple, and Program-Aware Agentic Inference System

1. 问题：Large language models (LLMs) are now used to power complex multi-turn agentic workflows.
2. 方法：提出/研究 ****ThunderAgent****；To address the challenges, we propose **ThunderAgent**, a fast, simple, and program-aware agentic inference system.
3. 机制：To address the challenges, we propose **ThunderAgent**, a fast, simple, and program-aware agentic inference system.
4. 结果：Evaluations across coding, routing, and scientific discovery agents demonstrate that ThunderAgent achieves **1.5-3.6×** throughput improvements in serving, **1.8-3.9×** in RL rollout, and…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[ThunderAgent: A Fast, Simple, and Program-Aware Agentic Inference System](https://openreview.net/forum?id=kR4iOTaAOJ)

## 428. [Spotlight] TideGS: Scalable Training of Over One Billion 3D Gaussian Splatting Primitives via Out-of-Core Optimization

1. 问题：Training 3D Gaussian Splatting (3DGS) at billion-primitive scale is fundamentally memory-bound: each Gaussian primitive carries a large attribute vector, and the aggregate…
2. 方法：提出/研究 **TideGS**；Building on this insight, we introduce TideGS, an out-of-core training framework that manages parameters across an SSD-CPU-GPU hierarchy via three…
3. 机制：Building on this insight, we introduce TideGS, an out-of-core training framework that manages parameters across an SSD-CPU-GPU hierarchy via three synergistic techniques…
4. 结果：Experiments show that TideGS enables training with over one billion Gaussians on a single 24-GB GPU while achieving the best reconstruction quality…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[TideGS: Scalable Training of Over One Billion 3D Gaussian Splatting Primitives via Out-of-Core Optimization](https://openreview.net/forum?id=K8UWWJUNYf)

## 429. [Spotlight] Tilt Matching for Scalable Sampling and Fine-Tuning

1. 问题：The approach, Tilt Matching, arises from a dynamical equation relating the flow matching velocity to one targeting the same distribution tilted by…
2. 方法：提出/研究 **simple**；We propose a simple, scalable algorithm based on stochastic interpolants for sampling from unnormalized densities and for fine-tuning generative models.
3. 机制：The method requires neither reward gradients nor backpropagation through trajectories of the flow or diffusion.
4. 结果：We empirically demonstrate that the approach is efficient and highly scalable, providing state-of-the-art results on sampling under Lennard-Jones systems and competitive performance…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Tilt Matching for Scalable Sampling and Fine-Tuning](https://openreview.net/forum?id=dQA4Gjt4KU)

## 430. [Spotlight] Time series saliency maps: Explaining models across multiple domains

1. 问题：However, in the context of time series, they offer limited insights because semantically meaningful features are often found in other domains.
2. 方法：提出/研究 **in this paper Cross-domain Integrated Gradients**；Thus, we introduce in this paper Cross-domain Integrated Gradients, a generalization of Integrated Gradients that enables feature attributions in any…
3. 机制：We validate our method via controlled mechanistic experiments, quantitative faithfulness and perturbation-stability tests, and real-world case studies.
4. 结果：We validate our method via controlled mechanistic experiments, quantitative faithfulness and perturbation-stability tests, and real-world case studies.
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Time series saliency maps: Explaining models across multiple domains](https://openreview.net/forum?id=Bd0NNopzpC)

## 431. [Spotlight] TimeRewarder: Learning Dense Reward from Passive Videos via Frame-wise Temporal Distance

1. 问题：Designing dense rewards is crucial for reinforcement learning (RL), yet in robotics it often demands extensive manual effort and lacks scalability.
2. 方法：提出/研究 **TimeRewarder**；We present TimeRewarder, a simple yet effective reward learning method that derives progress estimation signals from passive videos, including robot…
3. 机制：We present TimeRewarder, a simple yet effective reward learning method that derives progress estimation signals from passive videos, including robot demonstrations and…
4. 结果：This approach outperforms previous methods and even the manually designed environment dense reward on both the final success rate and sample efficiency.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[TimeRewarder: Learning Dense Reward from Passive Videos via Frame-wise Temporal Distance](https://openreview.net/forum?id=XztRm216YS)

## 432. [Oral] To Grok Grokking: Provable Grokking in Ridge Regression

1. 问题：We study *grokking* — the onset of generalization long after overfitting — in a classical ridge regression setting.
2. 方法：提出/研究 **To Grok Grokking**；We prove end-to-end grokking results for learning over-parameterized linear regression models using gradient descent with weight decay.
3. 机制：Moreover, we show, both theoretically and empirically, that grokking can be amplified or eliminated in a principled manner through proper hyperparameter tuning.
4. 理论/证据：We prove end-to-end grokking results for learning over-parameterized linear regression models using gradient descent with weight decay.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[To Grok Grokking: Provable Grokking in Ridge Regression](https://openreview.net/forum?id=5nNNVY8NW4)

## 433. [Oral] TokSuite: Measuring the Impact of Tokenizer Choice on Language Model Behavior

1. 问题：Despite the importance of tokenization, its role in LM performance and behavior is poorly understood due to the challenge of measuring the…
2. 方法：提出/研究 **TokSuite**；To address this need, we present TokSuite, a collection of models and a benchmark that supports research into tokenization's influence…
3. 机制：Tokenizers provide the fundamental basis through which text is represented and processed by language models (LMs).
4. 结果：We also release a multilingual robustness benchmark that measures model performance under real-world perturbations in English, Chinese, Farsi, Italian, and Turkish, curated…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[TokSuite: Measuring the Impact of Tokenizer Choice on Language Model Behavior](https://openreview.net/forum?id=vIZz7LvObC)

## 434. [Spotlight] Toward Stable Value Alignment: Introducing Independent Modules for Consistent Value Guidance

1. 问题：However, a critical gap exists: the model’s residual stream is highly dynamic, in which values exist as fragile, low-dimensional properties, inherently incompatible…
2. 方法：提出/研究 **Stable Value Guidance Transformer (SVGT)**；In this paper, we propose the Stable Value Guidance Transformer (SVGT), which addresses this gap through an independent value module…
3. 机制：In this paper, we propose the Stable Value Guidance Transformer (SVGT), which addresses this gap through an independent value module incorporating two…
4. 结果：Experiments across multiple backbones and safety benchmarks show that SVGT generally reduces harmful scores by over 70\% while maintaining generation fluency, demonstrating…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Toward Stable Value Alignment: Introducing Independent Modules for Consistent Value Guidance](https://openreview.net/forum?id=R80JLmXXPJ)

## 435. [Spotlight] Towards Efficient LLMs Annealing with Principled Sample Selection

1. 问题：However, effectively selecting training data during this phase remains a key challenge.
2. 方法：提出/研究 **data selection as a problem of satisfying these directional constraint**；Building on this insight, we formulate data selection as a problem of satisfying these directional constraints.
3. 机制：In this work, we characterize the annealing phase through the lens of the loss landscape's spectral geometry.
4. 结果：Extensive experiments across various model scales demonstrate that **DiReCT** consistently achieves state-of-the-art performance.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Towards Efficient LLMs Annealing with Principled Sample Selection](https://openreview.net/forum?id=2UH01A9Za0)

## 436. [Oral] Towards Hierarchy–Uniformity Equilibrium: Recovering Semantic Depth in Hypergraph Contrastive Learning

1. 问题：Hypergraph contrastive learning is an effective paradigm for representation learning on higher-order relational data, yet existing methods largely ignore that hyperedges link…
2. 方法：提出/研究 ****HyperDepth****；To address this issue, we introduce **HyperDepth**, a hypergraph contrastive learning framework that moves representations towards a hierarchy–uniformity equilibrium by…
3. 机制：Standard contrastive objectives emphasize instance discrimination via hyperspherical uniformity and tend to push embeddings apart in an indiscriminate manner.
4. 结果：Experiments on 15 hypergraph datasets and 17 supervised and self-supervised baselines, spanning homophilic and heterophilic regimes, show that HyperDepth attains strong performance…
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[Towards Hierarchy–Uniformity Equilibrium: Recovering Semantic Depth in Hypergraph Contrastive Learning](https://openreview.net/forum?id=88qwqo7VSK)

## 437. [Spotlight] Towards High-Fidelity CAD Generation via LLM-Driven Program Generation and Text-Based B-Rep Primitive Grounding

1. 问题：Consequently, this paradigm gap remains a critical factor limiting AI-driven CAD modeling for complex industrial product design.
2. 方法：提出/研究 **Towards High-Fidelity CAD Generation via LLM-Driven Program Generation…**；Existing methods typically fall into two separate categories: parametric CAD modeling and direct boundary representation (B-Rep) synthesis.
3. 机制：Our method generates executable CadQuery scripts, and introduces a text-based query mechanism that enables the LLM to specify geometric selections via natural…
4. 结果：Experiments show that *FutureCAD* achieves state-of-the-art CAD generation performance.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Towards High-Fidelity CAD Generation via LLM-Driven Program Generation and Text-Based B-Rep Primitive Grounding](https://openreview.net/forum?id=jfOhTGs5G5)

## 438. [Oral] Towards Long-Horizon Interpretability: Efficient and Faithful Multi-Token Attribution for Reasoning LLMs

1. 问题：However, as modern LLMs increasingly rely on extended reasoning chains, existing schemes face two critical challenges: (1) efficiency bottleneck, where attributing a…
2. 方法：提出/研究 **FlashTrace**；To address these, we introduce FlashTrace, an efficient multi-token attribution method that employs span-wise aggregation to compute attribution over multi-token…
3. 机制：Moreover, we design a recursive attribution mechanism that traces importance through intermediate reasoning chains back to source inputs.
4. 结果：We further analyze the dynamics of recursive attribution, showing that even a single recursive hop improves faithfulness by tracing importance through the…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Towards Long-Horizon Interpretability: Efficient and Faithful Multi-Token Attribution for Reasoning LLMs](https://openreview.net/forum?id=KY5Q9V9F5C)

## 439. [Spotlight] Towards Optimal Robustness in Learning-Augmented Paging

1. 问题：Learning-augmented paging has been extensively studied in recent years.
2. 方法：提出/研究 **new framework that achieves the best-possible robustness up to an…**；Guided by the above analysis, we develop a new framework that achieves the best-possible robustness up to an additive constant…
3. 机制：Guided by the above analysis, we develop a new framework that achieves the best-possible robustness up to an additive constant for learning-augmented…
4. 结果：Experiments further demonstrate strong practical performance.
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Towards Optimal Robustness in Learning-Augmented Paging](https://openreview.net/forum?id=ESa07RwpVr)

## 440. [Spotlight] Towards Pareto-Optimal Tool-Integrated Agents with Pareto Ranking Policy Optimization

1. 问题：However, existing alignment methods predominantly focus on maximizing task accuracy, while overlooking auxiliary objectives such as tool-use efficiency, which are essential for…
2. 方法：提出/研究 **ParetoPO**；To address this gap, we introduce ParetoPO, a two-stage multi-objective optimization framework for aligning tool-using large language models (LLMs) under…
3. 机制：In the second stage, it replaces scalarized learning signals with Pareto-ranking-based advantage computation, promoting nondominated trajectories through dominance-aware credit assignment.
4. 结果：Experimental results on mathematic reasoning and multi-hop QA tasks show that ParetoPO consistently discovers policies with superior accuracy-efficiency trade-offs compared…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Towards Pareto-Optimal Tool-Integrated Agents with Pareto Ranking Policy Optimization](https://openreview.net/forum?id=9sg34nj13o)

## 441. [Spotlight] Towards Sub-Second Molecular Docking as a Structural Primitive: A Quantized Consistency Diffusion Framework

1. 问题：Molecular docking exposes this bottleneck: it provides essential structural feedback for drug discovery, yet current high-fidelity docking and co-folding models remain limited…
2. 方法：提出/研究 **compute-efficient co-folding framework that turns molecular docking in**；We present a compute-efficient co-folding framework that turns molecular docking into a sub-second structural primitive.
3. 机制：Our framework combines two ideas.
4. 理论/证据：First, Progressive Consistency Regularization (PCR) compresses diffusion dynamics into reliable few-step inference through reconstruction-anchored consistency tuning.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Towards Sub-Second Molecular Docking as a Structural Primitive: A Quantized Consistency Diffusion Framework](https://openreview.net/forum?id=NyPHOtsJfE)

## 442. [Spotlight] Towards the Explainability of Temporal Graph Networks via Memory Backtracking and Topological Attribution

1. 问题：Temporal graphs are ubiquitous in real-world applications and Temporal Graph Networks (TGNs) have achieved superior predictive accuracy.
2. 方法：提出/研究 **optimization objectives to identify the important events**；Finally, top-k selection may be unfaithful due to the nonlinear mapping from logits to probabilities, we design optimization objectives to…
3. 机制：To address this, we attribute TGNs predictions through the topology attribution tree and memory backtracking tree.
4. 结果：Experiments on nine temporal graph datasets, spanning node property prediction, link prediction tasks and graph classification tasks, show that our method provides…
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[Towards the Explainability of Temporal Graph Networks via Memory Backtracking and Topological Attribution](https://openreview.net/forum?id=sKAgLgpujy)

## 443. [Spotlight] Towards Understanding Adam Convergence on Highly Degenerate Polynomials

1. 问题：Adam is a widely used optimization algorithm in deep learning, yet the specific class of objective functions where it exhibits inherent advantages…
2. 方法：提出/研究 **Towards Understanding Adam Convergence on Highly Degenerate Polynomials**；Unlike prior studies requiring external schedulers and _2 near 1 for convergence, this work investigates the ``natural'' auto-convergence properties of…
3. 机制：Unlike prior studies requiring external schedulers and _2 near 1 for convergence, this work investigates the ``natural'' auto-convergence properties of Adam.
4. 结果：We prove that Adam achieves local linear convergence on these degenerate functions, significantly outperforming the sub-linear convergence of Gradient Descent and Momentum.
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Towards Understanding Adam Convergence on Highly Degenerate Polynomials](https://openreview.net/forum?id=uYWVGk1Qt0)

## 444. [Spotlight] Train for Truth, Keep the Skills: Binary Retrieval-Augmented Reward Mitigates Hallucinations

1. 问题：Modern post-trained language models are increasingly capable, but remain prone to extrinsic hallucinations.
2. 方法：提出/研究 **Train for Truth, Keep the Skills**；We target the utility degradation issue that prior hallucination-reduction methods often struggle to avoid, and propose online RL with Binary…
3. 机制：Our error analysis shows that continuous factuality rewards (e.g., VeriScore) can be exploited via reward hacking by producing fewer or more generic…
4. 结果：On Qwen3-8B, it reduces long-form hallucination rates by 39.3\% and short-form hallucination rates by 54.4\%, outperforming supervised learning and preference optimization baselines.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Train for Truth, Keep the Skills: Binary Retrieval-Augmented Reward Mitigates Hallucinations](https://openreview.net/forum?id=BNCNSgLPy5)

## 445. [Spotlight] Training Diffusion Language Models for Black-Box Optimization

1. 问题：We study offline black-box optimization (BBO), aiming to discover improved designs from an offline dataset of designs and labels, a problem common…
2. 方法：提出/研究 **dapting diffusion LLMs to offline BBO to leverage their bidirectional**；To address this, we propose adapting diffusion LLMs to offline BBO to leverage their bidirectional modeling capabilities.
3. 机制：The first stage performs supervised fine-tuning on the unified dataset via masked-response prediction, and the second stage adopts reinforcement learning with rewards…
4. 结果：Our method achieves state-of-the-art results on Design-Bench under small-data settings.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Training Diffusion Language Models for Black-Box Optimization](https://openreview.net/forum?id=Z7wI0sor6i)

## 446. [Oral] Training-Free Bayesian Filtering with Generative Emulators

1. 问题：Bayesian filtering is a well-known problem that aims to estimate plausible states of a dynamical system from observations.
2. 方法：提出/研究 **Training-Free Bayesian Filtering with Generative Emulators**；Among existing approaches to solve this problem, particle filters are theoretically exact for non-linear dynamics and observations, but suffer from…
3. 机制：Among existing approaches to solve this problem, particle filters are theoretically exact for non-linear dynamics and observations, but suffer from poor scalability…
4. 结果：Experiments on nonlinear chaotic systems, including atmospheric dynamics, demonstrate that the proposed approach successfully scales particle filtering to high-dimensional settings.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Training-Free Bayesian Filtering with Generative Emulators](https://openreview.net/forum?id=ibcZNZwKfZ)

## 447. [Spotlight] Transformer Circuits Can Realize Clustering Algorithms

1. 问题：Although transformers are most commonly optimized as statistical sequence models, it is unclear to what extent they can implement and learn exact…
2. 方法：提出/研究 **Transformer Circuits Can Realize Clustering Algorithms**；Here, we specify a transformer implementation from first principles that executes a fundamental and widely used method for k-means clustering…
3. 机制：Here, we specify a transformer implementation from first principles that executes a fundamental and widely used method for k-means clustering: Lloyd's algorithm.
4. 理论/证据：We theoretically prove and empirically demonstrate that this implementation of a transformer architecture, which we term the _k-means transformer_, exactly…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Transformer Circuits Can Realize Clustering Algorithms](https://openreview.net/forum?id=2jw5U060C4)

## 448. [Oral] Transforming Weather Data from Pixel to Latent Space

1. 问题：However, existing studies often rely on weather data in pixel space, which presents several challenges such as smooth outputs in model outputs…
2. 方法：提出/研究 **novel Weather Latent Autoencoder (WLA) that transforms weather data fr**；To address these challenges, we propose a novel Weather Latent Autoencoder (WLA) that transforms weather data from pixel space to…
3. 机制：Through extensive experimentation, we demonstrate its superior compression and reconstruction performance, enabling the creation of the ERA5-Latent dataset with unified representations of…
4. 结果：The downstream task further demonstrates that task models can apply to multiple PVS with low data costs in latent space and achieve…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Transforming Weather Data from Pixel to Latent Space](https://openreview.net/forum?id=NlSWKeQPoZ)

## 449. [Spotlight] Treatment Responder Classification with Abstention

1. 问题：Rigorous theories and extensive experiments on two real-world datasets demonstrate the theoretical and experimental guarantee on our methods in learning treatment responders…
2. 方法：提出/研究 **doubly robust method named TRECA to learn the classification rule…**；By revealing the implicit relation between causal misclassification risk with abstention and Conditional Value at Risk (CVaR), we develop a…
3. 机制：By revealing the implicit relation between causal misclassification risk with abstention and Conditional Value at Risk (CVaR), we develop a doubly robust…
4. 结果：Rigorous theories and extensive experiments on two real-world datasets demonstrate the theoretical and experimental guarantee on our methods in learning treatment responders…
5. 启示：可识别性条件、干预设计和局部结构，比单纯提高预测精度更决定因果结论是否可信。

论文页面：[Treatment Responder Classification with Abstention](https://openreview.net/forum?id=WFdQSjmchK)

## 450. [Spotlight] Trojan-Speak: Bypassing Constitutional Classifiers with No Jailbreak Tax via Adversarial Finetuning

1. 问题：Fine-tuning APIs offered by major AI providers create new attack surfaces where adversaries can bypass safety measures through targeted fine-tuning.
2. 方法：提出/研究 ****Trojan-Speak****；We introduce **Trojan-Speak**, an adversarial fine-tuning method that bypasses Anthropic's Constitutional Classifiers.
3. 机制：Fine-tuning APIs offered by major AI providers create new attack surfaces where adversaries can bypass safety measures through targeted fine-tuning.
4. 结果：Our findings reveal that LLM-based content classifiers alone are insufficient for preventing dangerous information disclosure when adversaries have fine-tuning access…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Trojan-Speak: Bypassing Constitutional Classifiers with No Jailbreak Tax via Adversarial Finetuning](https://openreview.net/forum?id=5Aydbj0wYI)

## 451. [Spotlight] UDM-GRPO: Stable and Efficient Group Relative Policy Optimization for Uniform Discrete Diffusion Models

1. 问题：Uniform Discrete Diffusion Model (UDM) has recently emerged as a promising paradigm for discrete generative modeling; however, its integration with reinforcement learning…
2. 方法：提出/研究 ****UDM-GRPO****；To address this, we propose **UDM-GRPO**, the first framework to integrate UDM with RL.
3. 机制：Our method is guided by two key insights: (i) treating the final clean sample as the action provides more accurate and stable…
4. 结果：On the OCR benchmark, accuracy rises from 8\\% to 57\\%, further validating the generalization ability of our method.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[UDM-GRPO: Stable and Efficient Group Relative Policy Optimization for Uniform Discrete Diffusion Models](https://openreview.net/forum?id=WJcFtJriqv)

## 452. [Spotlight] Uncovering the Latent Potential of Deep Intermediate Representations

1. 问题：Foundational models pretrained on huge amounts of data learn representations that evolve across depth, forming a hierarchy of embeddings with distinct semantic…
2. 方法：提出/研究 **Layer-wise Optimal Embedding Selection (LOES)**；We introduce Layer-wise Optimal Embedding Selection (LOES), a constructive spectral method that identifies task-discriminative subspaces by minimizing residual error under…
3. 机制：Through a geometric and empirical study across multiple modalities, we show that effective transfer depends on identifying which layers encode task-discriminative structure…
4. 理论/证据：Contrary to the widespread practice of using only the final layer or shallow mixtures, we show that task-relevant information is…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[Uncovering the Latent Potential of Deep Intermediate Representations](https://openreview.net/forum?id=6up1qGJwYZ)

## 453. [Spotlight] Understanding Self-Supervised Learning via Latent Distribution Matching

1. 问题：Self-supervised learning (SSL) excels at finding general-purpose latent representations from complex data, yet lacks a unifying theoretical framework that explains the diverse…
2. 方法：提出/研究 **Understanding Self-Supervised Learning via Latent Distribution Matching**；We cast SSL as latent distribution matching (LDM): learning representations that maximize their log-probability under an assumed latent model (alignment)…
3. 机制：We cast SSL as latent distribution matching (LDM): learning representations that maximize their log-probability under an assumed latent model (alignment), while maximizing…
4. 理论/证据：Self-supervised learning (SSL) excels at finding general-purpose latent representations from complex data, yet lacks a unifying theoretical framework that explains…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[Understanding Self-Supervised Learning via Latent Distribution Matching](https://openreview.net/forum?id=schXkGSTus)

## 454. [Spotlight] Unifying and Optimizing Data Values for Selection via Sequential Decision-Making

1. 问题：Data selection has emerged as a crucial downstream application of data valuation, yet the theoretical foundations for using data values in selection…
2. 方法：提出/研究 **n efficient bipartite graph-based surrogate that preserves submodular**；To bridge theory and practice, we propose an efficient bipartite graph-based surrogate that preserves submodular structure while enabling scalable greedy…
3. 机制：This framework unifies and reinterprets existing methods like Data Shapley through the lens of approximate dynamic programming, revealing them as myopic linear…
4. 结果：Experiments on classical ML benchmarks and large-scale LLM fine-tuning data selection demonstrate substantial improvements over existing methods.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Unifying and Optimizing Data Values for Selection via Sequential Decision-Making](https://openreview.net/forum?id=GFFMLwn053)

## 455. [Spotlight] Unifying Masked Diffusion Models with Various Generation Orders and Beyond

1. 问题：Prior work either hard-codes an ordering (e.g., blockwise left-to-right) or learns an ordering policy for a pretrained MDM, which incurs extra cost…
2. 方法：提出/研究 **order-expressive masked diffusion model (OeMDM) for a broad class of…**；Motivated by this, we propose order-expressive masked diffusion model (OeMDM) for a broad class of diffusion generative processes with various…
3. 机制：Furthermore, building on OeMDM, we introduce learnable-order masked diffusion model (LoMDM), which jointly learns the generation ordering and diffusion backbone through a…
4. 结果：Empirically, we confirm that LoMDM outperforms various discrete diffusion models across multiple language modeling benchmarks.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Unifying Masked Diffusion Models with Various Generation Orders and Beyond](https://openreview.net/forum?id=ATpOQt9VVd)

## 456. [Spotlight] UniMapping: Unified SLAM Framework for Map-Centric Embodied Perception

1. 问题：However, existing approaches often struggle with scale-consistency and producing maps that lack the geometric fidelity required for reliable perception.
2. 方法：提出/研究 **_UniMapping_**；We propose _UniMapping_, a unified SLAM framework that constructs a persistent neural-descriptor map from multimodal observations.
3. 机制：We propose _UniMapping_, a unified SLAM framework that constructs a persistent neural-descriptor map from multimodal observations.
4. 结果：Notably, our method significantly enhances downstream tasks (mAP +3.1% and mIoU +7.1%) by leveraging accumulated multi-view context.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[UniMapping: Unified SLAM Framework for Map-Centric Embodied Perception](https://openreview.net/forum?id=bQkKVGuHZA)

## 457. [Spotlight] UniPercept: Towards Unified Perceptual-Level Image Understanding across Aesthetics, Quality, Structure, and Texture

1. 问题：However, their ability to perceive perceptual-level image features remains limited.
2. 方法：提出/研究 **UniPercept-Bench**；In this work, we present UniPercept-Bench, a unified framework for perceptual-level image understanding across three key domains: Aesthetics, Quality, Structure…
3. 机制：Based on this foundation, we develop a strong baseline UniPercept trained via Domain-Adaptive Pre-Training and Task-Aligned RL, enabling robust generalization across both…
4. 结果：This work defines perceptual-level image understanding in the era of MLLMs and, through the introduction of a comprehensive benchmark together with a…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[UniPercept: Towards Unified Perceptual-Level Image Understanding across Aesthetics, Quality, Structure, and Texture](https://openreview.net/forum?id=8VVbElV06v)

## 458. [Spotlight] Universal Redundancies in Time Series Foundation Models

1. 问题：Time Series Foundation Models (TSFMs) leverage extensive pretraining to accurately predict unseen time series during inference, without the need for task-specific fine-tuning.
2. 方法：提出/研究 **set of tools for mechanistic interpretability of TSFMs**；We introduce a set of tools for mechanistic interpretability of TSFMs, including ablations of specific components and direct logit attribution…
3. 机制：Through large-scale evaluations of standard benchmarks, we find that leading transformer-based TSFMs exhibit redundant components in their intermediate layers.
4. 结果：Through large-scale evaluations of standard benchmarks, we find that leading transformer-based TSFMs exhibit redundant components in their intermediate layers.
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Universal Redundancies in Time Series Foundation Models](https://openreview.net/forum?id=DyA4KHj1wy)

## 459. [Spotlight] Unraveling Syntax: Language Modeling and the Substructure of Grammars

1. 问题：While language models achieve impressive results, their *learning dynamics* are far from understood.
2. 方法：提出/研究 **Unraveling Syntax**；Many domains of interest – such as natural language syntax, coding languages, arithmetic – are captured by context-free grammars (CFGs).
3. 机制：Many domains of interest – such as natural language syntax, coding languages, arithmetic – are captured by context-free grammars (CFGs).
4. 结果：We find that subgrammar pretraining can improve final performance, but only for tiny models relative to the grammar, while alignment analyses show…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Unraveling Syntax: Language Modeling and the Substructure of Grammars](https://openreview.net/forum?id=sPIXjSkDFG)

## 460. [Oral] Unsupervised Partner Design Enables Robust Ad-hoc Teamwork

1. 问题：Across Level-Based Foraging, Overcooked-AI, and the Overcooked Generalisation Challenge, UPD consistently achieves strong performance compared to both population-based and population-free baselines.
2. 方法：提出/研究 **Unsupervised Partner Design (UPD)**；We introduce Unsupervised Partner Design (UPD), a population-free multi-agent reinforcement learning method for robust ad-hoc teamwork.
3. 机制：We introduce Unsupervised Partner Design (UPD), a population-free multi-agent reinforcement learning method for robust ad-hoc teamwork.
4. 结果：In a human-AI user study, agents trained with UPD achieve higher returns and are rated as more adaptive, more human-like, and less…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Unsupervised Partner Design Enables Robust Ad-hoc Teamwork](https://openreview.net/forum?id=0xtMUL0eiF)

## 461. [Spotlight] Updating Parametric Knowledge with Context Distillation Retains Post-Training Capabilities

1. 问题：However, these post-trained LLMs only encode knowledge up to a cut-off date, necessitating continual adaptation.
2. 方法：提出/研究 **Distillation via Split Contexts (DiSC)**；To address this, we introduce Distillation via Split Contexts (DiSC), a simple context-distillation based approach for continual knowledge adaptation.
3. 机制：To address this, we introduce Distillation via Split Contexts (DiSC), a simple context-distillation based approach for continual knowledge adaptation.
4. 结果：We run experiments on four post-trained models and two adaptation domains.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Updating Parametric Knowledge with Context Distillation Retains Post-Training Capabilities](https://openreview.net/forum?id=OJsGhlTayF)

## 462. [Oral] VALUEFLOW: Toward Pluralistic and Steerable Value-based Alignment in Large Language Models

1. 问题：Aligning Large Language Models (LLMs) with the diverse spectrum of human values remains a central challenge: preference-based methods often fail to capture…
2. 方法：提出/研究 **VALUEFLOW**；To address these limitations, we introduce VALUEFLOW, a unified framework that spans extraction, evaluation, and steering with calibrated intensity control.
3. 机制：The framework integrates three components: (i) HiVES, a hierarchical value embedding space that captures intra- and cross-theory value structure; (ii) the Value…
4. 理论/证据：The framework integrates three components: (i) HiVES, a hierarchical value embedding space that captures intra- and cross-theory value structure; (ii)…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[VALUEFLOW: Toward Pluralistic and Steerable Value-based Alignment in Large Language Models](https://openreview.net/forum?id=6zVV84vnCJ)

## 463. [Spotlight] Variational Learning for Insertion-based Generation

1. 问题：Non-monotonic sequence generation methods, such as masked diffusion models, provide a flexible alternative to left-to-right autoregressive modeling by allowing tokens to be…
2. 方法：提出/研究 **probabilistic framework for learning insertion order in variable-lengt**；In this work, we introduce a probabilistic framework for learning insertion order in variable-length insertion models.
3. 机制：Building on this result, we propose the Insertion Process (IP), a stochastic generative model that jointly learns where to insert, what to…
4. 结果：Experiments on goal-conditioned planning and molecular string generation demonstrate that learning insertion order improves both modeling quality and generalization in domains without…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Variational Learning for Insertion-based Generation](https://openreview.net/forum?id=thVeEXPaSg)

## 464. [Spotlight] VectorWorld: Efficient Streaming World Model via Diffusion Flow on Vector Graphs

1. 问题：Closed-loop evaluation of autonomous-driving policies requires interactive simulation beyond log replay.
2. 方法：提出/研究 **VectorWorld**；We propose VectorWorld, a streaming vector-graph world model that incrementally generates ego-centric lane—agent tiles during rollout.
3. 机制：We propose VectorWorld, a streaming vector-graph world model that incrementally generates ego-centric lane—agent tiles during rollout.
4. 结果：On Waymo Open Motion and nuPlan, VectorWorld improves map fidelity, initialization validity, and density calibration, enabling stable real-time 1km+ closed-loop rollouts.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[VectorWorld: Efficient Streaming World Model via Diffusion Flow on Vector Graphs](https://openreview.net/forum?id=yTEEiE3YtD)

## 465. [Oral] VenusBench-Mobile: A Challenging and User-Centric Benchmark for Mobile GUI Agents with Capability Diagnostics

1. 问题：Existing online benchmarks for mobile GUI agents remain largely app-centric and task-homogeneous, failing to reflect the diversity and instability of real-world mobile…
2. 方法：提出/研究 **VenusBench-Mobile**；To this end, we introduce VenusBench-Mobile, a challenging online benchmark for evaluating general-purpose mobile GUI agents under realistic, user-centric conditions.
3. 机制：VenusBench-Mobile builds two core evaluation pillars: defining what to evaluate via user-intent-driven task design that reflects real mobile usage, and how to…
4. 结果：Extensive evaluation of state-of-the-art mobile GUI agents reveals large performance gaps relative to prior benchmarks, indicating that VenusBench-Mobile poses substantially more challenging…
5. 启示：该工作通过显式结构假设或任务分解，把原本经验性的方案转化为更可解释、可扩展的设计。

论文页面：[VenusBench-Mobile: A Challenging and User-Centric Benchmark for Mobile GUI Agents with Capability Diagnostics](https://openreview.net/forum?id=coHiGZOFtS)

## 466. [Spotlight] VGGT-Motion: Motion-Aware Calibration-Free Monocular SLAM for Long-Range Consistency

1. 问题：Despite recent progress in calibration-free monocular SLAM via 3D vision foundation models, scale drift remains severe on long sequences.
2. 方法：提出/研究 **VGGT-Motion**；To address these issues, we propose VGGT-Motion, a calibration-free SLAM system for efficient and robust global consistency over kilometer-scale trajectories.
3. 机制：Despite recent progress in calibration-free monocular SLAM via 3D vision foundation models, scale drift remains severe on long sequences.
4. 结果：Experiments show that VGGT-Motion markedly improves trajectory accuracy and efficiency, achieving state-of-the-art performance in zero-shot, long-range calibration-free monocular SLAM.
5. 启示：图学习的关键在于同时处理结构表达能力、可扩展计算和跨规模泛化。

论文页面：[VGGT-Motion: Motion-Aware Calibration-Free Monocular SLAM for Long-Range Consistency](https://openreview.net/forum?id=GyRMbsYFiG)

## 467. [Oral] Video-Based Optimal Transport for Feedback-Efficient Offline Preference-Based Reinforcement Learning

1. 问题：Preference-based RL (PbRL) offers a promising alternative by learning reward functions from human feedback, but its scalability is hindered by high labeling…
2. 方法：提出/研究 **Video-based Optimal Transport Preference (VOTP)**；Inspired by advances in Video Foundation Models (ViFMs), we present Video-based Optimal Transport Preference (VOTP), a semi-supervised framework that learns…
3. 机制：Inspired by advances in Video Foundation Models (ViFMs), we present Video-based Optimal Transport Preference (VOTP), a semi-supervised framework that learns effective reward…
4. 结果：Extensive experiments across locomotion and manipulation benchmarks demonstrate the superiority of VOTP, which outperforms state-of-the-art offline PbRL methods under limited feedback budgets.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[Video-Based Optimal Transport for Feedback-Efficient Offline Preference-Based Reinforcement Learning](https://openreview.net/forum?id=G8LVO5easu)

## 468. [Spotlight] VideoFlexTok: Flexible-Length Coarse-to-Fine Video Tokenization

1. 问题：Visual tokenizers map high-dimensional raw pixels into a compressed representation for downstream modeling.
2. 方法：提出/研究 **_VideoFlexTok_**；This requires the downstream model, e.g., a text-to-video model, to learn to predict all low-level details "pixel-by-pixel" irrespective of the…
3. 机制：This requires the downstream model, e.g., a text-to-video model, to learn to predict all low-level details "pixel-by-pixel" irrespective of the video's inherent…
4. 结果：We evaluate VideoFlexTok on class- and text-to-video generative tasks and show that it yields more efficient training than 3D grid tokens, _achieving…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[VideoFlexTok: Flexible-Length Coarse-to-Fine Video Tokenization](https://openreview.net/forum?id=KyVlaw4BxE)

## 469. [Spotlight] VideoKR: Towards Knowledge- and Reasoning-Intensive Video Understanding

1. 问题：We develop a human-in-the-loop, skill-oriented example generation pipeline that targets progressively deeper video reasoning capabilities while ensuring the difficulty, diversity, and reliability…
2. 方法：提出/研究 **VideoKR**；We introduce VideoKR, the first large-scale training corpus specifically designed to strengthen knowledge- and reasoning-intensive video understanding.
3. 机制：It comprises 315K video reasoning examples over 145K newly collected, CC-licensed, expert-domain videos.
4. 结果：Our experiments show that, under a standard SFT GRPO pipeline, models post-trained on VideoKR outperform prior post-training approaches on knowledge-intensive video reasoning…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[VideoKR: Towards Knowledge- and Reasoning-Intensive Video Understanding](https://openreview.net/forum?id=eXxFlOPTk4)

## 470. [Spotlight] Vision2Web: A Hierarchical Benchmark for Visual Website Development with Agent Verification

1. 问题：Recent advances in large language models have improved the capabilities of coding agents, yet systematic evaluation of complex, end-to-end website development remains…
2. 方法：提出/研究 **Vision2Web**；To address this gap, we introduce Vision2Web, a hierarchical benchmark for visual website development, spanning from static UI-to-code generation, interactive…
3. 机制：The benchmark is constructed from real-world websites and comprises a total of 193 tasks across 16 categories, with 918 prototype images and…
4. 结果：We evaluate multiple visual language models instantiated under different coding-agent frameworks, revealing substantial performance gaps at all task levels, with state-of-the-art models…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Vision2Web: A Hierarchical Benchmark for Visual Website Development with Agent Verification](https://openreview.net/forum?id=lJpXXwhRRF)

## 471. [Spotlight] Wait, Wait, Wait... Why Do Reasoning Models Loop?

1. 问题：Reasoning models (e.g., DeepSeek-R1) generate long chains of thought to solve harder problems, but they often loop, repeating the same text at…
2. 方法：提出/研究 **synthetic graph reasoning task and demonstrate two mechanisms**；To understand how such errors cause loops, we introduce a synthetic graph reasoning task and demonstrate two mechanisms.
3. 机制：To understand how such errors cause loops, we introduce a synthetic graph reasoning task and demonstrate two mechanisms.
4. 结果：To understand how such errors cause loops, we introduce a synthetic graph reasoning task and demonstrate two mechanisms.
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Wait, Wait, Wait... Why Do Reasoning Models Loop?](https://openreview.net/forum?id=oZWE7mSqlk)

## 472. [Spotlight] Walrus: A Cross-domain Foundation Model for Continuum Dynamics

1. 问题：Foundation models have transformed machine learning for language and vision, but achieving comparable impact in physical simulation remains a challenge.
2. 方法：提出/研究 **Walrus**；Using these tools, we develop Walrus, a transformer-based foundation model developed primarily for fluid-like continuum dynamics.
3. 机制：Through empirical and theoretical analysis, we incorporate new approaches to mitigate these obstacles, including a harmonic-analysis–based stabilization method, load-balanced distributed 2D-3D training…
4. 结果：Experiments show that Walrus outperforms prior foundation models on both short- and long-term prediction horizons on downstream tasks and across the breadth…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Walrus: A Cross-domain Foundation Model for Continuum Dynamics](https://openreview.net/forum?id=kcyOjXoUZu)

## 473. [Spotlight] WaterSIC: Information-Theoretically (Near) Optimal \ Layer Quantization

1. 问题：This paper considers the problem of converting a given dense linear layer to low precision.
2. 方法：提出/研究 **WaterSIC**；The tradeoff between compressed length and output discrepancy is analyzed information theoretically (IT).
3. 机制：The tradeoff between compressed length and output discrepancy is analyzed information theoretically (IT).
4. 结果：Applying WaterSIC to the Llama and Qwen family of LLMs establishes new state-of-the-art performance for all quantization rates from 1 to 4…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[WaterSIC: Information-Theoretically (Near) Optimal \ Layer Quantization](https://openreview.net/forum?id=fCPgAHIciE)

## 474. [Spotlight] WBMM: Windowed Batch Matrix Multiplication for Efficient Large Receptive Field Convolution

1. 问题：Large kernel depthwise convolutions achieve strong performance but suffer from significant degradation as kernel size grows due to irregular memory access from…
2. 方法：提出/研究 **Windowed Batch Matrix Multiplication (WBMM)**；We propose Windowed Batch Matrix Multiplication (WBMM), which partitions input into contiguous windows and indexes a compact relative position bias…
3. 机制：We propose Windowed Batch Matrix Multiplication (WBMM), which partitions input into contiguous windows and indexes a compact relative position bias table to…
4. 结果：Combined with inter-block cross-window communication and hierarchical window reparameterization, WBMM achieves comparable or higher accuracy on ImageNet-1K, COCO, and ADE20K…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[WBMM: Windowed Batch Matrix Multiplication for Efficient Large Receptive Field Convolution](https://openreview.net/forum?id=Qg9Jcy788i)

## 475. [Spotlight] Weak Diffusion Priors Can Still Achieve Strong Inverse-Problem Performance

1. 问题：Diffusion models are widely used as priors for inverse problems, but standard approaches usually assume a high-fidelity model trained on data that…
2. 方法：提出/研究 **Weak Diffusion Priors Can Still Achieve Strong Inverse-Problem…**；Diffusion models are widely used as priors for inverse problems, but standard approaches usually assume a high-fidelity model trained on…
3. 机制：Through extensive experiments, we find that weak priors succeed when measurements are highly informative (e.g., many observed pixels), and we identify regimes…
4. 理论/证据：Through extensive experiments, we find that weak priors succeed when measurements are highly informative (e.g., many observed pixels), and we…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[Weak Diffusion Priors Can Still Achieve Strong Inverse-Problem Performance](https://openreview.net/forum?id=fdkSA4F0lN)

## 476. [Oral] WeDLM: Reconciling Diffusion Language Models with Standard Causal Attention for Fast Inference

1. 问题：Diffusion Language Models (DLLMs) offer parallel decoding by recovering multiple masked tokens per step; however, in practice they often fail to translate…
2. 方法：提出/研究 **WeDLM**；We propose WeDLM, a diffusion decoding framework built entirely on standard causal attention to make parallel generation prefix-cache friendly.
3. 机制：We propose WeDLM, a diffusion decoding framework built entirely on standard causal attention to make parallel generation prefix-cache friendly.
4. 结果：Experiments show that WeDLM preserves the quality of strong AR backbones while delivering substantial speedups, approaching 3× on challenging reasoning benchmarks and…
5. 启示：生成模型的性能瓶颈往往位于轨迹几何、采样控制或表示空间，而不只是网络规模。

论文页面：[WeDLM: Reconciling Diffusion Language Models with Standard Causal Attention for Fast Inference](https://openreview.net/forum?id=QwtmbKAOZU)

## 477. [Spotlight] Welfare-Optimal Classification with Accuracy Auctions

1. 问题：Prediction algorithms are increasingly used to inform decisions about humans, but maximizing accuracy—the standard learning objective—is not necessarily optimal for this purpose.
2. 方法：提出/研究 **optimizing social welfare**；Instead, we propose optimizing social welfare, defined as the average gain users receive from correct predictions.
3. 机制：Instead, we propose optimizing social welfare, defined as the average gain users receive from correct predictions.
4. 结果：We conclude with experiments on real and synthetic data that demonstrate our algorithm and explore the connections between welfare and accuracy.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[Welfare-Optimal Classification with Accuracy Auctions](https://openreview.net/forum?id=MA1LUDNA3s)

## 478. [Spotlight] WestWorld: A Knowledge-Encoded Scalable Trajectory World Model for Diverse Robotic Systems

1. 问题：To address these limitations, we introduce *WestWorld*, a kno**W**ledge-**E**ncoded **S**calable **T**rajectory **World** model for diverse robotic systems.
2. 方法：提出/研究 ***WestWorld***；To address these limitations, we introduce *WestWorld*, a kno**W**ledge-**E**ncoded **S**calable **T**rajectory **World** model for diverse robotic systems.
3. 机制：To tackle the scalability challenge, we propose a novel system-aware Mixture-of-Experts (Sys-MoE) that dynamically combines and routes specialized experts for different robotic…
4. 结果：Finally, we deploy our model on a real-world Unitree Go1, where it demonstrates stable locomotion performance.
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[WestWorld: A Knowledge-Encoded Scalable Trajectory World Model for Diverse Robotic Systems](https://openreview.net/forum?id=ncRRCG4BfP)

## 479. [Spotlight] What Do Agents Learn from Trajectory-SFT: Semantics or Interfaces?

1. 问题：Large language models are increasingly evaluated as interactive agents, yet standard agent benchmarks conflate two qualitatively distinct sources of success: semantic tool-use…
2. 方法：提出/研究 ****PIPE****；We propose **PIPE**, a protocol-level evaluation augmentation for diagnosing interface reliance by minimally rewriting environment interfaces while preserving task semantics…
3. 机制：We propose **PIPE**, a protocol-level evaluation augmentation for diagnosing interface reliance by minimally rewriting environment interfaces while preserving task semantics and execution…
4. 结果：Because both mechanisms can yield identical task success on the original interface, benchmark scores alone are not identifiable evidence of…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[What Do Agents Learn from Trajectory-SFT: Semantics or Interfaces?](https://openreview.net/forum?id=u1i3XoSXQG)

## 480. [Spotlight] What Makes Value Learning Efficient in Residual Reinforcement Learning?

1. 问题：However, value learning in residual RL poses unique challenges that remain poorly understood.
2. 方法：提出/研究 **DAWN**；Based on these insights, we propose DAWN (Data-Anchored Warmup and Normalization), a minimal approach targeting efficient value learning in residual…
3. 机制：Through systematic investigation, we uncover the mechanisms underlying these bottlenecks, revealing that simple yet principled solutions suffice: base-policy transitions serve as an…
4. 结果：By addressing these bottlenecks, DAWN demonstrates substantial efficiency gains across diverse benchmarks, policy architectures, and observation modalities.
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[What Makes Value Learning Efficient in Residual Reinforcement Learning?](https://openreview.net/forum?id=tSMZHXtJwZ)

## 481. [Oral] What Preferences Can—and Cannot—Predict in Multi-Agent Online Learning

1. 问题：We examine the interplay between ordinal, preference-based solution concepts in games and the outcomes of payoff-driven learning dynamics, asking to what extent…
2. 方法：提出/研究 **notion of *leaklessness***；To restore stability, we introduce the notion of *leaklessness*, a measure of aggregate payoff drift away from a set of…
3. 机制：To restore stability, we introduce the notion of *leaklessness*, a measure of aggregate payoff drift away from a set of pure profiles…
4. 理论/证据：In one direction, we show that the skeleton of every *dynamically stable* set (i.e., the set of pure profiles it…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[What Preferences Can—and Cannot—Predict in Multi-Agent Online Learning](https://openreview.net/forum?id=5W30WwL8wt)

## 482. [Spotlight] What You Think is What You See: Driving Exploration in VLM Agents via Visual-Linguistic Curiosity

1. 问题：However, mere passive exploitation of reasoning on visited states is insufficient for sparse-reward agentic tasks, as it lacks the epistemic drive to…
2. 方法：提出/研究 ****GLANCE****；We ask: *Can VLM agents actively find signals that challenge and update their internal world model through curiosity-driven exploration?* In…
3. 机制：To navigate partially observable visual environments, recent VLM agents increasingly internalize world modeling capabilities directly into their policies via explicit CoT reasoning…
4. 结果：Extensive experiments across a series of agentic tasks show the effectiveness of **GLANCE**, and demonstrate that aligning *what the agent thinks* with…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[What You Think is What You See: Driving Exploration in VLM Agents via Visual-Linguistic Curiosity](https://openreview.net/forum?id=zWStW3hrfW)

## 483. [Spotlight] When Attributes Disagree: Gradient Conflict in Image Aesthetic Assessment

1. 问题：Image Aesthetic Assessment (IAA) predicts an image’s overall aesthetic score, yet aesthetic is influenced by multiple attributes whose relative importance varies with…
2. 方法：提出/研究 **GREE**；To address these issues, we propose AGREE (Attribute-guided Gradient Routing for Establishing Agreement), which learns attribute-specific subspaces and performs gradient…
3. 机制：AGREE further reduces feature coupling across attributes with semantic anchors and improves robustness via error-aware reweighting.
4. 结果：Experiments on AVA, LAPIS, AADB, TAD66K, and PARA show consistent improvements over diverse IAA baseline models, and AGREE is plug-and-play…
5. 启示：结构化几何、问题相关复杂度和更准确的局部信息，能够突破通用优化方法的最坏情形限制。

论文页面：[When Attributes Disagree: Gradient Conflict in Image Aesthetic Assessment](https://openreview.net/forum?id=GrIs035ec3)

## 484. [Oral] When the Prompt Becomes Visual: Vision-Centric Jailbreak Attacks for Large Image Editing Models

1. 问题：Recent advances in large image editing models have shifted the paradigm from text-driven instructions to vision-prompt editing, where user intent is inferred…
2. 方法：提出/研究 **Vision-Centric Jailbreak Attack (VJA)**；In this work, we propose Vision-Centric Jailbreak Attack (VJA), the first visual-to-visual jailbreak attack that conveys malicious instructions purely through…
3. 机制：In this work, we propose Vision-Centric Jailbreak Attack (VJA), the first visual-to-visual jailbreak attack that conveys malicious instructions purely through visual inputs.
4. 结果：Our findings expose new vulnerabilities, provide both a benchmark and practical defense to advance safe and trustworthy modern image editing systems.
5. 启示：安全与隐私问题需要机制级保证和部署期控制，而不能仅依赖平均测试集表现。

论文页面：[When the Prompt Becomes Visual: Vision-Centric Jailbreak Attacks for Large Image Editing Models](https://openreview.net/forum?id=wQxRphkfxn)

## 485. [Spotlight] When to Trust the Cheap Check: Weak and Strong Verification for Reasoning

1. 问题：These signals differ sharply in cost and reliability: strong verification can establish trust but is resource-intensive, while weak verification is fast and…
2. 方法：提出/研究 **metrics capturing incorrect acceptance**；We introduce metrics capturing incorrect acceptance, incorrect rejection, and strong-verification frequency.
3. 机制：Externally, users inspect outputs and steer the model through feedback until results are trustworthy, which we call **strong verification**.
4. 结果：Experiments on mathematical reasoning and sequential decision-making demonstrate that our algorithm achieves reliability comparable to exhaustive strong verification while significantly reducing verification…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[When to Trust the Cheap Check: Weak and Strong Verification for Reasoning](https://openreview.net/forum?id=dfN4HMZbc9)

## 486. [Oral] Which Algorithms Can Graph Neural Networks Learn?

1. 问题：However, much existing work is either largely empirical and lacks formal guarantees or it focuses solely on expressivity, leaving open the question…
2. 方法：提出/研究 **general theoretical framework that characterizes sufficient conditions**；In this work, we propose a general theoretical framework that characterizes sufficient conditions under which MPNNs can learn an algorithm…
3. 机制：In this work, we propose a general theoretical framework that characterizes sufficient conditions under which MPNNs can learn an algorithm from a…
4. 理论/证据：However, much existing work is either largely empirical and lacks formal guarantees or it focuses solely on expressivity, leaving open…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[Which Algorithms Can Graph Neural Networks Learn?](https://openreview.net/forum?id=GnmuZIlvxw)

## 487. [Spotlight] Why Deep Jacobian Spectra Separate: Depth-Induced Scaling and Singular-Vector Alignment

1. 问题：Understanding why gradient-based training in deep networks exhibits strong implicit bias remains challenging, in part because tractable singular-value dynamics are typically available…
2. 方法：提出/研究 **n alternative route based on two theoretically grounded and empiricall**；We propose an alternative route based on two theoretically grounded and empirically testable signatures of deep Jacobians: depth-induced exponential scaling…
3. 机制：We propose an alternative route based on two theoretically grounded and empirically testable signatures of deep Jacobians: depth-induced exponential scaling of ordered…
4. 结果：Experiments in fixed-gates settings validate the predicted scaling, alignment, and resulting dynamics, supporting a mechanistic account of emergent low-rank Jacobian structure as…
5. 启示：显式利用连续时间、物理结构或谱结构，通常比无结构序列拟合更稳定、更可外推。

论文页面：[Why Deep Jacobian Spectra Separate: Depth-Induced Scaling and Singular-Vector Alignment](https://openreview.net/forum?id=2kSBDoP1rE)

## 488. [Spotlight] Why Linear Recurrent Memory Works in Partially Observable Reinforcement Learning

1. 问题：The family of linear recurrent neural networks has shown strong performance as recurrent memory units in partially observable reinforcement learning.
2. 方法：提出/研究 **Why Linear Recurrent Memory Works in Partially Observable…**；We provide a theoretical justification for their empirical effectiveness by constructing and studying two linear filters: (i) the first exactly…
3. 机制：We illustrate our main results through numerical experiments and further show that the constructed linear filter serves as a strong feature extractor…
4. 结果：We illustrate our main results through numerical experiments and further show that the constructed linear filter serves as a strong feature extractor…
5. 启示：更细粒度的探索、价值估计、约束或信用分配，是提升策略稳定性与样本效率的关键。

论文页面：[Why Linear Recurrent Memory Works in Partially Observable Reinforcement Learning](https://openreview.net/forum?id=ywjHJIkUgW)

## 489. [Spotlight] World-Model Inspired Emotion-aware Token Refinement for Training-Free Multimodal Emotion Recognition

1. 问题：Multimodal Large Language Models (MLLMs) show promise for Multimodal Emotion Recognition (MER) but often remain unreliable because sparse emotional cues could be…
2. 方法：提出/研究 **WETR**；Based on this insight, we propose WETR (World-Model inspired Emotion-aware Token Refinement), a training-free, plug-and-play regulator that reshapes token usage…
3. 机制：Based on this insight, we propose WETR (World-Model inspired Emotion-aware Token Refinement), a training-free, plug-and-play regulator that reshapes token usage through two…
4. 结果：Experiments on multiple MER benchmarks demonstrate that WETR consistently improves accuracy and stability under frozen parameters, which also improves token-level…
5. 启示：LLM 的能力、效率与可靠性可通过内部表示、推理过程和训练分布的结构化干预来改善。

论文页面：[World-Model Inspired Emotion-aware Token Refinement for Training-Free Multimodal Emotion Recognition](https://openreview.net/forum?id=ViQO8FlRFR)

## 490. [Oral] XR-1: Towards Versatile Vision-Language-Action Models via Learning Unified Vision-Motion Representations

1. 问题：However, existing VLA models still face two fundamental challenges: (i) producing precise low-level actions from high-dimensional observations, (ii) bridging domain gaps across…
2. 方法：提出/研究 **XR-1**；In this work, we present XR-1, a novel framework for versatile and scalable VLA learning across diverse robots, tasks, and…
3. 机制：At its core, XR-1 introduces the Unified Vision-Motion Codes (UVMC), a discrete latent representation learned via a dual-branch VQ-VAE that jointly encodes…
4. 结果：XR-1 consistently outperforms state-of-the-art baselines such as _0 and GR00T-N1.5 while demonstrating strong generalization to novel objects, background variations, distractors…
5. 启示：机器人泛化越来越依赖统一的视觉—状态—动作表示，以及分层或闭环的执行机制。

论文页面：[XR-1: Towards Versatile Vision-Language-Action Models via Learning Unified Vision-Motion Representations](https://openreview.net/forum?id=JO0IsGJg16)
