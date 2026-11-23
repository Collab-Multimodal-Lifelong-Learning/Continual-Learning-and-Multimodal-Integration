# Continual Learning and Multimodal Integration

**Research on continual learning models and multimodal integration for sustainable lifelong learning.**

This repository is part of [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning), associated with the research project **Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework**. It collects research on general-purpose continual learning methods, scalable memory and pre-trained models, efficient knowledge adaptation, and the integration of multimodal experience for reasoning and action.

Browse the [24 research projects](#code-and-resources) for source code and documentation.

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

## Representative Research and Publications

The following publications are highlighted in the project's July 15, 2026 progress evaluation.

### Expandable Memory and Knowledge Preservation

- **[Continual Learning by Contrastive Learning of Regularized Classes in Multivariate Gaussian Distributions](https://pubmed.ncbi.nlm.nih.gov/40186335/)** — *International Journal of Neural Systems, 2025*.
  - Stores class-wise statistical representations and uses contrastive learning and regularization to retain previous knowledge during class-incremental updates.

- **[Expandable and Differentiable Dual Memories with Orthogonal Regularization for Exemplar-free Continual Learning](https://ojs.aaai.org/index.php/AAAI/article/view/39626)** — *AAAI, 2026*.
  - Combines differentiable shared and task-specific memories, adaptive capacity expansion, and orthogonal regularization for exemplar-free continual learning.

### Continual Learning, Adaptation, and Decision-Making

- **[Prevalence of Negative Transfer in Continual Reinforcement Learning: Analyses and a Simple Baseline](https://proceedings.iclr.cc/paper_files/paper/2025/hash/ba9e3d60610f3525717665966d86e0cd-Abstract-Conference.html)** — *ICLR, 2025*.
  - Analyzes negative transfer across sequential reinforcement-learning tasks and introduces a reset-and-distill baseline.
  - [Reset-Distill code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/Reset-Distill/blob/0fa3158f6f0f41631a57e27b6c3243cffe74f957/README.md)

- **[Forget Forgetting: Continual Learning in a World of Abundant Memory](https://proceedings.iclr.cc/paper_files/paper/2026/hash/17fc58b1ba92abbb72c5f457e140d851-Abstract-Conference.html)** — *ICLR, 2026*.
  - Reexamines continual learning when memory is relatively abundant and emphasizes the ability to acquire new tasks efficiently.

- **[DoMIX: An Efficient Framework for Exploiting Domain Knowledge in Fine-Tuning](https://aclanthology.org/2025.acl-long.710/)** — *ACL, 2025*.
  - Uses modular LoRA-based adaptation to accumulate domain knowledge efficiently and reuse it for downstream tasks.
  - [DoMIX code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/DoMIX/blob/35b437f57b242b9fc81721613d94f2fea09c66ea/README.md)

- **[PRISP: Privacy-Safe Few-Shot Personalization via Lightweight Adaptation](https://aclanthology.org/2026.acl-long.1146/)** — *ACL, 2026*.
  - Studies privacy-conscious, resource-efficient personalization with a limited amount of user data.
  - [PRISP code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/PRISP/blob/7ad2e7f6ff040d7aeecfb02cc2d1d7ae35c2663b/README.md)

- **[Option-aware Temporally Abstracted Value for Offline Goal-Conditioned Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2025/hash/90080022263cddafddd4a0726f1fb186-Abstract-Conference.html)** — *NeurIPS, 2025*.
  - Uses option-aware temporal abstraction for value learning in long-horizon offline decision-making.
  - [OTA-V code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/ota-v/blob/38bc596c7bff21e4d2dbf05f2f197f03622ab544/README.md)

- **[Action-Sufficient Goal Representations](https://proceedings.mlr.press/v306/hyeon26a.html)** — *ICML, 2026*.
  - Distinguishes goal representations sufficient for action selection from representations sufficient only for value estimation.
  - [Project code and setup](https://github.com/Collab-Multimodal-Lifelong-Learning/action-sufficient/blob/cb70862302674fdd2ed299ad0d5e57950d10f544/README.md)

### Multimodal Knowledge Selection and Collaborative Adaptation

- **[Budgeted Online Continual Learning by Adaptive Layer Freezing and Frequency-based Sampling](https://proceedings.iclr.cc/paper_files/paper/2025/hash/760564ebba4797d0dcf1678e96e8cbcb-Abstract-Conference.html)** — *ICLR, 2025*.
  - Considers total compute and memory budgets and selectively updates model layers and replay samples for efficient online learning.

- **[Co-LoRA: Collaborative Model Personalization on Heterogeneous Multi-Modal Clients](https://proceedings.iclr.cc/paper_files/paper/2026/hash/1baeb4973da3e78e523024030ea81cf5-Abstract-Conference.html)** — *ICLR, 2026*.
  - Supports collaborative personalization and knowledge sharing across clients with heterogeneous data and model architectures.

- **[OASIS: Online Sample Selection for Continual Instruction Tuning](https://aclanthology.org/2026.acl-long.158/)** — *ACL, 2026*.
  - Selects informative streaming instruction samples to reduce redundant training while retaining adaptation performance.
  - [OASIS code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/oasis/blob/96e67e159397b851c4cc80cae559cef00370a8cf/README.md)

### Multimodal Planning and Embodied Adaptation

- **[Multi-Modal Grounded Planning and Efficient Replanning for Learning Embodied Agents with a Few Examples](https://doi.org/10.1609/aaai.v39i4.32455)** — *AAAI, 2025 (Oral)*.
  - Grounds planning in both language instructions and visual environmental observations, with adaptive replanning when execution conditions change.

- **[SCALE: Self-uncertainty Conditioned Adaptive Looking and Execution for Vision-Language-Action Models](https://proceedings.mlr.press/v306/choi26a.html)** — *ICML, 2026*.
  - Uses self-uncertainty to adapt perception and execution of vision–language–action models without additional training.
  - [SCALE code and documentation](https://github.com/Collab-Multimodal-Lifelong-Learning/scale/blob/b4ad2a69d14f91712704711e810cf9830e2b7121/README.md)

## Evaluation Highlights

The following figures are **project-reported results** from the **July 15, 2026 progress evaluation**. They are not independently reproduced results from this repository. Since the measures refer to different tasks and experimental settings, they should not be compared as scores on a common benchmark.

| Research / evaluation item | Evaluation setting | Reported target | Project-reported result |
| --- | --- | ---: | ---: |
| Class-incremental learning | CIFAR-100, 10 tasks; average accuracy after the final task (Sung-Bae Cho team) | ≥77% | **80.4%** |
| Embodied-agent instruction following | ALFRED, unseen-domain success rate; five trials (Jonghyun Choi team) | ≥25% | **28.87%** |

The project also studies average accuracy and forgetting in continual learning, computational and storage budgets, and the effectiveness of multimodal knowledge transfer and adaptive decision-making. The exact benchmarks and evaluation protocols depend on the associated study.

## Code and Resources

Each project is a Git submodule pinned to a commit in its organization fork. The table links to that revision's README and lists both the fork and its upstream repository.

Clone this repository and its project folders with:

```bash
git clone --recurse-submodules --shallow-submodules https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-and-Multimodal-Integration.git
```

In an existing checkout, run `git submodule update --init --recursive --depth 1`.

| Project README | Research focus | Repositories |
| --- | --- | --- |
| [ask4help](https://github.com/Collab-Multimodal-Lifelong-Learning/ask4help/blob/1a38de50faf63cb52cff0ec8f04bdda2c5eca8d6/README.md) | Learning when an embodied agent should request expert assistance. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/ask4help) · [Upstream](https://github.com/allenai/ask4help) |
| [cmota](https://github.com/Collab-Multimodal-Lifelong-Learning/cmota/blob/781528d12e8aceca0ae6e8e3527e069582138027/README.md) | Story visualization using context memory and online text augmentation. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/cmota) · [Upstream](https://github.com/yonseivnl/cmota) |
| [sdp](https://github.com/Collab-Multimodal-Lifelong-Learning/sdp/blob/c4a0666793c248ca1d2b9fbac804de5fd8c78222/README.md) | Online continual learning without explicit task boundaries. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/sdp) · [Upstream](https://github.com/yonseivnl/sdp) |
| [mcr-agent](https://github.com/Collab-Multimodal-Lifelong-Learning/mcr-agent/blob/c6b527c563ec7141adbcd618c6498e0ee1b2e93b/README.md) | Multi-level compositional reasoning for embodied instruction following. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/mcr-agent) · [Upstream](https://github.com/yonseivnl/mcr-agent) |
| [HLE](https://github.com/Collab-Multimodal-Lifelong-Learning/HLE/blob/3126cb37bbc6851843f09fc6cdf1128d3c5f786e/README.md) | Online continual learning as coarse labels expand into finer categories. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/HLE) · [Upstream](https://github.com/Hyun1A/HLE) |
| [earl](https://github.com/Collab-Multimodal-Lifelong-Learning/earl/blob/b3f0c7a8205d87e5fb28265b036b1269d145d930/README.md) | Experimental code for online continual learning. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/earl) · [Upstream](https://github.com/yonseivnl/earl) |
| [cl-alfred](https://github.com/Collab-Multimodal-Lifelong-Learning/cl-alfred/blob/7477ad3b72a6fcdf7789d68695db5b4b519c07d8/README.md) | Continual instruction following across new behaviors and environments in ALFRED. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/cl-alfred) · [Upstream](https://github.com/snumprlab/cl-alfred) |
| [vlm-rlaif](https://github.com/Collab-Multimodal-Lifelong-Learning/vlm-rlaif/blob/610cac72c16ae3862b0d83a0dc3708d73a42a4cc/README.md) | Video-language model alignment through reinforcement learning from AI feedback. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/vlm-rlaif) · [Upstream](https://github.com/yonseivnl/vlm-rlaif) |
| [prometheus-vision](https://github.com/Collab-Multimodal-Lifelong-Learning/prometheus-vision/blob/fe668b5e7e120e5bea8a3821eeb468ddf719c23c/README.md) | Rubric-based evaluation of vision-language models. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/prometheus-vision) · [Upstream](https://github.com/prometheus-eval/prometheus-vision) |
| [BGS](https://github.com/Collab-Multimodal-Lifelong-Learning/BGS/blob/3e79e59a64cbabaad8c9c55dad037bce7b651df6/README.md) | Continual learning in the presence of spurious correlations. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/BGS) · [Upstream](https://github.com/DQle38/BGS) |
| [LiRE](https://github.com/Collab-Multimodal-Lifelong-Learning/LiRE/blob/7af7697fe7b8e58edcd5e4438a78b49135d37e8c/README.md) | Listwise reward estimation for offline preference-based reinforcement learning. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/LiRE) · [Upstream](https://github.com/chwoong/LiRE) |
| [oasis](https://github.com/Collab-Multimodal-Lifelong-Learning/oasis/blob/96e67e159397b851c4cc80cae559cef00370a8cf/README.md) | Online sample selection for continual instruction tuning of language and vision-language models. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/oasis) · [Upstream](https://github.com/snumprlab/oasis) |
| [DoMIX](https://github.com/Collab-Multimodal-Lifelong-Learning/DoMIX/blob/35b437f57b242b9fc81721613d94f2fea09c66ea/README.md) | Efficient fine-tuning with domain-specific LoRA components. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/DoMIX) · [Upstream](https://github.com/dohoonkim-ai/DoMIX) |
| [Reset-Distill](https://github.com/Collab-Multimodal-Lifelong-Learning/Reset-Distill/blob/0fa3158f6f0f41631a57e27b6c3243cffe74f957/README.md) | Measuring and mitigating negative transfer in continual reinforcement learning. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/Reset-Distill) · [Upstream](https://github.com/hongjoon0805/Reset-Distill/tree/main) |
| [ota-v](https://github.com/Collab-Multimodal-Lifelong-Learning/ota-v/blob/38bc596c7bff21e4d2dbf05f2f197f03622ab544/README.md) | Option-aware value learning for long-horizon offline goal-conditioned reinforcement learning. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/ota-v) · [Upstream](https://github.com/ota-v/ota-v) |
| [agf](https://github.com/Collab-Multimodal-Lifelong-Learning/agf/blob/25e8424b8b2cd38df73e261b8611aa185fda4c58/README.md) | Self-attention for linear transformers in the singular-value domain. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/agf) · [Upstream](https://github.com/hyowonwi/agf) |
| [MASS](https://github.com/Collab-Multimodal-Lifelong-Learning/MASS/blob/145b0f8c118913f65dbe31bfb8b4b93f99153259/README.md) | Adaptive expert expansion for language and vision tasks. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/MASS) · [Upstream](https://github.com/psmiz/MASS) |
| [binder](https://github.com/Collab-Multimodal-Lifelong-Learning/binder/blob/43f850995bf669c481902f670bbdc2b8da646bed/README.md) | Adaptive mobile manipulation with open-vocabulary commands. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/binder) · [Upstream](https://github.com/snumprlab/binder) |
| [vector](https://github.com/Collab-Multimodal-Lifelong-Learning/vector/blob/d34a247ad6f6cc8996366fbe71848ab70f7ee076/README.md) | Benchmark and training method for temporal ordering of events in video. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/vector) · [Upstream](https://github.com/snumprlab/vector) |
| [dart](https://github.com/Collab-Multimodal-Lifelong-Learning/dart/blob/1b23c4f42f73168c78a20b353453145e74f64711/README.md) | One-shot vision-language-action adaptation under environmental shifts. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/dart) · [Upstream](https://github.com/snumprlab/dart) |
| [scale](https://github.com/Collab-Multimodal-Lifelong-Learning/scale/blob/b4ad2a69d14f91712704711e810cf9830e2b7121/README.md) | Uncertainty-guided visual perception and action decoding in vision-language-action models. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/scale) · [Upstream](https://github.com/snumprlab/scale) |
| [axis-lora](https://github.com/Collab-Multimodal-Lifelong-Learning/axis-lora/blob/2d795e48c20207e24c40ef3890bb3849061701f6/README.md) | Adapting embedding models for personal-memory retrieval. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/axis-lora) · [Upstream](https://github.com/dohoonkim-ai/axis-lora) |
| [action-sufficient](https://github.com/Collab-Multimodal-Lifelong-Learning/action-sufficient/blob/cb70862302674fdd2ed299ad0d5e57950d10f544/README.md) | Goal representations that preserve information needed for action selection. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/action-sufficient) · [Upstream](https://github.com/action-sufficient/action-sufficient) |
| [PRISP](https://github.com/Collab-Multimodal-Lifelong-Learning/PRISP/blob/7ad2e7f6ff040d7aeecfb02cc2d1d7ae35c2663b/README.md) | Privacy-safe few-shot personalization through lightweight adaptation. | [Fork](https://github.com/Collab-Multimodal-Lifelong-Learning/PRISP) · [Upstream](https://github.com/kingthebryan/PRISP) |

## Related Repositories

Other research areas within [Collab-Multimodal-Lifelong-Learning](https://github.com/Collab-Multimodal-Lifelong-Learning):

- [Continual-Learning-Vision-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Vision-Domain) — Continual learning for visual recognition and video understanding.
- [Continual-Learning-Language-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Language-Domain) — Continual learning and knowledge updating for language models.
- [Continual-Learning-Time-Series-Domain](https://github.com/Collab-Multimodal-Lifelong-Learning/Continual-Learning-Time-Series-Domain) — Continual learning for time-series data.
- [PDM-Framework](https://github.com/Collab-Multimodal-Lifelong-Learning/PDM-Framework) — Integrated PDM framework for sustainable collaborative multimodal continual learning.

## Acknowledgment

This research is associated with the Korean national R&D project **“Developing a Sustainable Collaborative Multi-modal Lifelong Learning Framework” (Project No. 2022-0-00113)**, within the *Human-Centered AI Core Technology Development* program, supported by the Ministry of Science and ICT (MSIT) and administered by the Institute of Information & Communications Technology Planning & Evaluation (IITP).
