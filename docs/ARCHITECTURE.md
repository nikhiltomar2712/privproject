# Architecture overview — Indos AI LLM

## High-level components
1. **UI / Client**
   - web, CLI, or desktop

2. **API / Backend**
   - orchestrates prompts, retrieval, tool calls

3. **LLM Inference Layer**
   - runs the selected open model
   - supports chat format and streaming

4. **RAG Layer (optional but recommended)**
   - document ingestion
   - chunking + embeddings
   - vector search
   - prompt assembly with retrieved context

5. **Tools / Plugins Layer (optional)**
   - functions the model can invoke

6. **Memory (optional)**
   - user preferences / conversation summary

7. **Evaluation & Logs**
   - store interactions and test outcomes

## Request flow (RAG)
1. User question arrives
2. Retrieve relevant chunks from vector DB
3. Compose final prompt (system + context + user)
4. Send to LLM
5. Return answer with citations (if desired)

## Design goals
- Modular: swap models + vector DB
- Reproducible: keep config with versions
- Measurable: evaluations for every iteration

