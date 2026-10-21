<div align="center">

# Gonzalo Fuentes

[![ML Engineer](https://img.shields.io/badge/ML%20Engineer-CENIA-blue?style=flat-square&logo=google-scholar&logoColor=white)](https://cenia.cl)
[![MSc](https://img.shields.io/badge/MSc-UC%20Chile-6B21A8?style=flat-square&logo=academia&logoColor=white)](https://uc.cl)
[![Location](https://img.shields.io/badge/Santiago-Chile-red?style=flat-square&logo=google-maps&logoColor=white)](https://maps.google.com/?q=Santiago,Chile)

### ML Engineer at [CENIA](https://cenia.cl) · MSc at UC Chile

Co-creator of [LatamGPT](https://www.latamgpt.org/en) — the first family of LLMs trained for Latin America.
I work on LLMs end to end (pretraining, post-training and data) and research world models (Dreamer, JEPA).

</div>

---

## LLM Learning Route

**[LatamGPT Engineering Hub](https://gonzalofuentes1.github.io/llm-learning-route/)** — an open learning route for building LLMs, from fundamentals to SOTA 2026, born at LatamGPT and updated as the field moves.
13 sections from data and pretraining to post-training, evaluation, safety, serving, agents and interpretability, a 7-stage recommended path, and hands-on guides with code. Written in Spanish, with a focus on Spanish and Portuguese.

[![Roadmap](https://img.shields.io/badge/Roadmap-300%2B%20topics%20%C2%B7%20900%2B%20papers-0EA5E9?style=flat-square&logo=bookstack&logoColor=white)](https://gonzalofuentes1.github.io/llm-learning-route/latamgpt-roadmap.html)
[![Guides](https://img.shields.io/badge/Guides-40%2B%20hands--on-10B981?style=flat-square&logo=readthedocs&logoColor=white)](https://gonzalofuentes1.github.io/llm-learning-route/)
[![Stars](https://img.shields.io/github/stars/GonzaloFuentes1/llm-learning-route?style=flat-square&logo=github&label=stars)](https://github.com/GonzaloFuentes1/llm-learning-route)
[![Updated](https://img.shields.io/github/last-commit/GonzaloFuentes1/llm-learning-route?style=flat-square&label=updated)](https://github.com/GonzaloFuentes1/llm-learning-route/commits)

---

## Stack

**LLMs / Research**
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co)
[![vLLM](https://img.shields.io/badge/vLLM-30A2FF?style=flat-square)](https://github.com/vllm-project/vllm)
[![JAX](https://img.shields.io/badge/JAX-8B5CF6?style=flat-square&logo=google&logoColor=white)](https://jax.readthedocs.io)
[![Lightning](https://img.shields.io/badge/Lightning-792EE5?style=flat-square&logo=lightning&logoColor=white)](https://lightning.ai)
[![W&B](https://img.shields.io/badge/W%26B-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black)](https://wandb.ai)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)

**Infra / Backend**
[![Slurm](https://img.shields.io/badge/Slurm-0B7A75?style=flat-square)](https://slurm.schedmd.com)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://docker.com)
[![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)](https://aws.amazon.com)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)](https://nextjs.org)

---

## LatamGPT

- **Pretraining** — continued pretraining of Llama 3.1 70B and consolidation of tensor-parallel distributed checkpoints into Hugging Face format
- **Post-training** — SFT of OLMo-3 on Spanish and Latin American data mixtures, synthetic SFT and preference data (personas, Constitutional AI)
- **Data** — LLM-labelled quality classifiers and toxicity filtering for Spanish and Latin American pretraining corpora
- **Evaluation** — [Trueque Benchmark](https://huggingface.co/datasets/latam-gpt/Trueque-Benchmark-beta-0.1): 500 cultural questions across 20 Latin American countries

---

## Projects

**LLM training**
- **[parallelism-from-scratch](https://github.com/GonzaloFuentes1/parallelism-from-scratch)** — DDP, ZeRO-1/2, tensor and pipeline parallelism for a tiny Llama, with float64 parity tests and DCP resharding
- **[post-training-from-scratch](https://github.com/GonzaloFuentes1/post-training-from-scratch)** — SFT packing and masking, DPO/IPO/SimPO and GRPO/Dr.GRPO/DAPO, each checked by invariant tests
- **[llama3-70b-dcp-to-hf](https://github.com/GonzaloFuentes1/llama3-70b-dcp-to-hf)** — Converts sharded DCP checkpoints (TP=8) of a Llama 3 70B pretraining run to Hugging Face safetensors
**LLM data**
- **[limpia](https://github.com/GonzaloFuentes1/limpia)** — Spanish and Latin American pretraining data curation: quality heuristics, MinHash dedup, PII scrubbing, decontamination
- **[quality-filter](https://github.com/GonzaloFuentes1/quality-filter)** — Text quality classifier distilled from an LLM judge, with batch filtering for pretraining data
- **[constitutional-ai-data-pipeline](https://github.com/GonzaloFuentes1/constitutional-ai-data-pipeline)** — vLLM pipeline for Constitutional AI data: red-team, critique and revision into SFT and preference pairs
- **[magpie-persona-gen](https://github.com/GonzaloFuentes1/magpie-persona-gen)** — Persona-conditioned synthetic SFT conversations with filtering and MinHash dedup

**World models**
- **[dreamer4](https://github.com/GonzaloFuentes1/dreamer4)** — Unofficial Dreamer 4 re-implementation: transformer tokenizer, shortcut dynamics and imagination RL on DMControl
- **[dreamer-core](https://github.com/GonzaloFuentes1/dreamer-core)** — Tested building blocks of DreamerV3-style world models: RSSM, KL balancing, symlog two-hot heads, λ-returns
- **[dreamer_study](https://github.com/GonzaloFuentes1/dreamer_study)** — PyTorch implementations of Dreamer V1 to V3 for DMControl
- *In progress* — JEPA-style latent world models for planning and model-based RL (paper in preparation)

**Tools**
- **[light-anonymizer](https://github.com/GonzaloFuentes1/light-anonymizer)** — Offline desktop tool that redacts PII from PDFs and images, with leak re-check and audit report
- **[skill-agents](https://github.com/GonzaloFuentes1/skill-agents)** — Claude Code plugin that routes subagents by model and effort, with observability and a strict git flow
- **[auto-lab](https://github.com/GonzaloFuentes1/auto-lab)** — Hypothesis-driven research workflow: append-only lab log, significance checks, paper pipeline

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-GonzaloFuentes1-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/GonzaloFuentes1)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-latam--gpt-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/latam-gpt)
[![Web](https://img.shields.io/badge/Web-latamgpt.org-0EA5E9?style=flat-square&logo=googlechrome&logoColor=white)](https://www.latamgpt.org/en)

</div>
