## A Survey on Knowledge Distillation of Vision-Language Models

In this paper, we present the first dedicated survey of knowledge distillation for vision-language models. We propose a unified taxonomy that organizes methods along three orthogonal views: **knowledge type**, **teacher accessibility**, and **structural compatibility**, and use it to organize methods across major VLM distillation settings.

## 📊 Taxonomy

Below is the taxonomy summarizing the landscape of knowledge distillation research for VLMs:

## 📚 Table of Contents

- [Awesome-KD-VLMs](#awesome-kd-vlms)
  - [\[EMNLP 2026\] A Survey on Knowledge Distillation of Vision-Language Models](#emnlp-2026-a-survey-on-knowledge-distillation-of-vision-language-models)
  - [📊 Taxonomy](#-taxonomy)
  - [Section I: Response-based Distillation](#section-i-response-based-distillation)
  - [Section II: Feature-based Distillation](#section-ii-feature-based-distillation)
  - [Section III: Relation-based Distillation](#section-iii-relation-based-distillation)
  - [Section IV: White-box Distillation](#section-iv-white-box-distillation)
  - [Section V: Black-box Distillation](#section-v-black-box-distillation)
  - [Section VI: Self-Distillation](#section-vi-self-distillation)
  - [Section VII: Multi-teacher Distillation](#section-vii-multi-teacher-distillation)
  - [Section VIII: Structural Compatibility - Isomorphic](#section-viii-structural-compatibility---isomorphic)
  - [Section IX: Structural Compatibility - Cross-Architecture](#section-ix-structural-compatibility---cross-architecture)
  - [Section X: Structural Compatibility - Cross-Modal](#section-x-structural-compatibility---cross-modal)
  - [Knowledge Distillation for Vision-Language-Action Models](#knowledge-distillation-for-vision-language-action-models)
  - [Knowledge Distillation for Vision-Language Embedding Models](#knowledge-distillation-for-vision-language-embedding-models)
  - [VLM Knowledge Distillation for Segmentation](#vlm-knowledge-distillation-for-segmentation)
  - [VLM Knowledge Distillation for Open-Vocabulary Object Detection](#vlm-knowledge-distillation-for-open-vocabulary-object-detection)
  - [Citation](#citation)


## Section I: Response-based Distillation

**Logit Distillation**

* LLaVA-KD: A Framework of Distilling Multimodal Large Language Models [[Paper]](https://www.semanticscholar.org/search?q=Llava-kd%3A%20A%20framework%20of%20distilling%20multimodal%20large%20language%20models) ![](https://img.shields.io/badge/year-2025-red)
* MASSV: Multimodal Adaptation and Self-Data Distillation for Speculative Decoding of Vision-Language Models [[Paper]](https://arxiv.org/abs/2505.10526) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:274437419) ![](https://img.shields.io/badge/year-2024-red)
* GenRecal: Generation after Recalibration from Large to Small Vision-Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:279447364) ![](https://img.shields.io/badge/year-2025-red)
* EM-KD: Distilling Efficient Multimodal Large Language Model with Unbalanced Vision Tokens [[Paper]](https://api.semanticscholar.org/CorpusID:283262068) ![](https://img.shields.io/badge/year-2025-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/search?q=Promptkd%3A%20Unsupervised%20prompt%20distillation%20for%20vision-language%20models) ![](https://img.shields.io/badge/year-2024-red)
* Improving Zero-Shot Generalization of Learned Prompts via Unsupervised Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Improving%20zero-shot%20generalization%20of%20learned%20prompts%20via%20unsupervised%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-KD: An Empirical Study of CLIP Model Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:260125303) ![](https://img.shields.io/badge/year-2023-red)
* AMMKD: Adaptive Multimodal Multi-Teacher Distillation for Lightweight Vision-Language Models [[Paper]](https://arxiv.org/abs/2509.00039) ![](https://img.shields.io/badge/year-2025-red)
* VL2Lite: Task-Specific Knowledge Distillation from Large Vision-Language Models to Lightweight Networks [[Paper]](https://doi.org/10.1109/CVPR52734.2025.02799) ![](https://img.shields.io/badge/year-2025-red)
* VLM-KD: Knowledge Distillation from VLM for Long-Tail Visual Recognition [[Paper]](https://api.semanticscholar.org/CorpusID:272310206) ![](https://img.shields.io/badge/year-2024-red)
* VLsI: Verbalized Layers-to-Interactions from Large to Small Vision Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:274436440) ![](https://img.shields.io/badge/year-2024-red)

**Sequence Distillation**

* MASSV: Multimodal Adaptation and Self-Data Distillation for Speculative Decoding of Vision-Language Models [[Paper]](https://arxiv.org/abs/2505.10526) ![](https://img.shields.io/badge/year-2025-red)
* Visual Program Distillation: Distilling Tools and Programmatic Reasoning into Vision-Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:265693898) ![](https://img.shields.io/badge/year-2023-red)
* Distilling Internet-Scale Vision-Language Models into Embodied Agents [[Paper]](https://arxiv.org/abs/2301.12507) ![](https://img.shields.io/badge/year-2023-red)
* VLM-KD: Knowledge Distillation from VLM for Long-Tail Visual Recognition [[Paper]](https://api.semanticscholar.org/CorpusID:272310206) ![](https://img.shields.io/badge/year-2024-red)
* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)
* Refined Policy Distillation: From VLA Generalists to RL Experts [[Paper]](https://www.semanticscholar.org/search?q=Refined%20policy%20distillation%3A%20From%20vla%20generalists%20to%20rl%20experts) ![](https://img.shields.io/badge/year-2025-red)
* RDT2: Exploring the Scaling Limit of UMI Data Towards Zero-Shot Cross-Embodiment Generalization [[Paper]](https://arxiv.org/abs/2602.03310) ![](https://img.shields.io/badge/year-2026-red)

**Preference Distillation**

* LLaVA-MoD: Making LLaVA Tiny via MoE Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:271974282) ![](https://img.shields.io/badge/year-2024-red)
* mDPO: Conditional Preference Optimization for Multimodal Large Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:270560448) ![](https://img.shields.io/badge/year-2024-red)


## Section II: Feature-based Distillation

**Hidden-state Distillation**

* Layerwised Multimodal Knowledge Distillation for Vision-Language Pretrained Model [[Paper]](https://doi.org/10.1016/j.neunet.2024.106272) ![](https://img.shields.io/badge/year-2024-red)
* KD-VLP: Improving End-to-End Vision-and-Language Pretraining with Object Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:237593048) ![](https://img.shields.io/badge/year-2021-red)
* Building Vision-Language Models on Solid Foundations with Masked Distillation [[Paper]](https://doi.org/10.1109/CVPR52733.2024.01348) ![](https://img.shields.io/badge/year-2024-red)
* TinyViT: Fast Pretraining Distillation for Small Vision Transformers [[Paper]](https://api.semanticscholar.org/CorpusID:250920355) ![](https://img.shields.io/badge/year-2022-red)
* Compressing Visual-Linguistic Model via Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:233033712) ![](https://img.shields.io/badge/year-2021-red)
* MiniVLM: A Smaller and Faster Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:229153061) ![](https://img.shields.io/badge/year-2020-red)
* VITA-VLA: Efficiently Teaching Vision-Language Models to Act via Action Expert Distillation [[Paper]](https://arxiv.org/abs/2510.09607) ![](https://img.shields.io/badge/year-2025-red)
* Shallow-pi: Knowledge Distillation for Flow-based VLAs [[Paper]](https://arxiv.org/abs/2601.20262) ![](https://img.shields.io/badge/year-2026-red)
* CEED-VLA: Consistency Vision-Language-Action Model with Early-Exit Decoding [[Paper]](https://arxiv.org/abs/2506.13725) ![](https://img.shields.io/badge/year-2025-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2023-red)
* LP-OVOD: Open-Vocabulary Object Detection by Linear Probing [[Paper]](https://www.semanticscholar.org/search?q=Lp-ovod%3A%20Open-vocabulary%20object%20detection%20by%20linear%20probing) ![](https://img.shields.io/badge/year-2024-red)

**Attention Distillation**

* CompoDistill: Attention Distillation for Compositional Reasoning in Multimodal LLMs [[Paper]](https://api.semanticscholar.org/CorpusID:282064279) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:274437419) ![](https://img.shields.io/badge/year-2024-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://api.semanticscholar.org/CorpusID:262083905) ![](https://img.shields.io/badge/year-2023-red)
* AC^2-VLA: Action-Context-Aware Adaptive Computation in Vision-Language-Action Models for Efficient Robotic Manipulation [[Paper]](https://arxiv.org/abs/2601.19634) ![](https://img.shields.io/badge/year-2026-red)
* DeCLIP: Decoupled Learning for Open-Vocabulary Dense Perception [[Paper]](https://www.semanticscholar.org/search?q=Declip%3A%20Decoupled%20learning%20for%20open-vocabulary%20dense%20perception) ![](https://img.shields.io/badge/year-2025-red)

**Cross-modal Feature Distillation**

* EM-KD: Distilling Efficient Multimodal Large Language Model with Unbalanced Vision Tokens [[Paper]](https://api.semanticscholar.org/CorpusID:283262068) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:274437419) ![](https://img.shields.io/badge/year-2024-red)
* Modality-specific Knowledge Distillation with Wasserstein Distance Minimization for Vision-Language Pretrained Models [[Paper]](https://doi.org/10.1109/TAI.2025.3613686) ![](https://img.shields.io/badge/year-2025-red)
* Multimodal Adaptive Distillation for Leveraging Unimodal Encoders for Vision-Language Tasks [[Paper]](https://api.semanticscholar.org/CorpusID:248366429) ![](https://img.shields.io/badge/year-2022-red)
* Unsupervised Knowledge Distillation via Local Representations for Vision-Language Models [[Paper]](https://doi.org/10.1109/LSP.2025.3582567) ![](https://img.shields.io/badge/year-2025-red)
* TE-VLM: Transfer Entropy for Vision Language Model Distillation [[Paper]](https://openreview.net/forum?id=vJV22Ig8YG) ![](https://img.shields.io/badge/year-2025-red)
* KAID: Knowledge-Aware Interactive Distillation for Vision-Language Models [[Paper]](https://doi.org/10.1145/3746027.3755008) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* FD-VLA: Force-Distilled Vision-Language-Action Model for Contact-Rich Manipulation [[Paper]](https://arxiv.org/abs/2602.02142) ![](https://img.shields.io/badge/year-2026-red)
* VISTA: Enhancing Visual Conditioning via Track-Following Preference Optimization in Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2602.05049) ![](https://img.shields.io/badge/year-2026-red)
* OmniReason: A Temporal-Guided Vision-Language-Action Framework for Autonomous Driving [[Paper]](https://arxiv.org/abs/2509.00789) ![](https://img.shields.io/badge/year-2025-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Open-vocabulary%20one-stage%20detection%20with%20hierarchical%20visual-language%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2022-red)
* Object-Aware Distillation Pyramid for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Object-aware%20distillation%20pyramid%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* Learning Background Prompts to Discover Implicit Knowledge for Open Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Learning%20background%20prompts%20to%20discover%20implicit%20knowledge%20for%20open%20vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2024-red)
* SKDF: A Simple Knowledge Distillation Framework for Distilling Open-Vocabulary Knowledge to Open-World Object Detector [[Paper]](https://www.semanticscholar.org/search?q=SKDF%3A%20a%20simple%20knowledge%20distillation%20framework%20for%20distilling%20open-vocabulary%20knowledge%20to%20open-world%20object%20detector) ![](https://img.shields.io/badge/year-2025-red)


## Section III: Relation-based Distillation

**Similarity-based Distillation**

* CLIP-KD: An Empirical Study of CLIP Model Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:260125303) ![](https://img.shields.io/badge/year-2023-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://api.semanticscholar.org/CorpusID:262083905) ![](https://img.shields.io/badge/year-2023-red)
* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://api.semanticscholar.org/CorpusID:265466718) ![](https://img.shields.io/badge/year-2023-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/search?q=Promptkd%3A%20Unsupervised%20prompt%20distillation%20for%20vision-language%20models) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-Embed-KD: Computationally Efficient Knowledge Distillation Using Embeddings as Teachers [[Paper]](https://arxiv.org/abs/2404.06170) ![](https://img.shields.io/badge/year-2024-red)
* Filtering, Distillation, and Hard Negatives for Vision-Language Pre-Training [[Paper]](https://api.semanticscholar.org/CorpusID:255522657) ![](https://img.shields.io/badge/year-2023-red)
* Open-Vocabulary Object Detection via Vision and Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.13921) ![](https://img.shields.io/badge/year-2021-red)

**Contrastive Distillation**

* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://api.semanticscholar.org/CorpusID:265466718) ![](https://img.shields.io/badge/year-2023-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/search?q=Promptkd%3A%20Unsupervised%20prompt%20distillation%20for%20vision-language%20models) ![](https://img.shields.io/badge/year-2024-red)
* Filtering, Distillation, and Hard Negatives for Vision-Language Pre-Training [[Paper]](https://api.semanticscholar.org/CorpusID:255522657) ![](https://img.shields.io/badge/year-2023-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://api.semanticscholar.org/CorpusID:262083905) ![](https://img.shields.io/badge/year-2023-red)
* A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance [[Paper]](https://api.semanticscholar.org/CorpusID:262217079) ![](https://img.shields.io/badge/year-2023-red)
* Distilling CLIP with Dual Guidance for Learning Discriminative Human Body Shape Representation [[Paper]](https://doi.org/10.1109/CVPR52733.2024.00032) ![](https://img.shields.io/badge/year-2024-red)
* Enabling Multimodal Generation on CLIP via Vision-Language Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:247447159) ![](https://img.shields.io/badge/year-2022-red)
* Aligning Bag of Regions for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Aligning%20bag%20of%20regions%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* Cyclic Contrastive Knowledge Transfer for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2503.11005) ![](https://img.shields.io/badge/year-2025-red)
* Exploring Multi-Modal Contextual Knowledge for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Exploring%20multi-modal%20contextual%20knowledge%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2024-red)
* VLDadaptor: Domain Adaptive Object Detection with Vision-Language Model Distillation [[Paper]](https://www.semanticscholar.org/search?q=VLDadaptor%3A%20Domain%20adaptive%20object%20detection%20with%20vision-language%20model%20distillation) ![](https://img.shields.io/badge/year-2024-red)


## Section IV: White-box Distillation

* Layerwised Multimodal Knowledge Distillation for Vision-Language Pretrained Model [[Paper]](https://doi.org/10.1016/j.neunet.2024.106272) ![](https://img.shields.io/badge/year-2024-red)
* KD-VLP: Improving End-to-End Vision-and-Language Pretraining with Object Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:237593048) ![](https://img.shields.io/badge/year-2021-red)
* CompoDistill: Attention Distillation for Compositional Reasoning in Multimodal LLMs [[Paper]](https://api.semanticscholar.org/CorpusID:282064279) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:274437419) ![](https://img.shields.io/badge/year-2024-red)
* EM-KD: Distilling Efficient Multimodal Large Language Model with Unbalanced Vision Tokens [[Paper]](https://api.semanticscholar.org/CorpusID:283262068) ![](https://img.shields.io/badge/year-2025-red)
* Modality-specific Knowledge Distillation with Wasserstein Distance Minimization for Vision-Language Pretrained Models [[Paper]](https://doi.org/10.1109/TAI.2025.3613686) ![](https://img.shields.io/badge/year-2025-red)
* TE-VLM: Transfer Entropy for Vision Language Model Distillation [[Paper]](https://openreview.net/forum?id=vJV22Ig8YG) ![](https://img.shields.io/badge/year-2025-red)
* KAID: Knowledge-Aware Interactive Distillation for Vision-Language Models [[Paper]](https://doi.org/10.1145/3746027.3755008) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* Shallow-pi: Knowledge Distillation for Flow-based VLAs [[Paper]](https://arxiv.org/abs/2601.20262) ![](https://img.shields.io/badge/year-2026-red)
* Aligning Bag of Regions for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Aligning%20bag%20of%20regions%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* Building Vision-Language Models on Solid Foundations with Masked Distillation [[Paper]](https://doi.org/10.1109/CVPR52733.2024.01348) ![](https://img.shields.io/badge/year-2024-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://api.semanticscholar.org/CorpusID:262083905) ![](https://img.shields.io/badge/year-2023-red)
* Compressing Visual-Linguistic Model via Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:233033712) ![](https://img.shields.io/badge/year-2021-red)
* MiniVLM: A Smaller and Faster Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:229153061) ![](https://img.shields.io/badge/year-2020-red)
* Multimodal Adaptive Distillation for Leveraging Unimodal Encoders for Vision-Language Tasks [[Paper]](https://api.semanticscholar.org/CorpusID:248366429) ![](https://img.shields.io/badge/year-2022-red)
* Unsupervised Knowledge Distillation via Local Representations for Vision-Language Models [[Paper]](https://doi.org/10.1109/LSP.2025.3582567) ![](https://img.shields.io/badge/year-2025-red)
* LLaVA-KD: A Framework of Distilling Multimodal Large Language Models [[Paper]](https://www.semanticscholar.org/search?q=Llava-kd%3A%20A%20framework%20of%20distilling%20multimodal%20large%20language%20models) ![](https://img.shields.io/badge/year-2025-red)
* GenRecal: Generation after Recalibration from Large to Small Vision-Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:279447364) ![](https://img.shields.io/badge/year-2025-red)


## Section V: Black-box Distillation

* Visual Program Distillation: Distilling Tools and Programmatic Reasoning into Vision-Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:265693898) ![](https://img.shields.io/badge/year-2023-red)
* ShareGPT4V: Improving Large Multi-Modal Models with Better Captions [[Paper]](https://www.semanticscholar.org/search?q=Sharegpt4v%3A%20Improving%20large%20multi-modal%20models%20with%20better%20captions) ![](https://img.shields.io/badge/year-2024-red)
* MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:258291930) ![](https://img.shields.io/badge/year-2023-red)
* ALLaVA: Harnessing GPT4V-Synthesized Data for Lite Vision-Language Models [[Paper]](https://arxiv.org/abs/2402.11684) ![](https://img.shields.io/badge/year-2024-red)
* PCoreSet: Effective Active Learning through Knowledge Distillation from Vision-Language Models [[Paper]](https://arxiv.org/abs/2506.00910) ![](https://img.shields.io/badge/year-2025-red)
* CLIP-Embed-KD: Computationally Efficient Knowledge Distillation Using Embeddings as Teachers [[Paper]](https://arxiv.org/abs/2404.06170) ![](https://img.shields.io/badge/year-2024-red)
* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Open-vocabulary%20one-stage%20detection%20with%20hierarchical%20visual-language%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2022-red)
* Bridging the Gap between Object and Image-Level Representations for Open-Vocabulary Detection [[Paper]](https://www.semanticscholar.org/search?q=Bridging%20the%20gap%20between%20object%20and%20image-level%20representations%20for%20open-vocabulary%20detection) ![](https://img.shields.io/badge/year-2022-red)


## Section VI: Self-Distillation

* COSMOS: Cross-Modality Self-Distillation for Vision Language Pre-training [[Paper]](https://www.semanticscholar.org/search?q=Cosmos%3A%20Cross-modality%20self-distillation%20for%20vision%20language%20pre-training) ![](https://img.shields.io/badge/year-2025-red)
* Align before Fuse: Vision and Language Representation Learning with Momentum Distillation [[Paper]](https://www.semanticscholar.org/search?q=Align%20before%20fuse%3A%20Vision%20and%20language%20representation%20learning%20with%20momentum%20distillation) ![](https://img.shields.io/badge/year-2021-red)
* Building Vision-Language Models on Solid Foundations with Masked Distillation [[Paper]](https://doi.org/10.1109/CVPR52733.2024.01348) ![](https://img.shields.io/badge/year-2024-red)
* Improving Zero-Shot Generalization of Learned Prompts via Unsupervised Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Improving%20zero-shot%20generalization%20of%20learned%20prompts%20via%20unsupervised%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2024-red)
* Self-Improving Vision-Language-Action Models with Data Generation via Residual RL [[Paper]](https://arxiv.org/abs/2511.00091) ![](https://img.shields.io/badge/year-2025-red)
* MoLe-VLA: Dynamic Layer-Skipping Vision Language Action Model via Mixture-of-Layers for Efficient Robot Manipulation [[Paper]](https://arxiv.org/abs/2503.20384) ![](https://img.shields.io/badge/year-2025-red)
* CEED-VLA: Consistency Vision-Language-Action Model with Early-Exit Decoding [[Paper]](https://arxiv.org/abs/2506.13725) ![](https://img.shields.io/badge/year-2025-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2023-red)


## Section VII: Multi-teacher Distillation

* MoVE-KD: Knowledge Distillation for VLMs with Mixture of Visual Encoders [[Paper]](https://www.semanticscholar.org/search?q=Move-kd%3A%20Knowledge%20distillation%20for%20vlms%20with%20mixture%20of%20visual%20encoders) ![](https://img.shields.io/badge/year-2025-red)
* MST-Distill: Mixture of Specialized Teachers for Cross-Modal Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Mst-distill%3A%20Mixture%20of%20specialized%20teachers%20for%20cross-modal%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2025-red)
* AMMKD: Adaptive Multimodal Multi-Teacher Distillation for Lightweight Vision-Language Models [[Paper]](https://arxiv.org/abs/2509.00039) ![](https://img.shields.io/badge/year-2025-red)
* Retaining Knowledge and Enhancing Long-Text Representations in CLIP through Dual-Teacher Distillation [[Paper]](https://doi.org/10.1109/CVPR52734.2025.02318) ![](https://img.shields.io/badge/year-2025-red)
* KAID: Knowledge-Aware Interactive Distillation for Vision-Language Models [[Paper]](https://doi.org/10.1145/3746027.3755008) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)


## Section VIII: Structural Compatibility - Isomorphic

* LLaVA-KD: A Framework of Distilling Multimodal Large Language Models [[Paper]](https://www.semanticscholar.org/search?q=Llava-kd%3A%20A%20framework%20of%20distilling%20multimodal%20large%20language%20models) ![](https://img.shields.io/badge/year-2025-red)
* MASSV: Multimodal Adaptation and Self-Data Distillation for Speculative Decoding of Vision-Language Models [[Paper]](https://arxiv.org/abs/2505.10526) ![](https://img.shields.io/badge/year-2025-red)
* Select and Distill: Selective Dual-Teacher Knowledge Transfer for Continual Learning on Vision-Language Models [[Paper]](https://www.semanticscholar.org/search?q=Select%20and%20distill%3A%20Selective%20dual-teacher%20knowledge%20transfer%20for%20continual%20learning%20on%20vision-language%20models) ![](https://img.shields.io/badge/year-2024-red)
* Collaborative Training of Tiny-Large Vision Language Models [[Paper]](https://openreview.net/forum?id=Ugy9DyhYYD) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-KD: An Empirical Study of CLIP Model Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:260125303) ![](https://img.shields.io/badge/year-2023-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://api.semanticscholar.org/CorpusID:262083905) ![](https://img.shields.io/badge/year-2023-red)
* CLIP-Embed-KD: Computationally Efficient Knowledge Distillation Using Embeddings as Teachers [[Paper]](https://arxiv.org/abs/2404.06170) ![](https://img.shields.io/badge/year-2024-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/search?q=Promptkd%3A%20Unsupervised%20prompt%20distillation%20for%20vision-language%20models) ![](https://img.shields.io/badge/year-2024-red)
* Filtering, Distillation, and Hard Negatives for Vision-Language Pre-Training [[Paper]](https://api.semanticscholar.org/CorpusID:255522657) ![](https://img.shields.io/badge/year-2023-red)
* Improving CLIP Fine-tuning Performance [[Paper]](https://doi.org/10.1109/ICCV51070.2023.00501) ![](https://img.shields.io/badge/year-2023-red)
* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://api.semanticscholar.org/CorpusID:265466718) ![](https://img.shields.io/badge/year-2023-red)
* Distilling CLIP with Dual Guidance for Learning Discriminative Human Body Shape Representation [[Paper]](https://doi.org/10.1109/CVPR52733.2024.00032) ![](https://img.shields.io/badge/year-2024-red)
* Self-Improving Vision-Language-Action Models with Data Generation via Residual RL [[Paper]](https://arxiv.org/abs/2511.00091) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)
* Open-Vocabulary Object Detection via Vision and Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.13921) ![](https://img.shields.io/badge/year-2021-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Open-vocabulary%20one-stage%20detection%20with%20hierarchical%20visual-language%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2022-red)
* Distilling DETR with Visual-Linguistic Knowledge for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Distilling%20detr%20with%20visual-linguistic%20knowledge%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* A Hierarchical Semantic Distillation Framework for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=A%20hierarchical%20semantic%20distillation%20framework%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2025-red)
* CAKE: Category Aware Knowledge Extraction for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Cake%3A%20Category%20aware%20knowledge%20extraction%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2025-red)
* GenRecal: Generation after Recalibration from Large to Small Vision-Language Models [[Paper]](https://api.semanticscholar.org/CorpusID:279447364) ![](https://img.shields.io/badge/year-2025-red)


## Section IX: Structural Compatibility - Cross-Architecture

* TinyViT: Fast Pretraining Distillation for Small Vision Transformers [[Paper]](https://api.semanticscholar.org/CorpusID:250920355) ![](https://img.shields.io/badge/year-2022-red)
* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://api.semanticscholar.org/CorpusID:265466718) ![](https://img.shields.io/badge/year-2023-red)
* Generative Negative Text Replay for Continual Vision-Language Pretraining [[Paper]](https://www.semanticscholar.org/search?q=Generative%20negative%20text%20replay%20for%20continual%20vision-language%20pretraining) ![](https://img.shields.io/badge/year-2022-red)
* LLaVA-MoD: Making LLaVA Tiny via MoE Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:271974282) ![](https://img.shields.io/badge/year-2024-red)
* MiniVLM: A Smaller and Faster Vision-Language Model [[Paper]](https://api.semanticscholar.org/CorpusID:229153061) ![](https://img.shields.io/badge/year-2020-red)
* VL2Lite: Task-Specific Knowledge Distillation from Large Vision-Language Models to Lightweight Networks [[Paper]](https://doi.org/10.1109/CVPR52734.2025.02799) ![](https://img.shields.io/badge/year-2025-red)
* CustomKD: Customizing Large Vision Foundation for Edge Model Improvement via Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Customkd%3A%20Customizing%20large%20vision%20foundation%20for%20edge%20model%20improvement%20via%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2025-red)
* EfficientVLM: Fast and Accurate Vision-Language Models via Knowledge Distillation and Modal-Adaptive Pruning [[Paper]](https://www.semanticscholar.org/search?q=Efficientvlm%3A%20Fast%20and%20accurate%20vision-language%20models%20via%20knowledge%20distillation%20and%20modal-adaptive%20pruning) ![](https://img.shields.io/badge/year-2023-red)
* CIFD: Controlled Information Flow to Enhance Knowledge Distillation [[Paper]](https://openreview.net/forum?id=xutrKezbPF) ![](https://img.shields.io/badge/year-2024-red)
* Compressing Visual-Linguistic Model via Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:233033712) ![](https://img.shields.io/badge/year-2021-red)
* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* VITA-VLA: Efficiently Teaching Vision-Language Models to Act via Action Expert Distillation [[Paper]](https://arxiv.org/abs/2510.09607) ![](https://img.shields.io/badge/year-2025-red)
* Refined Policy Distillation: From VLA Generalists to RL Experts [[Paper]](https://www.semanticscholar.org/search?q=Refined%20policy%20distillation%3A%20From%20vla%20generalists%20to%20rl%20experts) ![](https://img.shields.io/badge/year-2025-red)


## Section X: Structural Compatibility - Cross-Modal

* A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance [[Paper]](https://api.semanticscholar.org/CorpusID:262217079) ![](https://img.shields.io/badge/year-2023-red)
* Enabling Multimodal Generation on CLIP via Vision-Language Knowledge Distillation [[Paper]](https://api.semanticscholar.org/CorpusID:247447159) ![](https://img.shields.io/badge/year-2022-red)
* Distilling CLIP with Dual Guidance for Learning Discriminative Human Body Shape Representation [[Paper]](https://doi.org/10.1109/CVPR52733.2024.00032) ![](https://img.shields.io/badge/year-2024-red)
* Unsupervised Knowledge Distillation via Local Representations for Vision-Language Models [[Paper]](https://doi.org/10.1109/LSP.2025.3582567) ![](https://img.shields.io/badge/year-2025-red)
* TE-VLM: Transfer Entropy for Vision Language Model Distillation [[Paper]](https://openreview.net/forum?id=vJV22Ig8YG) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* FD-VLA: Force-Distilled Vision-Language-Action Model for Contact-Rich Manipulation [[Paper]](https://arxiv.org/abs/2602.02142) ![](https://img.shields.io/badge/year-2026-red)
* Bridging the Gap between Object and Image-Level Representations for Open-Vocabulary Detection [[Paper]](https://www.semanticscholar.org/search?q=Bridging%20the%20gap%20between%20object%20and%20image-level%20representations%20for%20open-vocabulary%20detection) ![](https://img.shields.io/badge/year-2022-red)
* The Modality Focusing Hypothesis: Towards Understanding Crossmodal Knowledge Distillation [[Paper]](https://arxiv.org/abs/2206.06487) ![](https://img.shields.io/badge/year-2022-red)

---

## Knowledge Distillation for Vision-Language-Action Models

* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* Self-Improving Vision-Language-Action Models with Data Generation via Residual RL [[Paper]](https://arxiv.org/abs/2511.00091) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* LatBot: Distilling Universal Latent Actions for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2511.23034) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* FD-VLA: Force-Distilled Vision-Language-Action Model for Contact-Rich Manipulation [[Paper]](https://arxiv.org/abs/2602.02142) ![](https://img.shields.io/badge/year-2026-red)
* VISTA: Enhancing Visual Conditioning via Track-Following Preference Optimization in Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2602.05049) ![](https://img.shields.io/badge/year-2026-red)
* VITA-VLA: Efficiently Teaching Vision-Language Models to Act via Action Expert Distillation [[Paper]](https://arxiv.org/abs/2510.09607) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)
* Refined Policy Distillation: From VLA Generalists to RL Experts [[Paper]](https://www.semanticscholar.org/search?q=Refined%20policy%20distillation%3A%20From%20vla%20generalists%20to%20rl%20experts) ![](https://img.shields.io/badge/year-2025-red)
* Shallow-pi: Knowledge Distillation for Flow-based VLAs [[Paper]](https://arxiv.org/abs/2601.20262) ![](https://img.shields.io/badge/year-2026-red)
* MoLe-VLA: Dynamic Layer-Skipping Vision Language Action Model via Mixture-of-Layers for Efficient Robot Manipulation [[Paper]](https://arxiv.org/abs/2503.20384) ![](https://img.shields.io/badge/year-2025-red)
* CEED-VLA: Consistency Vision-Language-Action Model with Early-Exit Decoding [[Paper]](https://arxiv.org/abs/2506.13725) ![](https://img.shields.io/badge/year-2025-red)
* AC^2-VLA: Action-Context-Aware Adaptive Computation in Vision-Language-Action Models for Efficient Robotic Manipulation [[Paper]](https://arxiv.org/abs/2601.19634) ![](https://img.shields.io/badge/year-2026-red)
* OmniReason: A Temporal-Guided Vision-Language-Action Framework for Autonomous Driving [[Paper]](https://arxiv.org/abs/2509.00789) ![](https://img.shields.io/badge/year-2025-red)
* RDT2: Exploring the Scaling Limit of UMI Data Towards Zero-Shot Cross-Embodiment Generalization [[Paper]](https://arxiv.org/abs/2602.03310) ![](https://img.shields.io/badge/year-2026-red)


## Knowledge Distillation for Vision-Language Embedding Models

* Qwen3-VL-Embedding and Qwen3-VL-Reranker: A Unified Framework for State-of-the-Art Multimodal Retrieval and Ranking [[Paper]](https://arxiv.org/abs/2601.04720) ![](https://img.shields.io/badge/year-2026-red)
* UniME-V2: MLLM-as-a-Judge for Universal Multimodal Embedding Learning [[Paper]](https://arxiv.org/abs/2510.13515) ![](https://img.shields.io/badge/year-2025-red)
* xVLM2Vec: Adapting LVLM-based Embedding Models to Multilinguality using Self-Knowledge Distillation [[Paper]](https://arxiv.org/abs/2503.09313) ![](https://img.shields.io/badge/year-2025-red)
* Breaking the Modality Barrier: Universal Embedding Learning with Multimodal LLMs [[Paper]](https://arxiv.org/abs/2504.17432) ![](https://img.shields.io/badge/year-2025-red)


## VLM Knowledge Distillation for Segmentation

* Extract Free Dense Labels from CLIP [[Paper]](https://arxiv.org/abs/2112.01071) ![](https://img.shields.io/badge/year-2022-red)
* CLIP is Also an Efficient Segmenter: A Text-Driven Approach for Weakly Supervised Semantic Segmentation [[Paper]](https://arxiv.org/abs/2212.09506) ![](https://img.shields.io/badge/year-2023-red)
* Plug-and-Play, Dense-Label-Free Extraction of Open-Vocabulary Semantic Segmentation from Vision-Language Models [[Paper]](https://doi.org/10.48550/arXiv.2311.17095) ![](https://img.shields.io/badge/year-2023-red)
* Segment Anything is A Good Pseudo-label Generator for Weakly Supervised Semantic Segmentation [[Paper]](https://arxiv.org/abs/2305.01275) ![](https://img.shields.io/badge/year-2023-red)
* ZegCLIP: Towards Adapting CLIP for Zero-shot Semantic Segmentation [[Paper]](https://arxiv.org/abs/2212.03588) ![](https://img.shields.io/badge/year-2023-red)
* Open-Vocabulary Semantic Segmentation with Frozen Vision-Language Models [[Paper]](https://arxiv.org/abs/2210.15138) ![](https://img.shields.io/badge/year-2022-red)
* Open-Vocabulary Semantic Segmentation with Mask-adapted CLIP [[Paper]](https://arxiv.org/abs/2210.04150) ![](https://img.shields.io/badge/year-2023-red)
* A Simple Baseline for Open-Vocabulary Semantic Segmentation with Pre-trained Vision-language Model [[Paper]](https://arxiv.org/abs/2112.14757) ![](https://img.shields.io/badge/year-2022-red)
* Scaling Open-Vocabulary Image Segmentation with Image-Level Labels [[Paper]](https://arxiv.org/abs/2112.12143) ![](https://img.shields.io/badge/year-2022-red)
* FreeSeg: Unified, Universal and Open-Vocabulary Image Segmentation [[Paper]](https://arxiv.org/abs/2303.17225) ![](https://img.shields.io/badge/year-2023-red)
* Language-driven Semantic Segmentation [[Paper]](https://arxiv.org/abs/2201.03546) ![](https://img.shields.io/badge/year-2022-red)
* Image Segmentation Using Text and Image Prompts [[Paper]](https://arxiv.org/abs/2112.10003) ![](https://img.shields.io/badge/year-2022-red)
* SegPrompt: Boosting Open-world Segmentation via Category-level Prompt Learning [[Paper]](https://arxiv.org/abs/2308.06531) ![](https://img.shields.io/badge/year-2023-red)
* Exploring Open-Vocabulary Semantic Segmentation without Human Labels [[Paper]](https://arxiv.org/abs/2306.00450) ![](https://img.shields.io/badge/year-2023-red)
* Mask-free OVIS: Open-Vocabulary Instance Segmentation without Manual Mask Annotations [[Paper]](https://arxiv.org/abs/2303.16891) ![](https://img.shields.io/badge/year-2023-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2024-red)
* PartDistill: 3D Shape Part Segmentation by Vision-Language Model Distillation [[Paper]](https://arxiv.org/abs/2312.04016) ![](https://img.shields.io/badge/year-2024-red)
* Decoupling Zero-Shot Semantic Segmentation [[Paper]](https://arxiv.org/abs/2112.07910) ![](https://img.shields.io/badge/year-2022-red)


## VLM Knowledge Distillation for Open-Vocabulary Object Detection

* Open-Vocabulary Object Detection via Vision and Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.13921) ![](https://img.shields.io/badge/year-2021-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://www.semanticscholar.org/search?q=Open-vocabulary%20one-stage%20detection%20with%20hierarchical%20visual-language%20knowledge%20distillation) ![](https://img.shields.io/badge/year-2022-red)
* Bridging the Gap between Object and Image-Level Representations for Open-Vocabulary Detection [[Paper]](https://www.semanticscholar.org/search?q=Bridging%20the%20gap%20between%20object%20and%20image-level%20representations%20for%20open-vocabulary%20detection) ![](https://img.shields.io/badge/year-2022-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2023-red)
* Object-Aware Distillation Pyramid for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Object-aware%20distillation%20pyramid%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* Aligning Bag of Regions for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Aligning%20bag%20of%20regions%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* Distilling DETR with Visual-Linguistic Knowledge for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Distilling%20detr%20with%20visual-linguistic%20knowledge%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2023-red)
* DeCLIP: Decoupled Learning for Open-Vocabulary Dense Perception [[Paper]](https://www.semanticscholar.org/search?q=Declip%3A%20Decoupled%20learning%20for%20open-vocabulary%20dense%20perception) ![](https://img.shields.io/badge/year-2025-red)
* A Hierarchical Semantic Distillation Framework for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=A%20hierarchical%20semantic%20distillation%20framework%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2025-red)
* CAKE: Category Aware Knowledge Extraction for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Cake%3A%20Category%20aware%20knowledge%20extraction%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2025-red)
* Cyclic Contrastive Knowledge Transfer for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2503.11005) ![](https://img.shields.io/badge/year-2025-red)
* Learning Background Prompts to Discover Implicit Knowledge for Open Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Learning%20background%20prompts%20to%20discover%20implicit%20knowledge%20for%20open%20vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2024-red)
* Exploring Multi-Modal Contextual Knowledge for Open-Vocabulary Object Detection [[Paper]](https://www.semanticscholar.org/search?q=Exploring%20multi-modal%20contextual%20knowledge%20for%20open-vocabulary%20object%20detection) ![](https://img.shields.io/badge/year-2024-red)
* LP-OVOD: Open-Vocabulary Object Detection by Linear Probing [[Paper]](https://www.semanticscholar.org/search?q=Lp-ovod%3A%20Open-vocabulary%20object%20detection%20by%20linear%20probing) ![](https://img.shields.io/badge/year-2024-red)
* SKDF: A Simple Knowledge Distillation Framework for Distilling Open-Vocabulary Knowledge to Open-World Object Detector [[Paper]](https://www.semanticscholar.org/search?q=SKDF%3A%20a%20simple%20knowledge%20distillation%20framework%20for%20distilling%20open-vocabulary%20knowledge%20to%20open-world%20object%20detector) ![](https://img.shields.io/badge/year-2025-red)
* VLDadaptor: Domain Adaptive Object Detection with Vision-Language Model Distillation [[Paper]](https://www.semanticscholar.org/search?q=VLDadaptor%3A%20Domain%20adaptive%20object%20detection%20with%20vision-language%20model%20distillation) ![](https://img.shields.io/badge/year-2024-red)

