# Gonzalo Fuentes

ML engineer working on **LLM training at scale** and **self-supervised learning (JEPA)**.
Tech Lead of [LatamGPT](https://www.latamgpt.org/en) at [CENIA](https://cenia.cl), MSc researcher at UC Chile. Santiago, Chile.

[![Web](https://img.shields.io/badge/Web-gonzalofuentes1.github.io-0EA5E9?style=flat-square&logo=googlechrome&logoColor=white)](https://gonzalofuentes1.github.io/en/)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-GonzaloFuentes1-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/GonzaloFuentes1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-gonzalo--fuentes--olivares-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gonzalo-fuentes-olivares-850bb12a7/)

---

## What I work on

**LatamGPT 70B** is an open foundation model for Latin America, continually pre-trained and post-trained from Llama 3.1 70B.
Since April 2026 I lead its technical work (4 teams, 10 people): data, pretraining, post-training and evaluation.

- **Pretraining**: 70B continued pretraining on 128 H200 GPUs (TP=8 × hybrid-sharded FSDP=16, FP8, 8k context, ~141.6k tokens/s), and conversion of tensor-parallel distributed checkpoints to Hugging Face format
- **Data**: the 296.5B-token LatamGPT-Corpus from 20 countries, with quality classifiers distilled from an LLM judge, MinHash dedup, PII scrubbing and benchmark decontamination
- **Post-training**: SFT, safety tuning and synthetic data (personas, Constitutional AI) on Llama and OLMo-3
- **Evaluation**: lead of [Trueque](https://huggingface.co/datasets/latam-gpt/Trueque-Benchmark-beta-0.1), a human-reviewed benchmark of Latin American knowledge across 20 countries

**Research**: JEPA-style latent world models and the SIGReg regularizer from LeJEPA, for planning, model-based RL and language models.

---

## Selected open source

**LLM training, from scratch and tested**
- **[parallelism-from-scratch](https://github.com/GonzaloFuentes1/parallelism-from-scratch)**: DDP, ZeRO-1/2, tensor and pipeline parallelism for a tiny Llama, each matched against a float64 single-process reference (atol 1e-12), plus DCP resharding
- **[post-training-from-scratch](https://github.com/GonzaloFuentes1/post-training-from-scratch)**: SFT packing and masking, DPO/IPO/SimPO and GRPO/Dr.GRPO/DAPO, each objective checked by invariant tests
- **[llama3-70b-dcp-to-hf](https://github.com/GonzaloFuentes1/llama3-70b-dcp-to-hf)**: converts sharded DCP checkpoints (TP=8) of a Llama 3 70B pretraining run to Hugging Face safetensors

**Pretraining and post-training data**
- **[limpia](https://github.com/GonzaloFuentes1/limpia)**: Spanish and Portuguese pretraining data curation with Gopher/FineWeb quality rules, MinHash dedup, PII scrubbing and decontamination
- **[quality-filter](https://github.com/GonzaloFuentes1/quality-filter)**: multilabel quality classifier distilled from an LLM judge, with batch filtering for pretraining corpora
- **[constitutional-ai-data-pipeline](https://github.com/GonzaloFuentes1/constitutional-ai-data-pipeline)**: vLLM pipeline for Constitutional AI data (red-team, critique, revision) into SFT and preference pairs
- **[magpie-persona-gen](https://github.com/GonzaloFuentes1/magpie-persona-gen)**: persona-conditioned synthetic SFT conversations with filtering and dedup

**Self-supervised learning and world models**
- **[dreamer4](https://github.com/GonzaloFuentes1/dreamer4)**: unofficial Dreamer 4 re-implementation with a transformer tokenizer, shortcut dynamics and imagination RL on DMControl
- **[dreamer-core](https://github.com/GonzaloFuentes1/dreamer-core)**: tested building blocks of DreamerV3-style world models (RSSM, KL balancing, symlog two-hot heads, λ-returns)

**Teaching**
- **[llm-learning-route](https://github.com/GonzaloFuentes1/llm-learning-route)**: an open route for building LLMs, in Spanish, with 300+ topics, 900+ papers and 40+ hands-on guides from data to serving

---

## Publications

- **LatamGPT 70B Technical Report**. LatamGPT Team, CENIA, 2026.
- **LatamGPT-Corpus, a text corpus of 296 billion tokens for language model pre-training**. Submitted to Springer Nature, 2026.
- **Unlearnability of Symmetry-based Visual Relations by Deep Neural Networks**. CCN 2026, extended abstract.
- **WayraPPL: Accelerating Curriculum Learning with Knowledge-Distilled Perplexity Models**. NeurIPS 2025 LatinX in AI workshop, LatamGPT Team.

---

<sub>PyTorch · JAX · TorchTitan · Megatron-Core / NeMo · vLLM · Hugging Face · Lightning · Hydra · W&B · Slurm · AWS · Docker</sub>
