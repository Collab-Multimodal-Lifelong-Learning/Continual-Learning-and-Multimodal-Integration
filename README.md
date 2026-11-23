# Continual Learning and Multimodal Integration

**Research on continual learning models and multimodal integration for sustainable lifelong learning.**

This repository is part of [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning), associated with the research project **Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework**. It collects research on general-purpose continual learning methods, scalable memory and pre-trained models, efficient knowledge adaptation, and the integration of multimodal experience for reasoning and action.

## Research list

### Continual learning and online adaptation

- **Online Boundary-Free Continual Learning by Scheduled Data Prior (SDP)** (ICLR 2023) — Hyunseo Koh et al.
  - Online continual learning without explicit task boundaries.
  - [Paper](https://openreview.net/forum?id=qco4ekz2Epm) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/sdp/blob/c917fb2b2a50b498840ba5edc810d21d65be8d16/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/sdp) · [Upstream](https://github.com/yonseivnl/sdp)

- **Online Continual Learning on Hierarchical Label Expansion (HLE)** (ICCV 2023) — Byung Hyun Lee et al.
  - Online continual learning as coarse labels expand into finer categories.
  - [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Lee_Online_Continual_Learning_on_Hierarchical_Label_Expansion_ICCV_2023_paper.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/HLE/blob/3202cee11297b48c8561c0631a8631ec1745d213/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/HLE) · [Upstream](https://github.com/Hyun1A/HLE)

- **Learning Equi-angular Representations for Online Continual Learning (EARL)** (CVPR 2024) — Minhyuk Seo et al.
  - Uses neural-collapse-inspired class representations to learn from changing data streams.
  - [Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Seo_Learning_Equi-angular_Representations_for_Online_Continual_Learning_CVPR_2024_paper.pdf) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/earl/blob/1475ca244472d32b8891cc14063842a9002a546b/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/earl) · [Upstream](https://github.com/yonseivnl/earl)

- **Continual Learning in the Presence of Spurious Correlations: Analyses and a Simple Baseline** (ICLR 2024) — Donggyu Lee, Sangwon Jung, and Taesup Moon
  - Continual learning in the presence of spurious correlations.
  - [Paper](https://openreview.net/forum?id=3Y7r6xueJJ) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/BGS/blob/871d5c11b09f3ee46c17d8ed3b94e770dfde6e06/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/BGS) · [Upstream](https://github.com/DQle38/BGS)

- **OASIS: Online Sample Selection for Continual Instruction Tuning** (ACL 2026) — Minjae Lee et al.
  - Selects informative streaming instruction samples to reduce redundant training while retaining adaptation performance.
  - [Paper](https://aclanthology.org/2026.acl-long.158/) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/oasis/blob/0f73d50f70055386a10789cf6e6f1b18597419f6/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/oasis) · [Upstream](https://github.com/snumprlab/oasis)

- **Prevalence of Negative Transfer in Continual Reinforcement Learning: Analyses and a Simple Baseline** (ICLR 2025) — Hongjoon Ahn et al.
  - Analyzes negative transfer across sequential reinforcement-learning tasks and introduces a reset-and-distill baseline.
  - [Paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/ba9e3d60610f3525717665966d86e0cd-Abstract-Conference.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/Reset-Distill/blob/5e72d08f7173a6a006c1f691f74b40d6f52f873f/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/Reset-Distill) · [Upstream](https://github.com/hongjoon0805/Reset-Distill/tree/main)

### Model adaptation and representation learning

- **DoMIX: An Efficient Framework for Exploiting Domain Knowledge in Fine-Tuning** (ACL 2025) — Dohoon Kim, Donghun Kang, and Taesup Moon
  - Uses modular LoRA-based adaptation to accumulate domain knowledge efficiently and reuse it for downstream tasks.
  - [Paper](https://aclanthology.org/2025.acl-long.710/) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/DoMIX/blob/09069aa727d88a87cf98c773799156ea739feea5/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/DoMIX) · [Upstream](https://github.com/dohoonkim-ai/DoMIX)

- **Learning Advanced Self-Attention for Linear Transformers in the Singular Value Domain (AGF)** (IJCAI 2025) — Hyowon Wi, Jeongwhan Choi, and Noseong Park
  - Self-attention for linear transformers in the singular-value domain.
  - [Paper](https://arxiv.org/abs/2505.08516) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/agf/blob/0ca7b2774d1eece35987b99bd7b67fce692326ad/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/agf) · [Upstream](https://github.com/hyowonwi/agf)

- **How Many Experts Are Enough? Towards Optimal Semantic Specialization for Mixture-of-Experts (MASS)** (AAAI 2026) — Sumin Park and Noseong Park
  - Adaptive expert expansion for language and vision tasks.
  - [Paper](https://arxiv.org/abs/2512.19765) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/MASS/blob/3cca7483fa14311d38906f212fcc2cebc00ae567/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/MASS) · [Upstream](https://github.com/psmiz/MASS)

- **Axis-LoRA: Probing and Adapting Embedding Models for Personal-Memory Retrieval** (EMNLP 2026) — Dohoon Kim et al.
  - Adapting embedding models for personal-memory retrieval.
  - [Paper](https://aclanthology.org/2026.emnlp-main.542/) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/axis-lora/blob/2dec422685355c3d0d5ec220ae52925e1dd359c8/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/axis-lora) · [Upstream](https://github.com/dohoonkim-ai/axis-lora)

- **PRISP: Privacy-Safe Few-Shot Personalization via Lightweight Adaptation** (ACL 2026 (Oral)) — Junho Park et al.
  - Studies privacy-conscious, resource-efficient personalization with a limited amount of user data.
  - [Paper](https://aclanthology.org/2026.acl-long.1146/) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/PRISP/blob/5ce9208f8010e8e90002c9ca20d942707cdde1df/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/PRISP) · [Upstream](https://github.com/kingthebryan/PRISP)

### Vision-language learning and evaluation

- **Story Visualization by Online Text Augmentation with Context Memory (CMOTA)** (ICCV 2023) — Daechul Ahn et al.
  - Story visualization using context memory and online text augmentation.
  - [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Ahn_Story_Visualization_by_Online_Text_Augmentation_with_Context_Memory_ICCV_2023_paper.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/cmota/blob/53f575654d19b910d70105cae25a459405277c08/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/cmota) · [Upstream](https://github.com/yonseivnl/cmota)

- **Tuning Large Multimodal Models for Videos using Reinforcement Learning from AI Feedback (VLM-RLAIF)** (ACL 2024) — Daechul Ahn et al.
  - Video-language model alignment through reinforcement learning from AI feedback.
  - [Paper](https://arxiv.org/abs/2402.03746) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/vlm-rlaif/blob/d5f6b830832182d83ff6b2b2556821a0df2c0ba9/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/vlm-rlaif) · [Upstream](https://github.com/yonseivnl/vlm-rlaif)

- **Prometheus-Vision: Vision-Language Model as a Judge for Fine-Grained Evaluation** (Findings of ACL 2024) — Seongyun Lee et al.
  - Rubric-based evaluation of vision-language models.
  - [Paper](https://arxiv.org/abs/2401.06591) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/prometheus-vision/blob/4a3489cb59e758f32e24e69058218a203e8a1ceb/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/prometheus-vision) · [Upstream](https://github.com/prometheus-eval/prometheus-vision)

- **What Happens When: Learning Temporal Orders of Events in Videos (VECTOR)** (WACV 2026) — Daechul Ahn et al.
  - Benchmark and training method for temporal ordering of events in video.
  - [Paper](https://arxiv.org/abs/2512.08979) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/vector/blob/2d7e7a4a8614aeda620cd55049bf986f1e30c7ac/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/vector) · [Upstream](https://github.com/snumprlab/vector)

### Embodied agents and reinforcement learning

- **Ask4Help: Learning to Leverage an Expert for Embodied Tasks** (NeurIPS 2022) — Kunal Pratap Singh et al.
  - Learning when an embodied agent should request expert assistance.
  - [Paper](https://arxiv.org/abs/2211.09960) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/ask4help/blob/45783e6eb05cd77d710997bcc7a65708790cf19d/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/ask4help) · [Upstream](https://github.com/allenai/ask4help)

- **Multi-Level Compositional Reasoning for Interactive Instruction Following (MCR-Agent)** (AAAI 2023) — Suvaansh Bhambri, Byeonghwi Kim, and Jonghyun Choi
  - Multi-level compositional reasoning for embodied instruction following.
  - [Paper](https://arxiv.org/abs/2308.09387) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/mcr-agent/blob/8727f7d8233844ff0ad90aaa35f5957ed6da2d5f/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/mcr-agent) · [Upstream](https://github.com/yonseivnl/mcr-agent)

- **Online Continual Learning for Interactive Instruction Following Agents (CL-ALFRED)** (ICLR 2024) — Byeonghwi Kim, Minhyuk Seo, and Jonghyun Choi
  - Evaluates continual instruction following as agents encounter new behaviors and environments in ALFRED.
  - [Paper](https://arxiv.org/abs/2403.07548) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/cl-alfred/blob/ef7d6128471c15d1f54fe037313f17ef733c059f/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/cl-alfred) · [Upstream](https://github.com/snumprlab/cl-alfred)

- **Listwise Reward Estimation for Offline Preference-based Reinforcement Learning (LiRE)** (ICML 2024) — Heewoong Choi, Sangwon Jung, Hongjoon Ahn, and Taesup Moon
  - Builds ranked trajectory lists from pairwise preference feedback to estimate rewards for offline reinforcement learning.
  - [Paper](https://proceedings.mlr.press/v235/choi24b.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/LiRE/blob/f7c0f55e0ba2ca6f421f9724d1e477dcf6462edf/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/LiRE) · [Upstream](https://github.com/chwoong/LiRE)

- **Option-aware Temporally Abstracted Value for Offline Goal-Conditioned Reinforcement Learning (OTA-V)** (NeurIPS 2025) — Hongjoon Ahn et al.
  - Uses option-aware temporal abstraction for value learning in long-horizon offline decision-making.
  - [Paper](https://proceedings.neurips.cc/paper_files/paper/2025/hash/90080022263cddafddd4a0726f1fb186-Abstract-Conference.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/ota-v/blob/8b26e0fae3b9dfb2baabb09dd8fe7069b5b9eda9/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/ota-v) · [Upstream](https://github.com/ota-v/ota-v)

- **BINDER: Instantly Adaptive Mobile Manipulation with Open-Vocabulary Commands** (ICRA 2026) — Seongwon Cho et al.
  - Pairs continuous video monitoring with task planning so mobile robots can replan as their surroundings change.
  - [Paper](https://arxiv.org/abs/2511.22364) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/binder/blob/d8eadf1730efe90c2dace180403d23ddfecd8fef/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/binder) · [Upstream](https://github.com/snumprlab/binder)

- **Domain Arithmetic: One-Shot VLA Adaptation under Environmental Shifts (DART)** (ECCV 2026) — Taewook Kang et al.
  - One-shot vision-language-action adaptation under environmental shifts.
  - [Paper](https://arxiv.org/abs/2607.00666) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/dart/blob/92052605b0561a98b76edac0a8ca9d0a0a12c917/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/dart) · [Upstream](https://github.com/snumprlab/dart)

- **SCALE: Self-uncertainty Conditioned Adaptive Looking and Execution for Vision-Language-Action Models** (ICML 2026 (Spotlight)) — Hyeonbeom Choi et al.
  - Uses self-uncertainty to adapt perception and execution of vision–language–action models without additional training.
  - [Paper](https://proceedings.mlr.press/v306/choi26a.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/scale/blob/60474a0996939ee56569df0455b2628446eb51a4/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/scale) · [Upstream](https://github.com/snumprlab/scale)

- **Action-Sufficient Goal Representations** (ICML 2026) — Jinu Hyeon et al.
  - Distinguishes goal representations sufficient for action selection from representations sufficient only for value estimation.
  - [Paper](https://proceedings.mlr.press/v306/hyeon26a.html) · [Project code](https://github.com/Collab-Multimodal-Lifelong-Learning/action-sufficient/blob/1e1dfeadaefc6a32a94e155c83fc11b53bf2cd9a/README.md) · [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/action-sufficient) · [Upstream](https://github.com/action-sufficient/action-sufficient)

### Additional project research

The following publications are highlighted in the project's July 15, 2026 progress evaluation.

#### Expandable Memory and Knowledge Preservation

- **[Continual Learning by Contrastive Learning of Regularized Classes in Multivariate Gaussian Distributions](https://pubmed.ncbi.nlm.nih.gov/40186335/)** — *International Journal of Neural Systems, 2025*.
  - Stores class-wise statistical representations and uses contrastive learning and regularization to retain previous knowledge during class-incremental updates.

- **[Expandable and Differentiable Dual Memories with Orthogonal Regularization for Exemplar-free Continual Learning](https://ojs.aaai.org/index.php/AAAI/article/view/39626)** — *AAAI, 2026*.
  - Combines differentiable shared and task-specific memories, adaptive capacity expansion, and orthogonal regularization for exemplar-free continual learning.

#### Continual Learning, Adaptation, and Decision-Making

- **[Forget Forgetting: Continual Learning in a World of Abundant Memory](https://proceedings.iclr.cc/paper_files/paper/2026/hash/17fc58b1ba92abbb72c5f457e140d851-Abstract-Conference.html)** — *ICLR, 2026*.
  - Reexamines continual learning when memory is relatively abundant and emphasizes the ability to acquire new tasks efficiently.

#### Multimodal Knowledge Selection and Collaborative Adaptation

- **[Budgeted Online Continual Learning by Adaptive Layer Freezing and Frequency-based Sampling](https://proceedings.iclr.cc/paper_files/paper/2025/hash/760564ebba4797d0dcf1678e96e8cbcb-Abstract-Conference.html)** — *ICLR, 2025*.
  - Considers total compute and memory budgets and selectively updates model layers and replay samples for efficient online learning.

- **[Co-LoRA: Collaborative Model Personalization on Heterogeneous Multi-Modal Clients](https://proceedings.iclr.cc/paper_files/paper/2026/hash/1baeb4973da3e78e523024030ea81cf5-Abstract-Conference.html)** — *ICLR, 2026*.
  - Supports collaborative personalization and knowledge sharing across clients with heterogeneous data and model architectures.

#### Multimodal Planning and Embodied Adaptation

- **[Multi-Modal Grounded Planning and Efficient Replanning for Learning Embodied Agents with a Few Examples](https://doi.org/10.1609/aaai.v39i4.32455)** — *AAAI, 2025 (Oral)*.
  - Grounds planning in both language instructions and visual environmental observations, with adaptive replanning when execution conditions change.

## Research Overview

Real-world AI systems encounter new tasks, domains, and modalities over time. To support lifelong learning, they need to **acquire new knowledge without unnecessarily discarding previous knowledge**, **adapt with limited computation and memory**, and **combine experiences from different data sources**.

Within the project's **PDM (Pre-trained, Data, Memory)** perspective, this repository focuses primarily on the **pre-trained-model and memory-based learning methods** and the **cross-modal knowledge integration** that complement the vision, language, and time-series domain repositories. Integrated framework-level implementations are addressed separately by the [PDM-Framework](https://github.com/Collab-Multimodal-Lifelong-Learning/PDM-Framework) repository.

The principal research directions are:

1. **Expandable Memory and Knowledge Preservation:** Compactly store, retrieve, and expand knowledge as new tasks arrive.
2. **Pre-trained Models and Knowledge Integration:** Reuse pre-trained representations and integrate knowledge across models and modalities.
3. **Efficient Continual Learning and Decision-Making:** Study forgetting, plasticity, negative transfer, resource-constrained adaptation, and long-horizon decisions.
4. **Continual Multimodal Learning and Personalization:** Select, update, and share knowledge from evolving vision–language–action experiences for adaptive agents.

## Research Directions

### 1. Expandable Memory and Knowledge Preservation

**Research focus:** Scalable memory structures and compact representations for class- and task-incremental learning.

- Represent previously learned classes with compact feature statistics, including class-specific multivariate Gaussian distributions, rather than retaining all raw examples.
- Preserve and recover earlier knowledge through representation regularization, contrastive learning, and memory-based reconstruction.
- Learn **expandable, differentiable dual memories** that separate shared features from task-specific knowledge and reduce interference across tasks.
- Investigate distributed external memory, prototype-based compression, and selective preservation of informative representations.

**Research team:** Prof. Sung-Bae Cho, Yonsei University.

### 2. Pre-trained Models and Knowledge Integration

**Research focus:** Incrementally extending pre-trained knowledge and integrating information from multiple models and modalities.

- Adapt pre-trained representations when new classes, domains, or uncertain inputs appear.
- Explore knowledge transfer and distillation to consolidate previous and newly acquired information.
- Combine knowledge from multiple language models and external sources while examining consistency and relevance.
- Investigate visual–language knowledge retrieval, reasoning, and selective use of previously acquired information.

**Research team:** Prof. Sung-Bae Cho, Yonsei University.

### 3. Efficient Continual Learning and Long-Horizon Decision-Making

**Research focus:** Understanding the practical bottlenecks of continual learning and reusing accumulated knowledge for future decisions.

- Revisit the **stability–plasticity trade-off** under realistic memory and computation budgets, including settings where learning new tasks is a greater bottleneck than storing past examples.
- Analyze and mitigate **negative transfer** between sequential tasks in continual reinforcement learning.
- Study parameter-efficient adaptation and domain knowledge reuse with modular **LoRA** methods, as well as privacy-aware few-shot personalization.
- Learn reusable value functions and **action-sufficient goal representations** for long-horizon, offline goal-conditioned reinforcement learning.

**Research team:** Prof. Taesup Moon, Seoul National University.

### 4. Continual Multimodal Learning and Adaptive Agents

**Research focus:** Building, selecting, and updating useful multimodal knowledge from streaming experiences.

- Discover meaningful events, temporal relationships, and visually grounded knowledge from continuous **vision–language–action** observations.
- Adapt with limited FLOPs, memory, or labeled instruction data through selective layer updates and informative-sample selection.
- Share and personalize knowledge across **heterogeneous multimodal clients and model architectures**.
- Connect accumulated multimodal knowledge to embodied-agent **planning**, **replanning**, perception, and adaptive action in changing environments.

**Research team:** Prof. Jonghyun Choi, Seoul National University.

## Evaluation Highlights

The following figures are **project-reported results** from the **July 15, 2026 progress evaluation**. They are not independently reproduced results from this repository. Since the measures refer to different tasks and experimental settings, they should not be compared as scores on a common benchmark.

| Research / evaluation item | Evaluation setting | Reported target | Project-reported result |
| --- | --- | ---: | ---: |
| Class-incremental learning | CIFAR-100, 10 tasks; average accuracy after the final task (Sung-Bae Cho team) | ≥77% | **80.4%** |
| Embodied-agent instruction following | ALFRED, unseen-domain success rate; five trials (Jonghyun Choi team) | ≥25% | **28.87%** |

The project also studies average accuracy and forgetting in continual learning, computational and storage budgets, and the effectiveness of multimodal knowledge transfer and adaptive decision-making. The exact benchmarks and evaluation protocols depend on the associated study.

## Code and Resources

Each Project code link opens the README at the pinned commit in the organization fork. The corresponding submodule uses the same revision. Open the upstream repository for the original source.

Clone this repository and its project folders with:

```bash
git clone --recurse-submodules --shallow-submodules https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-and-Multimodal-Integration.git
```

In an existing checkout, run `git submodule update --init --recursive --depth 1`.

## Related Repositories

Other research areas within [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning):

- [Continual-Learning-Vision-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Vision-Domain) — Continual learning for visual recognition and video understanding.
- [Continual-Learning-Language-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Language-Domain) — Continual learning and knowledge updating for language models.
- [Continual-Learning-Time-Series-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Time-Series-Domain) — Continual learning for time-series data.
- [PDM-Framework](https://github.com/Collab-Multimodal-Lifelong-Learning/PDM-Framework) — Integrated PDM framework for sustainable collaborative multimodal continual learning.

## Acknowledgment

This research is associated with the Korean national R&D project **“Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework” (Project No. 2022-0-00113)**, conducted within the *Human-Centered AI Core Technology Development* program, supported by the Ministry of Science and ICT (MSIT) and administered by the Institute of Information & Communications Technology Planning & Evaluation (IITP).
