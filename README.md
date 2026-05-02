# Awesome-Pathology-VLMs

**Awesome-Pathology-VLMs** aims to curates research resources in the field of **Pathology Vision-Language Models (Pathology VLMs)**, covering VLM / Multimodal LLM works, datasets, and benchmarks.

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


| **Paper Title** | **Granularity** | **Venue** | **Resources** | **Summary** |
| --------------- | --------------- | --------- | ------------- | ----------- |


### 1.2 Generative / Instruction-Tuned

Pathology MLLMs that connect pathology visual encoders to language models and are trained or instruction-tuned for generation, dialogue, VQA, or report-style outputs.


| **Paper Title** | **Granularity** | **Venue** | **Resources** | **Summary** |
| --------------- | --------------- | --------- | ------------- | ----------- |


### 1.3 Reasoning / RL-Enhanced

Pathology VLMs or MLLMs that add explicit reasoning, chain-of-thought-style supervision, RLVR, preference optimization, or other post-training methods.


| **Paper Title** | **Granularity** | **Venue** | **Resources** | **Summary** |
| --------------- | --------------- | --------- | ------------- | ----------- |


### 1.4 Agent-Based Systems

Pathology systems where an LLM or MLLM orchestrates perception, slide navigation, retrieval, tool use, multi-scale inspection, or external domain-specific modules.


| **Paper Title** | **Granularity** | **Venue** | **Resources** | **Summary** |
| --------------- | --------------- | --------- | ------------- | ----------- |


### 1.5 VLM-Augmented MIL

Slide-level MIL methods that use frozen VLMs, text embeddings, prompts, or language-derived priors to improve WSI aggregation. 


| **Paper Title** | **Granularity** | **Venue** | **Resources** | **Summary** |
| --------------- | --------------- | --------- | ------------- | ----------- |


## 2. Datasets


| **Data Name** | **Paper** | **Link** | **Quantity** |
| ------------- | --------- | -------- | ------------ |


## 3. Benchmarks


| **Evaluation Framework** | **Code** | **Supported Benchmarks** |
| ------------------------ | -------- | ------------------------ |


