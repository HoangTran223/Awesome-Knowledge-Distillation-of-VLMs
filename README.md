## A Survey on Knowledge Distillation of Vision-Language Models

## 🔔 News

- **[21/08/2026]** 🎉 This survey has been accepted by the Conference on Empirical Methods in Natural Language Processing (EMNLP) 2026!

## 📝 Introduction

This paper provides **the first dedicated survey of knowledge distillation for vision-language models**. We propose a unified taxonomy that organizes methods along three orthogonal views: knowledge type, teacher accessibility, and structural compatibility, and use it to organize methods across major VLM distillation settings.

## 📊 Taxonomy

Below is the taxonomy summarizing the landscape of knowledge distillation research for VLMs:

![Taxonomy](./Figure/Taxonomy.png)

This survey organizes VLM distillation methods along three **orthogonal** axes. Each axis is illustrated below, immediately before the corresponding paper sections.

| Axis | Question | Sections |
|---|---|---|
| **Knowledge Type** | What does the student learn from the teacher? | [I](#section-i-response-based-distillation) · [II](#section-ii-feature-based-distillation) · [III](#section-iii-relation-based-distillation) |
| **Teacher Accessibility** | What can the student observe about the teacher? | [IV](#section-iv-white-box-distillation) · [V](#section-v-black-box-distillation) · [VI](#section-vi-self-distillation) · [VII](#section-vii-multi-teacher-distillation) |
| **Structural Compatibility** | What must be bridged before distillation can proceed? | [VIII](#section-viii-structural-compatibility---isomorphic) · [IX](#section-ix-structural-compatibility---cross-architecture) · [X](#section-x-structural-compatibility---cross-modal) |

| Application | Section |
|---|---|
| Vision-Language-Action | [VLA](#knowledge-distillation-for-vision-language-action-models) |
| Vision-Language Embedding | [Embedding](#knowledge-distillation-for-vision-language-embedding-models) |
| Semantic Segmentation | [Segmentation](#vlm-knowledge-distillation-for-segmentation) |
| Open-Vocabulary Object Detection | [OVD](#vlm-knowledge-distillation-for-open-vocabulary-object-detection) |

## Knowledge Type

<p align="left">
  <img src="./Figure/Figure_2.jpg" alt="Knowledge Type view of VLM distillation" width="600">
</p>

| Branch | Section |
|---|---|
| Response-based Distillation | [Section I](#section-i-response-based-distillation) |
| Feature-based Distillation | [Section II](#section-ii-feature-based-distillation) |
| Relation-based Distillation | [Section III](#section-iii-relation-based-distillation) |

## Section I: Response-based Distillation

**Logit Distillation**

* LLaVA-KD: A Framework of Distilling Multimodal Large Language Models [[Paper]](https://openaccess.thecvf.com/content/ICCV2025/papers/Cai_LLaVA-KD_A_Framework_of_Distilling_Multimodal_Large_Language_Models_ICCV_2025_paper.pdf) ![](https://img.shields.io/badge/year-2025-red)
* VLsI: Verbalized Layers-to-Interactions from Large to Small Vision Language Models [[Paper]](https://arxiv.org/abs/2412.01822) ![](https://img.shields.io/badge/year-2025-red)
* MASSV: Multimodal Adaptation and Self-Data Distillation for Speculative Decoding of Vision-Language Models [[Paper]](https://arxiv.org/abs/2505.10526) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://openreview.net/pdf?id=xsCK546dra) ![](https://img.shields.io/badge/year-2024-red)
* GenRecal: Generation after Recalibration from Large to Small Vision-Language Models [[Paper]](https://arxiv.org/pdf/2506.15681) ![](https://img.shields.io/badge/year-2025-red)
* EM-KD: Distilling Efficient Multimodal Large Language Model with Unbalanced Vision Tokens [[Paper]](https://arxiv.org/pdf/2511.21106) ![](https://img.shields.io/badge/year-2025-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_PromptKD_Unsupervised_Prompt_Distillation_for_Vision-Language_Models_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* Improving Zero-Shot Generalization of Learned Prompts via Unsupervised Knowledge Distillation [[Paper]](https://arxiv.org/abs/2407.03056) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-KD: An Empirical Study of CLIP Model Distillation [[Paper]](https://arxiv.org/abs/2307.12732) ![](https://img.shields.io/badge/year-2023-red)
* AMMKD: Adaptive Multimodal Multi-Teacher Distillation for Lightweight Vision-Language Models [[Paper]](https://arxiv.org/abs/2509.00039) ![](https://img.shields.io/badge/year-2025-red)
* VL2Lite: Task-Specific Knowledge Distillation from Large Vision-Language Models to Lightweight Networks [[Paper]](https://openaccess.thecvf.com/content/CVPR2025/papers/Jang_VL2Lite_Task-Specific_Knowledge_Distillation_from_Large_Vision-Language_Models_to_Lightweight_CVPR_2025_paper.pdf) ![](https://img.shields.io/badge/year-2025-red)
* VLM-KD: Knowledge Distillation from VLM for Long-Tail Visual Recognition [[Paper]](https://arxiv.org/abs/2408.16930) ![](https://img.shields.io/badge/year-2024-red)
* DHO: Simple yet Effective Semi-supervised Knowledge Distillation from Vision-Language Models via Dual-Head Optimization [[Paper]](https://arxiv.org/abs/2505.07675) ![](https://img.shields.io/badge/year-2025-red)
* MoPD: Mixture-of-Prompts Distillation for Vision-Language Models [[Paper]](https://doi.org/10.1109/TMM.2025.3645615) ![](https://img.shields.io/badge/year-2026-red)
* Switch-KD: Visual-Switch KD for Vision-Language Models [[Paper]](https://arxiv.org/abs/2604.14629) ![](https://img.shields.io/badge/year-2026-red)
* Prompt-stable knowledge distillation of vision-language models for efficient waste classification in material recovery facilities [[Paper]](https://www.sciencedirect.com/science/article/pii/S0921344926001096) ![](https://img.shields.io/badge/year-2026-red)
* Visual-Language Model Knowledge Distillation Method for Image Quality Assessment [[Paper]](https://arxiv.org/abs/2507.15680) ![](https://img.shields.io/badge/year-2025-red)
* Hide to See: Reasoning-prefix Masking for Visual-anchored Thinking in VLM Distillation [[Paper]](https://arxiv.org/abs/2605.11651) ![](https://img.shields.io/badge/year-2026-red)
* Gated Relational Alignment via Confidence-based Distillation for Efficient VLMs [[Paper]](https://arxiv.org/abs/2601.22709) ![](https://img.shields.io/badge/year-2026-red)
* Large Language Model Teaches Visual Students: Cross-Modality Transfer of Fine-Grained Conceptual Knowledge [[Paper]](https://icml.cc/virtual/2026/poster/66244) ![](https://img.shields.io/badge/year-2026-red)
* Cross-Modal Knowledge Distillation without Paired Data: Theoretical Foundation and Algorithm [[Paper]](https://icml.cc/virtual/2026/poster/60546) ![](https://img.shields.io/badge/year-2026-red)

**Sequence Distillation**

* MASSV: Multimodal Adaptation and Self-Data Distillation for Speculative Decoding of Vision-Language Models [[Paper]](https://arxiv.org/abs/2505.10526) ![](https://img.shields.io/badge/year-2025-red)
* VLM-KD: Knowledge Distillation from VLM for Long-Tail Visual Recognition [[Paper]](https://arxiv.org/abs/2408.16930) ![](https://img.shields.io/badge/year-2024-red)
* Visual Program Distillation: Distilling Tools and Programmatic Reasoning into Vision-Language Models [[Paper]](https://arxiv.org/abs/2312.03052) ![](https://img.shields.io/badge/year-2024-red)
* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)
* Refined Policy Distillation: From VLA Generalists to RL Experts [[Paper]](https://arxiv.org/abs/2503.05833) ![](https://img.shields.io/badge/year-2025-red)
* RDT2: Exploring the Scaling Limit of UMI Data Towards Zero-Shot Cross-Embodiment Generalization [[Paper]](https://arxiv.org/abs/2602.03310) ![](https://img.shields.io/badge/year-2026-red)
* Online In-Context Distillation for Low-Resource Vision Language Models [[Paper]](https://arxiv.org/abs/2510.18117) ![](https://img.shields.io/badge/year-2025-red)
* Towards Long-window Anchoring in Vision-Language Model Distillation [[Paper]](https://arxiv.org/abs/2512.21576) ![](https://img.shields.io/badge/year-2025-red)

**Preference Distillation**

* LLaVA-MoD: Making LLaVA Tiny via MoE Knowledge Distillation [[Paper]](https://arxiv.org/abs/2408.15881) ![](https://img.shields.io/badge/year-2024-red)
* mDPO: Conditional Preference Optimization for Multimodal Large Language Models [[Paper]](https://aclanthology.org/2024.emnlp-main.460/) ![](https://img.shields.io/badge/year-2024-red)
* Embedding the Teacher: Distilling vLLM Preferences for Scalable Image Retrieval [[Paper]](https://arxiv.org/abs/2510.12014) ![](https://img.shields.io/badge/year-2025-red)
* Silkie: Preference Distillation for Large Visual Language Models [[Paper]](https://arxiv.org/abs/2312.10665) ![](https://img.shields.io/badge/year-2023-red)

## Section II: Feature-based Distillation

**Hidden-state Distillation**

* Layerwised Multimodal Knowledge Distillation for Vision-Language Pretrained Model [[Paper]](https://www.sciencedirect.com/science/article/abs/pii/S0893608024001965) ![](https://img.shields.io/badge/year-2024-red)
* KD-VLP: Improving End-to-End Vision-and-Language Pretraining with Object Knowledge Distillation [[Paper]](https://arxiv.org/abs/2109.10504) ![](https://img.shields.io/badge/year-2022-red)
* Building Vision-Language Models on Solid Foundations with Masked Distillation [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Sameni_Building_Vision-Language_Models_on_Solid_Foundations_with_Masked_Distillation_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* TinyViT: Fast Pretraining Distillation for Small Vision Transformers [[Paper]](https://arxiv.org/abs/2207.10666) ![](https://img.shields.io/badge/year-2022-red)
* Compressing Visual-Linguistic Model via Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.02096) ![](https://img.shields.io/badge/year-2021-red)
* MiniVLM: A Smaller and Faster Vision-Language Model [[Paper]](https://arxiv.org/abs/2012.06946) ![](https://img.shields.io/badge/year-2021-red)
* VITA-VLA: Efficiently Teaching Vision-Language Models to Act via Action Expert Distillation [[Paper]](https://arxiv.org/abs/2510.09607) ![](https://img.shields.io/badge/year-2025-red)
* Shallow-pi: Knowledge Distillation for Flow-based VLAs [[Paper]](https://arxiv.org/abs/2601.20262) ![](https://img.shields.io/badge/year-2026-red)
* CEED-VLA: Consistency Vision-Language-Action Model with Early-Exit Decoding [[Paper]](https://arxiv.org/abs/2506.13725) ![](https://img.shields.io/badge/year-2025-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2023-red)
* MaskCLIP: Masked Self-Distillation Advances Contrastive Language-Image Pretraining [[Paper]](https://openaccess.thecvf.com/content/CVPR2023/papers/Dong_MaskCLIP_Masked_Self-Distillation_Advances_Contrastive_Language-Image_Pretraining_CVPR_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* FineCLIP: Self-distilled Region-based CLIP for Better Fine-grained Understanding [[Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/3122aaa22b2fe83f9cead1a696f65ceb-Paper-Conference.pdf) ![](https://img.shields.io/badge/year-2024-red)
* LP-OVOD: Open-Vocabulary Object Detection by Linear Probing [[Paper]](https://arxiv.org/abs/2310.17109) ![](https://img.shields.io/badge/year-2024-red)
* Distilling Large Vision-Language Model with Out-of-Distribution Generalizability [[Paper]](https://openaccess.thecvf.com/content/ICCV2023/papers/Li_Distilling_Large_Vision-Language_Model_with_Out-of-Distribution_Generalizability_ICCV_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* Masking Teacher and Reinforcing Student for Distilling Vision-Language Models [[Paper]](https://arxiv.org/abs/2512.22238) ![](https://img.shields.io/badge/year-2025-red)
* PracticalDG: Perturbation Distillation on Vision-Language Models for Hybrid Domain Generalization [[Paper]](https://arxiv.org/abs/2404.09011) ![](https://img.shields.io/badge/year-2024-red)
* DLIP: Distilling Language-Image Pre-training [[Paper]](https://arxiv.org/abs/2308.12956) ![](https://img.shields.io/badge/year-2023-red)
* Distilling Knowledge from Caption-Guided Replay for VLM-Based Continual Learning [[Paper]](https://openreview.net/forum?id=HN18kuyf4o) ![](https://img.shields.io/badge/year-2026-red)
* LinMU: Multimodal Understanding Made Linear [[Paper]](https://arxiv.org/pdf/2601.01322) ![](https://img.shields.io/badge/year-2026-red)
* Prodistill: A Progressive Prompting Framework for Fine-Grained VLM Distillation [[Paper]](https://ieeexplore.ieee.org/document/11461281/) ![](https://img.shields.io/badge/year-2026-red)
* Drive-KD: Multi-Teacher Distillation for VLMs in Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.21288) ![](https://img.shields.io/badge/year-2026-red)
* SF-CLIP: CLIP-based Arbitrary Style Image Retrieval with Style and Fine-Grained Semantic Enhancement [[Paper]](https://doi.org/10.1109/ICASSP55912.2026.11461615) ![](https://img.shields.io/badge/year-2026-red)

**Attention Distillation**

* CompoDistill: Attention Distillation for Compositional Reasoning in Multimodal LLMs [[Paper]](https://arxiv.org/abs/2510.12184) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://openreview.net/pdf?id=xsCK546dra) ![](https://img.shields.io/badge/year-2024-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://arxiv.org/abs/2309.12314) ![](https://img.shields.io/badge/year-2023-red)
* AC^2-VLA: Action-Context-Aware Adaptive Computation in Vision-Language-Action Models for Efficient Robotic Manipulation [[Paper]](https://arxiv.org/abs/2601.19634) ![](https://img.shields.io/badge/year-2026-red)
* DeCLIP: Decoupled Learning for Open-Vocabulary Dense Perception [[Paper]](https://arxiv.org/abs/2505.04410) ![](https://img.shields.io/badge/year-2025-red)
* DIDE: Distilled Dual-Encoder Model for Vision-Language Understanding [[Paper]](https://doi.org/10.18653/v1/2022.emnlp-main.608) ![](https://img.shields.io/badge/year-2022-red)
* DLIP: Distilling Language-Image Pre-training [[Paper]](https://arxiv.org/abs/2308.12956) ![](https://img.shields.io/badge/year-2023-red)
* Drive-KD: Multi-Teacher Distillation for VLMs in Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.21288) ![](https://img.shields.io/badge/year-2026-red)

**Cross-modal Feature Distillation**

* EM-KD: Distilling Efficient Multimodal Large Language Model with Unbalanced Vision Tokens [[Paper]](https://arxiv.org/pdf/2511.21106) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://openreview.net/pdf?id=xsCK546dra) ![](https://img.shields.io/badge/year-2024-red)
* Modality-specific Knowledge Distillation with Wasserstein Distance Minimization for Vision-Language Pretrained Models [[Paper]](https://ieeexplore.ieee.org/document/11178237) ![](https://img.shields.io/badge/year-2025-red)
* Multimodal Adaptive Distillation for Leveraging Unimodal Encoders for Vision-Language Tasks [[Paper]](https://arxiv.org/abs/2204.10496) ![](https://img.shields.io/badge/year-2022-red)
* Unsupervised Knowledge Distillation via Local Representations for Vision-Language Models [[Paper]](https://ieeexplore.ieee.org/document/11048580) ![](https://img.shields.io/badge/year-2025-red)
* TE-VLM: Transfer Entropy for Vision Language Model Distillation [[Paper]](https://openreview.net/forum?id=vJV22Ig8YG) ![](https://img.shields.io/badge/year-2025-red)
* KAID: Knowledge-Aware Interactive Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/paper/KAID%3A-Knowledge-Aware-Interactive-Distillation-for-Zhang-Wang/30af36e012240ef4402b57230c109900f49f7102) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* FD-VLA: Force-Distilled Vision-Language-Action Model for Contact-Rich Manipulation [[Paper]](https://arxiv.org/abs/2602.02142) ![](https://img.shields.io/badge/year-2026-red)
* VISTA: Enhancing Visual Conditioning via Track-Following Preference Optimization in Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2602.05049) ![](https://img.shields.io/badge/year-2026-red)
* OmniReason: A Temporal-Guided Vision-Language-Action Framework for Autonomous Driving [[Paper]](https://arxiv.org/abs/2509.00789) ![](https://img.shields.io/badge/year-2025-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2203.10593) ![](https://img.shields.io/badge/year-2022-red)
* Object-Aware Distillation Pyramid for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2303.05892) ![](https://img.shields.io/badge/year-2023-red)
* Learning Background Prompts to Discover Implicit Knowledge for Open Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2406.00510) ![](https://img.shields.io/badge/year-2024-red)
* SKDF: A Simple Knowledge Distillation Framework for Distilling Open-Vocabulary Knowledge to Open-World Object Detector [[Paper]](https://arxiv.org/abs/2312.08653) ![](https://img.shields.io/badge/year-2024-red)
* AME: Aligned Manifold Entropy for Robust Vision-Language Distillation [[Paper]](https://arxiv.org/abs/2508.08644) ![](https://img.shields.io/badge/year-2025-red)
* PartDistill: 3D Shape Part Segmentation by Vision-Language Model Distillation [[Paper]](https://arxiv.org/abs/2312.04016) ![](https://img.shields.io/badge/year-2024-red)
* VLScene: Vision-language guidance distillation for camera-based 3D semantic scene completion [[Paper]](https://arxiv.org/abs/2503.06219) ![](https://img.shields.io/badge/year-2025-red)
* 3D-aware vision-language models fine-tuning with geometric distillation [[Paper]](https://arxiv.org/abs/2506.09883) ![](https://img.shields.io/badge/year-2025-red)
* cViL: Cross-Lingual Training of Vision-Language Models using Knowledge Distillation [[Paper]](https://doi.org/10.1109/ICPR56361.2022.9956259) ![](https://img.shields.io/badge/year-2022-red)
* Prompt-stable knowledge distillation of vision-language models for efficient waste classification in material recovery facilities [[Paper]](https://www.sciencedirect.com/science/article/pii/S0921344926001096) ![](https://img.shields.io/badge/year-2026-red)
* Visual-Language Model Knowledge Distillation Method for Image Quality Assessment [[Paper]](https://arxiv.org/abs/2507.15680) ![](https://img.shields.io/badge/year-2025-red)
* FLARE: Learning Future-Aware Latent Representations from Vision-Language Models for Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.05611) ![](https://img.shields.io/badge/year-2026-red)
* DAIT: Distillation from Vision-Language Models to Lightweight Classifiers with Adaptive Intermediate Teacher Transfer [[Paper]](https://arxiv.org/pdf/2603.15166) ![](https://img.shields.io/badge/year-2026-red)
* HieRD: Hierarchical Relational Distillation for Vision-Language Embedding Models [[Paper]](https://icml.cc/virtual/2026/poster/63112) ![](https://img.shields.io/badge/year-2026-red)
* Cross-Modal Knowledge Distillation without Paired Data: Theoretical Foundation and Algorithm [[Paper]](https://icml.cc/virtual/2026/poster/60546) ![](https://img.shields.io/badge/year-2026-red)

## Section III: Relation-based Distillation

**Similarity-based Distillation**

* CLIP-KD: An Empirical Study of CLIP Model Distillation [[Paper]](https://arxiv.org/abs/2307.12732) ![](https://img.shields.io/badge/year-2023-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://arxiv.org/abs/2309.12314) ![](https://img.shields.io/badge/year-2023-red)
* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://arxiv.org/abs/2311.17049) ![](https://img.shields.io/badge/year-2024-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_PromptKD_Unsupervised_Prompt_Distillation_for_Vision-Language_Models_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-Embed-KD: Computationally Efficient Knowledge Distillation Using Embeddings as Teachers [[Paper]](https://arxiv.org/abs/2404.06170) ![](https://img.shields.io/badge/year-2024-red)
* Filtering, Distillation, and Hard Negatives for Vision-Language Pre-Training [[Paper]](https://arxiv.org/abs/2301.02280) ![](https://img.shields.io/badge/year-2023-red)
* Open-Vocabulary Object Detection via Vision and Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.13921) ![](https://img.shields.io/badge/year-2022-red)
* DIME-FM: Distilling Multimodal and Efficient Foundation Models [[Paper]](https://arxiv.org/abs/2303.18232) ![](https://img.shields.io/badge/year-2023-red)
* Gated Relational Alignment via Confidence-based Distillation for Efficient VLMs [[Paper]](https://arxiv.org/abs/2601.22709) ![](https://img.shields.io/badge/year-2026-red)
* Learning From Expert: Vision-Language Knowledge Distillation for Unsupervised Cross-Modal Hashing Retrieval [[Paper]](https://doi.org/10.1145/3591106.3592242) ![](https://img.shields.io/badge/year-2023-red)
* HieRD: Hierarchical Relational Distillation for Vision-Language Embedding Models [[Paper]](https://icml.cc/virtual/2026/poster/63112) ![](https://img.shields.io/badge/year-2026-red)

**Contrastive Distillation**

* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://arxiv.org/abs/2311.17049) ![](https://img.shields.io/badge/year-2024-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_PromptKD_Unsupervised_Prompt_Distillation_for_Vision-Language_Models_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-CID: Efficient CLIP Distillation via Cluster-Instance Discrimination [[Paper]](https://doi.org/10.1609/aaai.v39i20.35505) ![](https://img.shields.io/badge/year-2025-red)
* Filtering, Distillation, and Hard Negatives for Vision-Language Pre-Training [[Paper]](https://arxiv.org/abs/2301.02280) ![](https://img.shields.io/badge/year-2023-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://arxiv.org/abs/2309.12314) ![](https://img.shields.io/badge/year-2023-red)
* A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance [[Paper]](https://arxiv.org/abs/2309.12530) ![](https://img.shields.io/badge/year-2023-red)
* Distilling CLIP with Dual Guidance for Learning Discriminative Human Body Shape Representation [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_Distilling_CLIP_with_Dual_Guidance_for_Learning_Discriminative_Human_Body_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* Enabling Multimodal Generation on CLIP via Vision-Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2203.06386) ![](https://img.shields.io/badge/year-2022-red)
* Aligning Bag of Regions for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2302.13996) ![](https://img.shields.io/badge/year-2023-red)
* Cyclic Contrastive Knowledge Transfer for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2503.11005) ![](https://img.shields.io/badge/year-2025-red)
* Exploring Multi-Modal Contextual Knowledge for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2308.15846) ![](https://img.shields.io/badge/year-2023-red)
* VLDadaptor: Domain Adaptive Object Detection with Vision-Language Model Distillation [[Paper]](https://ieeexplore.ieee.org/document/10669066) ![](https://img.shields.io/badge/year-2024-red)
* Adversarial prompt distillation for vision-language models [[Paper]](https://arxiv.org/abs/2411.15244) ![](https://img.shields.io/badge/year-2024-red)
* Dynamic contrastive distillation for image-text retrieval [[Paper]](https://arxiv.org/abs/2207.01426) ![](https://img.shields.io/badge/year-2023-red)

## Teacher Accessibility

<p align="left">
  <img src="./Figure/Figure_3.jpg" alt="Teacher accessibility view of VLM distillation" width="600">
</p>

| Regime | Section |
|---|---|
| White-box Distillation  | [Section IV](#section-iv-white-box-distillation) |
| Black-box Distillation  | [Section V](#section-v-black-box-distillation) |
| Self-Distillation | [Section VI](#section-vi-self-distillation) |
| Multi-teacher Distillation  | [Section VII](#section-vii-multi-teacher-distillation) |

## Section IV: White-box Distillation

* Layerwised Multimodal Knowledge Distillation for Vision-Language Pretrained Model [[Paper]](https://www.sciencedirect.com/science/article/abs/pii/S0893608024001965) ![](https://img.shields.io/badge/year-2024-red)
* KD-VLP: Improving End-to-End Vision-and-Language Pretraining with Object Knowledge Distillation [[Paper]](https://arxiv.org/abs/2109.10504) ![](https://img.shields.io/badge/year-2022-red)
* CompoDistill: Attention Distillation for Compositional Reasoning in Multimodal LLMs [[Paper]](https://arxiv.org/abs/2510.12184) ![](https://img.shields.io/badge/year-2025-red)
* Align-KD: Distilling Cross-Modal Alignment Knowledge for Mobile Vision-Language Model [[Paper]](https://openreview.net/pdf?id=xsCK546dra) ![](https://img.shields.io/badge/year-2024-red)
* VLsI: Verbalized Layers-to-Interactions from Large to Small Vision Language Models [[Paper]](https://arxiv.org/abs/2412.01822) ![](https://img.shields.io/badge/year-2025-red)
* EM-KD: Distilling Efficient Multimodal Large Language Model with Unbalanced Vision Tokens [[Paper]](https://arxiv.org/pdf/2511.21106) ![](https://img.shields.io/badge/year-2025-red)
* Modality-specific Knowledge Distillation with Wasserstein Distance Minimization for Vision-Language Pretrained Models [[Paper]](https://ieeexplore.ieee.org/document/11178237) ![](https://img.shields.io/badge/year-2025-red)
* TE-VLM: Transfer Entropy for Vision Language Model Distillation [[Paper]](https://openreview.net/forum?id=vJV22Ig8YG) ![](https://img.shields.io/badge/year-2025-red)
* KAID: Knowledge-Aware Interactive Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/paper/KAID%3A-Knowledge-Aware-Interactive-Distillation-for-Zhang-Wang/30af36e012240ef4402b57230c109900f49f7102) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* Shallow-pi: Knowledge Distillation for Flow-based VLAs [[Paper]](https://arxiv.org/abs/2601.20262) ![](https://img.shields.io/badge/year-2026-red)
* Aligning Bag of Regions for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2302.13996) ![](https://img.shields.io/badge/year-2023-red)
* 3D-aware vision-language models fine-tuning with geometric distillation [[Paper]](https://arxiv.org/abs/2506.09883) ![](https://img.shields.io/badge/year-2025-red)
* CLIP-TD: CLIP targeted distillation for vision-language tasks [[Paper]](https://arxiv.org/abs/2201.05729) ![](https://img.shields.io/badge/year-2022-red)
* DIDE: Distilled Dual-Encoder Model for Vision-Language Understanding [[Paper]](https://doi.org/10.18653/v1/2022.emnlp-main.608) ![](https://img.shields.io/badge/year-2022-red)
* CLIPPING: Distilling CLIP-Based Models with a Student Base for Video-Language Retrieval [[Paper]](https://openaccess.thecvf.com/content/CVPR2023/papers/Pei_CLIPPING_Distilling_CLIP-Based_Models_With_a_Student_Base_for_Video-Language_CVPR_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* MoPD: Mixture-of-Prompts Distillation for Vision-Language Models [[Paper]](https://doi.org/10.1109/TMM.2025.3645615) ![](https://img.shields.io/badge/year-2026-red)
* Distilling Knowledge from Caption-Guided Replay for VLM-Based Continual Learning [[Paper]](https://openreview.net/forum?id=HN18kuyf4o) ![](https://img.shields.io/badge/year-2026-red)
* Prompt-stable knowledge distillation of vision-language models for efficient waste classification in material recovery facilities [[Paper]](https://www.sciencedirect.com/science/article/pii/S0921344926001096) ![](https://img.shields.io/badge/year-2026-red)
* Visual-Language Model Knowledge Distillation Method for Image Quality Assessment [[Paper]](https://arxiv.org/abs/2507.15680) ![](https://img.shields.io/badge/year-2025-red)
* LinMU: Multimodal Understanding Made Linear [[Paper]](https://arxiv.org/pdf/2601.01322) ![](https://img.shields.io/badge/year-2026-red)
* FLARE: Learning Future-Aware Latent Representations from Vision-Language Models for Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.05611) ![](https://img.shields.io/badge/year-2026-red)
* DAIT: Distillation from Vision-Language Models to Lightweight Classifiers with Adaptive Intermediate Teacher Transfer [[Paper]](https://arxiv.org/pdf/2603.15166) ![](https://img.shields.io/badge/year-2026-red)
* Hide to See: Reasoning-prefix Masking for Visual-anchored Thinking in VLM Distillation [[Paper]](https://arxiv.org/abs/2605.11651) ![](https://img.shields.io/badge/year-2026-red)
* Prodistill: A Progressive Prompting Framework for Fine-Grained VLM Distillation [[Paper]](https://ieeexplore.ieee.org/document/11461281/) ![](https://img.shields.io/badge/year-2026-red)
* HieRD: Hierarchical Relational Distillation for Vision-Language Embedding Models [[Paper]](https://icml.cc/virtual/2026/poster/63112) ![](https://img.shields.io/badge/year-2026-red)
* Gated Relational Alignment via Confidence-based Distillation for Efficient VLMs [[Paper]](https://arxiv.org/abs/2601.22709) ![](https://img.shields.io/badge/year-2026-red)
* Cross-Modal Knowledge Distillation without Paired Data: Theoretical Foundation and Algorithm [[Paper]](https://icml.cc/virtual/2026/poster/60546) ![](https://img.shields.io/badge/year-2026-red)
* SF-CLIP: CLIP-based Arbitrary Style Image Retrieval with Style and Fine-Grained Semantic Enhancement [[Paper]](https://doi.org/10.1109/ICASSP55912.2026.11461615) ![](https://img.shields.io/badge/year-2026-red)

## Section V: Black-box Distillation

* Visual Program Distillation: Distilling Tools and Programmatic Reasoning into Vision-Language Models [[Paper]](https://arxiv.org/abs/2312.03052) ![](https://img.shields.io/badge/year-2024-red)
* ShareGPT4V: Improving Large Multi-Modal Models with Better Captions [[Paper]](https://arxiv.org/abs/2311.12793) ![](https://img.shields.io/badge/year-2023-red)
* MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models [[Paper]](https://arxiv.org/abs/2304.10592) ![](https://img.shields.io/badge/year-2023-red)
* ALLaVA: Harnessing GPT4V-Synthesized Data for Lite Vision-Language Models [[Paper]](https://arxiv.org/abs/2402.11684) ![](https://img.shields.io/badge/year-2024-red)
* PCoreSet: Effective Active Learning through Knowledge Distillation from Vision-Language Models [[Paper]](https://arxiv.org/abs/2506.00910) ![](https://img.shields.io/badge/year-2025-red)
* CLIP-Embed-KD: Computationally Efficient Knowledge Distillation Using Embeddings as Teachers [[Paper]](https://arxiv.org/abs/2404.06170) ![](https://img.shields.io/badge/year-2024-red)
* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2203.10593) ![](https://img.shields.io/badge/year-2022-red)
* Bridging the Gap between Object and Image-Level Representations for Open-Vocabulary Detection [[Paper]](https://arxiv.org/abs/2207.03482) ![](https://img.shields.io/badge/year-2022-red)
* LVLM2P: Sample Efficient Reinforcement Learning via Large Vision Language Model Distillation [[Paper]](https://doi.org/10.1109/ICASSP49660.2025.10888998) ![](https://img.shields.io/badge/year-2025-red)
* Online In-Context Distillation for Low-Resource Vision Language Models [[Paper]](https://arxiv.org/abs/2510.18117) ![](https://img.shields.io/badge/year-2025-red)
* Switch-KD: Visual-Switch KD for Vision-Language Models [[Paper]](https://arxiv.org/abs/2604.14629) ![](https://img.shields.io/badge/year-2026-red)
* Large Language Model Teaches Visual Students: Cross-Modality Transfer of Fine-Grained Conceptual Knowledge [[Paper]](https://icml.cc/virtual/2026/poster/66244) ![](https://img.shields.io/badge/year-2026-red)

## Section VI: Self-Distillation

* COSMOS: Cross-Modality Self-Distillation for Vision Language Pre-training [[Paper]](https://arxiv.org/abs/2412.01814) ![](https://img.shields.io/badge/year-2025-red)
* Align before Fuse: Vision and Language Representation Learning with Momentum Distillation [[Paper]](https://arxiv.org/abs/2107.07651) ![](https://img.shields.io/badge/year-2021-red)
* Building Vision-Language Models on Solid Foundations with Masked Distillation [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Sameni_Building_Vision-Language_Models_on_Solid_Foundations_with_Masked_Distillation_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* MaskCLIP: Masked Self-Distillation Advances Contrastive Language-Image Pretraining [[Paper]](https://openaccess.thecvf.com/content/CVPR2023/papers/Dong_MaskCLIP_Masked_Self-Distillation_Advances_Contrastive_Language-Image_Pretraining_CVPR_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* FineCLIP: Self-distilled Region-based CLIP for Better Fine-grained Understanding [[Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/3122aaa22b2fe83f9cead1a696f65ceb-Paper-Conference.pdf) ![](https://img.shields.io/badge/year-2024-red)
* Improving Zero-Shot Generalization of Learned Prompts via Unsupervised Knowledge Distillation [[Paper]](https://arxiv.org/abs/2407.03056) ![](https://img.shields.io/badge/year-2024-red)
* Self-Improving Vision-Language-Action Models with Data Generation via Residual RL [[Paper]](https://arxiv.org/abs/2511.00091) ![](https://img.shields.io/badge/year-2025-red)
* MoLe-VLA: Dynamic Layer-Skipping Vision Language Action Model via Mixture-of-Layers for Efficient Robot Manipulation [[Paper]](https://arxiv.org/abs/2503.20384) ![](https://img.shields.io/badge/year-2025-red)
* CEED-VLA: Consistency Vision-Language-Action Model with Early-Exit Decoding [[Paper]](https://arxiv.org/abs/2506.13725) ![](https://img.shields.io/badge/year-2025-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2023-red)
* Multimodality Self-distillation for Fast Inference of Vision and Language Pretrained Models [[Paper]](https://ieeexplore.ieee.org/document/10487847) ![](https://img.shields.io/badge/year-2024-red)

## Section VII: Multi-teacher Distillation

* MoVE-KD: Knowledge Distillation for VLMs with Mixture of Visual Encoders [[Paper]](https://arxiv.org/abs/2501.01709) ![](https://img.shields.io/badge/year-2025-red)
* MST-Distill: Mixture of Specialized Teachers for Cross-Modal Knowledge Distillation [[Paper]](https://arxiv.org/abs/2507.07015) ![](https://img.shields.io/badge/year-2025-red)
* AMMKD: Adaptive Multimodal Multi-Teacher Distillation for Lightweight Vision-Language Models [[Paper]](https://arxiv.org/abs/2509.00039) ![](https://img.shields.io/badge/year-2025-red)
* Retaining Knowledge and Enhancing Long-Text Representations in CLIP through Dual-Teacher Distillation [[Paper]](https://openaccess.thecvf.com/content/CVPR2025/papers/Feng_Retaining_Knowledge_and_Enhancing_Long-Text_Representations_in_CLIP_through_Dual-Teacher_CVPR_2025_paper.pdf) ![](https://img.shields.io/badge/year-2025-red)
* KAID: Knowledge-Aware Interactive Distillation for Vision-Language Models [[Paper]](https://www.semanticscholar.org/paper/KAID%3A-Knowledge-Aware-Interactive-Distillation-for-Zhang-Wang/30af36e012240ef4402b57230c109900f49f7102) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)
* Drive-KD: Multi-Teacher Distillation for VLMs in Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.21288) ![](https://img.shields.io/badge/year-2026-red)

## Structural Compatibility

<p align="left">
  <img src="./Figure/Figure_4.jpg" alt="Structural compatibility view of VLM distillation" width="600">
</p>

| Type | Section |
|---|---|
| Isomorphic | [Section VIII](#section-viii-structural-compatibility---isomorphic) |
| Cross-Architecture | [Section IX](#section-ix-structural-compatibility---cross-architecture) |
| Cross-Modal | [Section X](#section-x-structural-compatibility---cross-modal) |

## Section VIII: Structural Compatibility - Isomorphic

* LLaVA-KD: A Framework of Distilling Multimodal Large Language Models [[Paper]](https://openaccess.thecvf.com/content/ICCV2025/papers/Cai_LLaVA-KD_A_Framework_of_Distilling_Multimodal_Large_Language_Models_ICCV_2025_paper.pdf) ![](https://img.shields.io/badge/year-2025-red)
* VLsI: Verbalized Layers-to-Interactions from Large to Small Vision Language Models [[Paper]](https://arxiv.org/abs/2412.01822) ![](https://img.shields.io/badge/year-2025-red)
* MASSV: Multimodal Adaptation and Self-Data Distillation for Speculative Decoding of Vision-Language Models [[Paper]](https://arxiv.org/abs/2505.10526) ![](https://img.shields.io/badge/year-2025-red)
* Select and Distill: Selective Dual-Teacher Knowledge Transfer for Continual Learning on Vision-Language Models [[Paper]](https://arxiv.org/abs/2403.09296) ![](https://img.shields.io/badge/year-2024-red)
* Collaborative Training of Tiny-Large Vision Language Models [[Paper]](https://openreview.net/pdf?id=Ugy9DyhYYD) ![](https://img.shields.io/badge/year-2024-red)
* CLIP-KD: An Empirical Study of CLIP Model Distillation [[Paper]](https://arxiv.org/abs/2307.12732) ![](https://img.shields.io/badge/year-2023-red)
* TinyCLIP: CLIP Distillation via Affinity Mimicking and Weight Inheritance [[Paper]](https://arxiv.org/abs/2309.12314) ![](https://img.shields.io/badge/year-2023-red)
* CLIP-CID: Efficient CLIP Distillation via Cluster-Instance Discrimination [[Paper]](https://doi.org/10.1609/aaai.v39i20.35505) ![](https://img.shields.io/badge/year-2025-red)
* CLIP-Embed-KD: Computationally Efficient Knowledge Distillation Using Embeddings as Teachers [[Paper]](https://arxiv.org/abs/2404.06170) ![](https://img.shields.io/badge/year-2024-red)
* PromptKD: Unsupervised Prompt Distillation for Vision-Language Models [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_PromptKD_Unsupervised_Prompt_Distillation_for_Vision-Language_Models_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* Self-Improving Vision-Language-Action Models with Data Generation via Residual RL [[Paper]](https://arxiv.org/abs/2511.00091) ![](https://img.shields.io/badge/year-2025-red)
* FT-NCFM: An Influence-Aware Data Distillation Framework for Efficient VLA Models [[Paper]](https://arxiv.org/abs/2511.16233) ![](https://img.shields.io/badge/year-2025-red)
* DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action [[Paper]](https://arxiv.org/abs/2511.22134) ![](https://img.shields.io/badge/year-2025-red)
* Open-Vocabulary Object Detection via Vision and Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.13921) ![](https://img.shields.io/badge/year-2022-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2203.10593) ![](https://img.shields.io/badge/year-2022-red)
* Distilling DETR with Visual-Linguistic Knowledge for Open-Vocabulary Object Detection [[Paper]](https://openaccess.thecvf.com/content/ICCV2023/papers/Li_Distilling_DETR_with_Visual-Linguistic_Knowledge_for_Open-Vocabulary_Object_Detection_ICCV_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* A Hierarchical Semantic Distillation Framework for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2503.10152) ![](https://img.shields.io/badge/year-2025-red)
* CAKE: Category Aware Knowledge Extraction for Open-Vocabulary Object Detection [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/32639)
* DIME-FM: Distilling Multimodal and Efficient Foundation Models [[Paper]](https://arxiv.org/abs/2303.18232) ![](https://img.shields.io/badge/year-2023-red)
* CLIPPING: Distilling CLIP-Based Models with a Student Base for Video-Language Retrieval [[Paper]](https://openaccess.thecvf.com/content/CVPR2023/papers/Pei_CLIPPING_Distilling_CLIP-Based_Models_With_a_Student_Base_for_Video-Language_CVPR_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* Online In-Context Distillation for Low-Resource Vision Language Models [[Paper]](https://arxiv.org/abs/2510.18117) ![](https://img.shields.io/badge/year-2025-red)
* Distilling Knowledge from Caption-Guided Replay for VLM-Based Continual Learning [[Paper]](https://openreview.net/forum?id=HN18kuyf4o) ![](https://img.shields.io/badge/year-2026-red)
* Switch-KD: Visual-Switch KD for Vision-Language Models [[Paper]](https://arxiv.org/abs/2604.14629) ![](https://img.shields.io/badge/year-2026-red)
* Gated Relational Alignment via Confidence-based Distillation for Efficient VLMs [[Paper]](https://arxiv.org/abs/2601.22709) ![](https://img.shields.io/badge/year-2026-red)
* Hide to See: Reasoning-prefix Masking for Visual-anchored Thinking in VLM Distillation [[Paper]](https://arxiv.org/abs/2605.11651) ![](https://img.shields.io/badge/year-2026-red)

## Section IX: Structural Compatibility - Cross-Architecture

* TinyViT: Fast Pretraining Distillation for Small Vision Transformers [[Paper]](https://arxiv.org/abs/2207.10666) ![](https://img.shields.io/badge/year-2022-red)
* MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training [[Paper]](https://arxiv.org/abs/2311.17049) ![](https://img.shields.io/badge/year-2024-red)
* Generative Negative Text Replay for Continual Vision-Language Pretraining [[Paper]](https://arxiv.org/abs/2210.17322) ![](https://img.shields.io/badge/year-2022-red)
* LLaVA-MoD: Making LLaVA Tiny via MoE Knowledge Distillation [[Paper]](https://arxiv.org/abs/2408.15881) ![](https://img.shields.io/badge/year-2024-red)
* MiniVLM: A Smaller and Faster Vision-Language Model [[Paper]](https://arxiv.org/abs/2012.06946) ![](https://img.shields.io/badge/year-2021-red)
* VL2Lite: Task-Specific Knowledge Distillation from Large Vision-Language Models to Lightweight Networks [[Paper]](https://openaccess.thecvf.com/content/CVPR2025/papers/Jang_VL2Lite_Task-Specific_Knowledge_Distillation_from_Large_Vision-Language_Models_to_Lightweight_CVPR_2025_paper.pdf) ![](https://img.shields.io/badge/year-2025-red)
* CustomKD: Customizing Large Vision Foundation for Edge Model Improvement via Knowledge Distillation [[Paper]](https://arxiv.org/abs/2503.18244) ![](https://img.shields.io/badge/year-2025-red)
* EfficientVLM: Fast and Accurate Vision-Language Models via Knowledge Distillation and Modal-Adaptive Pruning [[Paper]](https://arxiv.org/abs/2210.07795) ![](https://img.shields.io/badge/year-2023-red)
* CIFD: Controlled Information Flow to Enhance Knowledge Distillation [[Paper]](https://openreview.net/forum?id=xutrKezbPF) ![](https://img.shields.io/badge/year-2024-red)
* RLDG: Robotic Generalist Policy Distillation via Reinforcement Learning [[Paper]](https://arxiv.org/abs/2412.09858) ![](https://img.shields.io/badge/year-2024-red)
* VITA-VLA: Efficiently Teaching Vision-Language Models to Act via Action Expert Distillation [[Paper]](https://arxiv.org/abs/2510.09607) ![](https://img.shields.io/badge/year-2025-red)
* Refined Policy Distillation: From VLA Generalists to RL Experts [[Paper]](https://arxiv.org/abs/2503.05833) ![](https://img.shields.io/badge/year-2025-red)
* Clip4Retrofit: Enabling real-time image labeling on edge devices via cross-architecture CLIP distillation [[Paper]](https://arxiv.org/abs/2505.18039) ![](https://img.shields.io/badge/year-2025-red)
* Module-wise Adaptive Distillation for Multimodality Foundation Models [[Paper]](https://arxiv.org/abs/2310.04550) ![](https://img.shields.io/badge/year-2023-red)
* LinMU: Multimodal Understanding Made Linear [[Paper]](https://arxiv.org/pdf/2601.01322) ![](https://img.shields.io/badge/year-2026-red)
* Prodistill: A Progressive Prompting Framework for Fine-Grained VLM Distillation [[Paper]](https://ieeexplore.ieee.org/document/11461281/) ![](https://img.shields.io/badge/year-2026-red)
* Drive-KD: Multi-Teacher Distillation for VLMs in Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.21288) ![](https://img.shields.io/badge/year-2026-red)

## Section X: Structural Compatibility - Cross-Modal

* A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance [[Paper]](https://arxiv.org/abs/2309.12530) ![](https://img.shields.io/badge/year-2023-red)
* Enabling Multimodal Generation on CLIP via Vision-Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2203.06386) ![](https://img.shields.io/badge/year-2022-red)
* Distilling CLIP with Dual Guidance for Learning Discriminative Human Body Shape Representation [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_Distilling_CLIP_with_Dual_Guidance_for_Learning_Discriminative_Human_Body_CVPR_2024_paper.pdf) ![](https://img.shields.io/badge/year-2024-red)
* Unsupervised Knowledge Distillation via Local Representations for Vision-Language Models [[Paper]](https://ieeexplore.ieee.org/document/11048580) ![](https://img.shields.io/badge/year-2025-red)
* TE-VLM: Transfer Entropy for Vision Language Model Distillation [[Paper]](https://openreview.net/forum?id=vJV22Ig8YG) ![](https://img.shields.io/badge/year-2025-red)
* GLaD: Geometric Latent Distillation for Vision-Language-Action Models [[Paper]](https://arxiv.org/abs/2512.09619) ![](https://img.shields.io/badge/year-2025-red)
* FD-VLA: Force-Distilled Vision-Language-Action Model for Contact-Rich Manipulation [[Paper]](https://arxiv.org/abs/2602.02142) ![](https://img.shields.io/badge/year-2026-red)
* Bridging the Gap between Object and Image-Level Representations for Open-Vocabulary Detection [[Paper]](https://arxiv.org/abs/2207.03482) ![](https://img.shields.io/badge/year-2022-red)
* Vision-Language-Vision Auto-Encoder: Scalable Knowledge Distillation from Diffusion Models [[Paper]](https://arxiv.org/abs/2507.07104) ![](https://img.shields.io/badge/year-2025-red)
* LVLM2P: Sample Efficient Reinforcement Learning via Large Vision Language Model Distillation [[Paper]](https://doi.org/10.1109/ICASSP49660.2025.10888998) ![](https://img.shields.io/badge/year-2025-red)
* Prompt-stable knowledge distillation of vision-language models for efficient waste classification in material recovery facilities [[Paper]](https://www.sciencedirect.com/science/article/pii/S0921344926001096) ![](https://img.shields.io/badge/year-2026-red)
* Visual-Language Model Knowledge Distillation Method for Image Quality Assessment [[Paper]](https://arxiv.org/abs/2507.15680) ![](https://img.shields.io/badge/year-2025-red)
* FLARE: Learning Future-Aware Latent Representations from Vision-Language Models for Autonomous Driving [[Paper]](https://arxiv.org/abs/2601.05611) ![](https://img.shields.io/badge/year-2026-red)
* DAIT: Distillation from Vision-Language Models to Lightweight Classifiers with Adaptive Intermediate Teacher Transfer [[Paper]](https://arxiv.org/pdf/2603.15166) ![](https://img.shields.io/badge/year-2026-red)
* HieRD: Hierarchical Relational Distillation for Vision-Language Embedding Models [[Paper]](https://icml.cc/virtual/2026/poster/63112) ![](https://img.shields.io/badge/year-2026-red)
* Large Language Model Teaches Visual Students: Cross-Modality Transfer of Fine-Grained Conceptual Knowledge [[Paper]](https://icml.cc/virtual/2026/poster/66244) ![](https://img.shields.io/badge/year-2026-red)
* Cross-Modal Knowledge Distillation without Paired Data: Theoretical Foundation and Algorithm [[Paper]](https://icml.cc/virtual/2026/poster/60546) ![](https://img.shields.io/badge/year-2026-red)
* SF-CLIP: CLIP-based Arbitrary Style Image Retrieval with Style and Fine-Grained Semantic Enhancement [[Paper]](https://doi.org/10.1109/ICASSP55912.2026.11461615) ![](https://img.shields.io/badge/year-2026-red)


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
* Refined Policy Distillation: From VLA Generalists to RL Experts [[Paper]](https://arxiv.org/abs/2503.05833) ![](https://img.shields.io/badge/year-2025-red)
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

* Open-Vocabulary Object Detection via Vision and Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2104.13921) ![](https://img.shields.io/badge/year-2022-red)
* Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation [[Paper]](https://arxiv.org/abs/2203.10593) ![](https://img.shields.io/badge/year-2022-red)
* Bridging the Gap between Object and Image-Level Representations for Open-Vocabulary Detection [[Paper]](https://arxiv.org/abs/2207.03482) ![](https://img.shields.io/badge/year-2022-red)
* CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction [[Paper]](https://arxiv.org/abs/2310.01403) ![](https://img.shields.io/badge/year-2023-red)
* Object-Aware Distillation Pyramid for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2303.05892) ![](https://img.shields.io/badge/year-2023-red)
* Aligning Bag of Regions for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2302.13996) ![](https://img.shields.io/badge/year-2023-red)
* Distilling DETR with Visual-Linguistic Knowledge for Open-Vocabulary Object Detection [[Paper]](https://openaccess.thecvf.com/content/ICCV2023/papers/Li_Distilling_DETR_with_Visual-Linguistic_Knowledge_for_Open-Vocabulary_Object_Detection_ICCV_2023_paper.pdf) ![](https://img.shields.io/badge/year-2023-red)
* DeCLIP: Decoupled Learning for Open-Vocabulary Dense Perception [[Paper]](https://arxiv.org/abs/2505.04410) ![](https://img.shields.io/badge/year-2025-red)
* A Hierarchical Semantic Distillation Framework for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2503.10152) ![](https://img.shields.io/badge/year-2025-red)
* CAKE: Category Aware Knowledge Extraction for Open-Vocabulary Object Detection [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/32639)
* Cyclic Contrastive Knowledge Transfer for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2503.11005) ![](https://img.shields.io/badge/year-2025-red)
* Learning Background Prompts to Discover Implicit Knowledge for Open Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2406.00510) ![](https://img.shields.io/badge/year-2024-red)
* Exploring Multi-Modal Contextual Knowledge for Open-Vocabulary Object Detection [[Paper]](https://arxiv.org/abs/2308.15846) ![](https://img.shields.io/badge/year-2023-red)
* LP-OVOD: Open-Vocabulary Object Detection by Linear Probing [[Paper]](https://arxiv.org/abs/2310.17109) ![](https://img.shields.io/badge/year-2024-red)
* SKDF: A Simple Knowledge Distillation Framework for Distilling Open-Vocabulary Knowledge to Open-World Object Detector [[Paper]](https://arxiv.org/abs/2312.08653) ![](https://img.shields.io/badge/year-2024-red)
* VLDadaptor: Domain Adaptive Object Detection with Vision-Language Model Distillation [[Paper]](https://ieeexplore.ieee.org/document/10669066) ![](https://img.shields.io/badge/year-2024-red)
