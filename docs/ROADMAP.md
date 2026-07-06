# Roadmap — Indos AI LLM

## Milestone 0: Planning (1–2 days)
- finalize scope: “assistant + RAG” first
- pick target model size
- define evaluation dataset format

## Milestone 1: Chat MVP (3–7 days)
- basic chat loop
- system prompt + conversation formatting
- logging

## Milestone 2: RAG MVP (5–14 days)
- ingest documents
- chunk + embeddings
- retrieval + context injection
- response evaluation v1

## Milestone 3: Tools & Workflows (7–21 days)
- tool calling (summarize/extract/search in your dataset)
- workflow prompts

## Milestone 4: Fine-tuning (optional, 1–4 weeks)
- only if you have enough data
- start with small model
- compare before/after using evaluation set

## Milestone 5: Polish + Deployment (ongoing)
- caching
- UI improvements
- safety guardrails
- documentation and release tags

## Notes
- The fastest “wow” usually comes from RAG + good document quality.
- Fine-tuning is last, not first.

