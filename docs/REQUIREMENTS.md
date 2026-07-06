# What you need to build your own AI LLM

## 1) Compute options (choose one)
- **Local GPU** (best long-term)
  - typical: consumer GPU 8GB+ (more is better)
- **CPU-only** (possible for small models; slower)
- **Free/open hosted runtime** (temporary; cost may later appear)

## 2) Model strategy
- Start with an **open instruct/chat** model
- Prefer small-to-medium models you can run comfortably
- Use quantization if needed

## 3) Data
- High-quality documents you want the assistant to know
- For fine-tuning:
  - instruction/response pairs
  - consistent formatting

## 4) Stack (suggested)
- Language runtime: Python (common for LLM apps)
- Inference/runtime: llama.cpp / vLLM / transformers (depending on your hardware)
- RAG:
  - embeddings model
  - vector database (or local alternative)
- Evaluation:
  - simple benchmark scripts

## 5) Storage
- Documents + chunk index
- Vector DB files
- Logs and evaluation outputs

## 6) Engineering practices
- Version your prompts and pipelines
- Keep an evaluation set fixed
- Track model + embedding versions

## “Free-of-cost” reality check
- Free = often achievable for docs + open-source tooling.
- Compute availability matters (local hardware or free tiers).
- The most cost-efficient path is: **RAG + tools first**, then fine-tune only if required.

