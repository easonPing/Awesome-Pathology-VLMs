# Awesome-Pathology-VLMs

**Awesome-Pathology-VLMs** aims to curate research resources in the field of **Pathology Vision-Language Models (Pathology VLMs)**, covering VLM / Multimodal LLM works, datasets, and benchmarks.

Table of Contents:

- [1. Pathology VLMs](#1-pathology-vlms)
  - [1.1 Contrastive / Dual-Encoder](#11-contrastive--dual-encoder)
  - [1.2 Generative / Instruction-Tuned](#12-generative--instruction-tuned)
  - [1.3 Reasoning / RL-Enhanced](#13-reasoning--rl-enhanced)
  - [1.4 Agent-Based Systems](#14-agent-based-systems)
  - [1.5 VLM-Augmented MIL (utilization)](#15-vlm-augmented-mil-utilization)
- [2. Datasets](#2-datasets)
- [3. Benchmarks](#3-benchmarks)

## 1. Pathology VLMs

Use the **Granularity** column to mark where each system operates:

- `G1` = Patch / Tile
- `G2` = Region of interest (ROI)
- `G3` = Whole-slide image (WSI)

For systems spanning multiple levels, use combined labels such as `G1/G3` or `G2/G3`.

### 1.1 Contrastive / Dual-Encoder

Pathology VLMs trained with image-text contrastive alignment or related dual-encoder objectives.


| Paper Title                                                                                   | Granularity | Venue                | Resources                                                                                                                                                      | Summary |
| --------------------------------------------------------------------------------------------- | ----------- | -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| A Visual-Language Foundation Model for Pathology Image Analysis Using Medical Twitter         | G1          | Nature Medicine 2023 | [paper](https://doi.org/10.1038/s41591-023-02504-3) [code](https://github.com/PathologyFoundation/plip) [project](https://huggingface.co/spaces/vinid/webplip) |         |
| A Visual-Language Foundation Model for Computational Pathology                                | G1/G2/G3    | Nature Medicine 2024 | [paper](https://doi.org/10.1038/s41591-024-02856-4) [code](https://github.com/mahmoodlab/CONCH)                                                                |         |
| Multi-Resolution Pathology-Language Pre-training Model with Text-Guided Visual Representation | G1/G2/G3    | CVPR 2025            | [paper](https://arxiv.org/abs/2504.18856) [code](https://github.com/BasitAlawode/MR-PLIP)                                                                      |         |
| A Vision-Language Foundation Model for Precision Oncology                                     | G1/G2/G3    | Nature 2025          | [paper](https://doi.org/10.1038/s41586-024-08378-w) [code](https://github.com/lilab-stanford/MUSK)                                                             |         |
| Multimodal Whole Slide Foundation Model for Pathology                                         | G1/G2/G3    | Nature Medicine 2025 | [paper](https://doi.org/10.1038/s41591-025-03982-3) [code](https://github.com/mahmoodlab/TITAN)                                                                |         |
| PathFLIP: Fine-grained Language-Image Pretraining for Versatile Computational Pathology       | G1/G2/G3    | arXiv 2025           | [paper](https://arxiv.org/abs/2512.17621)                                                                                                                      |         |
| PRISM: A Multi-Modal Generative Foundation Model for Slide-Level Histopathology               | G2/G3       | arXiv 2024           | [paper](https://arxiv.org/abs/2405.10254)                                                                                                                      |         |
| PRISM2: Unlocking Multi-Modal General Pathology AI with Clinical Dialogue                     | G2/G3       | arXiv 2025           | [paper](https://arxiv.org/abs/2506.13063)                                                                                                                      |         |
| HiPath: Hierarchical Vision-Language Alignment for Structured Pathology Report Prediction     | G2/G3       | arXiv 2026           | [paper](https://arxiv.org/abs/2603.19957)                                                                                                                      |         |


### 1.2 Generative / Instruction-Tuned

Pathology MLLMs that connect pathology visual encoders to language models and are trained or instruction-tuned for generation, dialogue, VQA, or report-style outputs.


| Paper Title                                                                                                             | Granularity | Venue                               | Resources                                                                                                                                                | Summary |
| ----------------------------------------------------------------------------------------------------------------------- | ----------- | ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| LLaVA-Med: Training a Large Language-and-Vision Assistant for Biomedicine in One Day                                    | G1          | NeurIPS D&B 2023                    | [paper](https://arxiv.org/abs/2306.00890) [code](https://github.com/microsoft/LLaVA-Med)                                                                 |         |
| Quilt-LLaVA: Visual Instruction Tuning by Extracting Localized Narratives from Open-Source Histopathology Videos        | G1          | CVPR 2024                           | [paper](https://arxiv.org/abs/2312.04746) [code](https://github.com/aldraus/quilt-llava) [project](https://quilt-llava.github.io/)                       |         |
| PathAsst: A Generative Foundation AI Assistant Towards Artificial General Intelligence of Pathology                     | G1          | AAAI 2024                           | [paper](https://arxiv.org/abs/2305.15072) [code](https://github.com/superjamessyx/Generative-Foundation-AI-Assistant-for-Pathology)                      |         |
| A Multimodal Generative AI Copilot for Human Pathology                                                                  | G1/G2       | Nature 2024                         | [paper](https://doi.org/10.1038/s41586-024-07618-3) [code](https://github.com/fedshyvana/pathology_mllm_training)                                        |         |
| PA-LLaVA: A Large Language-Vision Assistant for Human Pathology Image Understanding                                     | G1          | IEEE BIBM 2024                      | [paper](https://doi.org/10.1109/BIBM62325.2024.10821785) [code](https://github.com/ddw2AIGROUP2CQUPT/PA-LLaVA)                                           |         |
| PathInsight: Instruction Tuning of Multimodal Datasets and Models for Intelligence Assisted Diagnosis in Histopathology | G1          | arXiv 2024                          | [paper](https://arxiv.org/abs/2408.07037)                                                                                                                |         |
| Dr-LLaVA: Visual Instruction Tuning with Symbolic Clinical Grounding                                                    | G1          | NeurIPS MAR Workshop 2024           | [paper](https://arxiv.org/abs/2405.19567)                                                                                                                |         |
| PathologyVLM: A Large Vision-Language Model for Pathology Image Understanding                                           | G1          | Artificial Intelligence Review 2025 | [paper](https://doi.org/10.1007/s10462-025-11190-1) [code](https://github.com/ddw2AIGROUP2CQUPT/PA-LLaVA)                                                |         |
| SlideChat: A Large Vision-Language Assistant for Whole-Slide Pathology Image Understanding                              | G3          | CVPR 2025                           | [paper](https://arxiv.org/abs/2410.11761) [code](https://github.com/uni-medical/SlideChat) [project](https://uni-medical.github.io/SlideChat.github.io/) |         |
| CPath-Omni: A Unified Multimodal Foundation Model for Patch and Whole Slide Image Analysis in Computational Pathology   | G1/G2/G3    | CVPR 2025                           | [paper](https://arxiv.org/abs/2412.12077) [code](https://github.com/PathFoundation/CPath-Omni)                                                           |         |
| WSI-LLaVA: A Multimodal Large Language Model for Whole Slide Image                                                      | G2/G3       | ICCV 2025                           | [paper](https://arxiv.org/abs/2412.02141) [project](https://wsi-llava.github.io/)                                                                        |         |


### 1.3 Reasoning / RL-Enhanced

Pathology VLMs or MLLMs that add explicit reasoning, chain-of-thought-style supervision, RLVR, preference optimization, or other post-training methods.


| Paper Title                                                                                                                    | Granularity | Venue      | Resources                                                                                        | Summary |
| ------------------------------------------------------------------------------------------------------------------------------ | ----------- | ---------- | ------------------------------------------------------------------------------------------------ | ------- |
| EAGLE: Expert-Guided Self-Enhancement for Preference Alignment in Pathology Large Vision-Language Model                        | G1          | ACL 2025   | [paper](https://doi.org/10.18653/v1/2025.acl-long.711) [code](https://github.com/meidandz/EAGLE) |         |
| Patho-R1: A Multimodal Reinforcement Learning-Based Pathology Expert Reasoner                                                  | G1          | AAAI 2026  | [paper](https://arxiv.org/abs/2505.11404) [code](https://github.com/Wenchuan-Zhang/Patho-R1)     |         |
| PathVLM-R1: A Reinforcement Learning-Driven Reasoning Model for Pathology Visual-Language Tasks                                | G1          | arXiv 2025 | [paper](https://arxiv.org/abs/2504.09258)                                                        |         |
| SmartPath-R1: A MoE-Based Multimodal Reasoner Unifying ROI and WSI Pathology Tasks                                             | G1/G2/G3    | arXiv 2025 | [paper](https://arxiv.org/abs/2507.17303)                                                        |         |
| PathReasoner-R1: Instilling Structured Reasoning into Pathology Vision-Language Model via Knowledge-Guided Policy Optimization | G1/G3       | arXiv 2026 | [paper](https://arxiv.org/abs/2601.21617)                                                        |         |


### 1.4 Agent-Based Systems

Pathology systems where an LLM or MLLM orchestrates perception, slide navigation, retrieval, tool use, multi-scale inspection, or external domain-specific modules.


| Paper Title                                                                                                                                     | Granularity | Venue        | Resources                                 | Summary |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ------------ | ----------------------------------------- | ------- |
| CPathAgent: An Agent-based Foundation Model for Interpretable High-Resolution Pathology Image Analysis Mimicking Pathologists' Diagnostic Logic | G2/G3       | NeurIPS 2025 | [paper](https://arxiv.org/abs/2505.20510) |         |


### 1.5 VLM-Augmented MIL

Slide-level MIL methods that use frozen VLMs, text embeddings, prompts, or language-derived priors to improve WSI aggregation.


| Paper Title                                                                                                                             | Granularity | Venue         | Resources                                                                                             | Summary |
| --------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ------------- | ----------------------------------------------------------------------------------------------------- | ------- |
| ViLa-MIL: Dual-scale Vision-Language Multiple Instance Learning for Whole Slide Image Classification                                    | G3          | CVPR 2024     | [paper](https://doi.org/10.1109/CVPR52733.2024.01069) [code](https://github.com/Jiangbo-Shi/ViLa-MIL) |         |
| VLEER: Vision and Language Embeddings for Explainable Whole Slide Image Representation                                                  | G3          | MICCAI-W 2025 | [paper](https://arxiv.org/abs/2502.20850)                                                             |         |
| Slide-Level Prompt Learning with Vision Language Models for Few-Shot Multiple Instance Learning in Histopathology                       | G3          | ISBI 2025     | [paper](https://arxiv.org/abs/2503.17238) [code](https://github.com/LTS5/SLIP)                        |         |
| GMAT: Grounded Multi-Agent Clinical Description Generation for Text Encoder in Vision-Language MIL for Whole Slide Image Classification | G3          | MICCAI-W 2025 | [paper](https://arxiv.org/abs/2508.01293)                                                             |         |
| Act Like a Pathologist: Tissue-Aware Whole Slide Image Reasoning                                                                        | G2/G3       | CVPR 2026     | [paper](https://arxiv.org/abs/2603.00667) [code](https://github.com/winston52/HistoSelect)            |         |


## 2. Datasets


| Data Name | Paper | Link | Quantity |
| --------- | ----- | ---- | -------- |
|           |       |      |          |


## 3. Benchmarks


| Evaluation Framework | Code | Supported Benchmarks |
| -------------------- | ---- | -------------------- |
|                      |      |                      |


