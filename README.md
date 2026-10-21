# Gonzalo Fuentes

ML Engineer at [CENIA](https://cenia.cl) (Santiago, Chile) and MSc student at Pontificia Universidad Católica de Chile.
I work on large language models end to end (pretraining, post-training and the data behind them) and research world models for control.

**Co-creator of [LatamGPT](https://www.latamgpt.org/en)**, an open family of LLMs trained for Latin America ([Hugging Face](https://huggingface.co/latam-gpt)). My work there includes:

- **Pretraining**: continued pretraining of Llama 3.1 70B, and tooling to consolidate tensor-parallel distributed checkpoints into Hugging Face format.
- **Post-training**: supervised fine-tuning of OLMo-3 models on Spanish and Latin American data mixtures, and synthetic SFT and preference data (persona-conditioned dialogues, Constitutional AI critique and revision).
- **Data**: LLM-labelled quality classifiers and toxicity filtering for Spanish and Latin American pretraining corpora.
- **Evaluation**: [Trueque](https://huggingface.co/datasets/latam-gpt/Trueque-Benchmark-beta-0.1), a cultural knowledge benchmark with 500 questions across 20 Latin American countries.

## Open source

### Large language models

| Repository | Description |
|---|---|
| [parallelism-from-scratch](https://github.com/GonzaloFuentes1/parallelism-from-scratch) | DDP, ZeRO-1/2, tensor and pipeline parallelism for a tiny Llama, with float64 parity tests on CPU and DCP resharding |
| [post-training-from-scratch](https://github.com/GonzaloFuentes1/post-training-from-scratch) | Tested post-training objectives: SFT packing and masking, DPO/IPO/SimPO, GRPO/Dr.GRPO/DAPO |
| [limpia](https://github.com/GonzaloFuentes1/limpia) | Spanish and Latin American pretraining data curation: quality heuristics, MinHash dedup, PII scrubbing, decontamination |
| [llama3-70b-dcp-to-hf](https://github.com/GonzaloFuentes1/llama3-70b-dcp-to-hf) | Converts sharded PyTorch DCP checkpoints (TP=8) of a Llama 3 70B pretraining run to Hugging Face safetensors |
| [quality-filter](https://github.com/GonzaloFuentes1/quality-filter) | Multilabel text quality classifier distilled from an LLM judge, with batch filtering for pretraining data |
| [constitutional-ai-data-pipeline](https://github.com/GonzaloFuentes1/constitutional-ai-data-pipeline) | vLLM pipeline for Constitutional AI data: red-team, critique and revision, exported as SFT and preference pairs |
| [magpie-persona-gen](https://github.com/GonzaloFuentes1/magpie-persona-gen) | Persona-conditioned synthetic SFT conversations with filtering and MinHash dedup |
| [llm-learning-route](https://gonzalofuentes1.github.io/llm-learning-route/) | Roadmap and hands-on guides (in Spanish) for building LLMs, from data to serving |

### World models

| Repository | Description |
|---|---|
| [dreamer4](https://github.com/GonzaloFuentes1/dreamer4) | Unofficial re-implementation of Dreamer 4: transformer tokenizer, shortcut dynamics and imagination RL on DMControl |
| [dreamer-core](https://github.com/GonzaloFuentes1/dreamer-core) | Tested building blocks of DreamerV3-style world models: RSSM, KL balancing, symlog two-hot heads, λ-returns |
| [dreamer_study](https://github.com/GonzaloFuentes1/dreamer_study) | PyTorch implementations of Dreamer V1 to V3 for DMControl |

**In progress:** JEPA-style latent world models for planning and model-based RL. Paper in preparation; code will be released with the paper.

### Engineering

| Repository | Description |
|---|---|
| [light-anonymizer](https://github.com/GonzaloFuentes1/light-anonymizer) | Offline desktop tool that redacts PII from PDFs and images, with leak re-check and audit report |
| [skill-agents](https://github.com/GonzaloFuentes1/skill-agents) | Claude Code plugin that routes subagents by model and effort, with observability and a strict git flow |
| [auto-lab](https://github.com/GonzaloFuentes1/auto-lab) | Hypothesis-driven research workflow: append-only lab log, significance checks, paper pipeline |

## Stack

PyTorch · JAX · Hugging Face Transformers, TRL and Datasets · vLLM · OLMo-core · FSDP and torch.distributed.checkpoint · Lightning · Hydra · Weights & Biases · Slurm · Docker

[LatamGPT](https://www.latamgpt.org/en) · [Hugging Face](https://huggingface.co/latam-gpt) · [CENIA](https://cenia.cl)
