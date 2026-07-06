# Project structure map

Recommended repository layout for an LLM assistant.

```text
privproject/
  README.md
  LICENSE
  docs/
    index.md
    HOW_TO_BUILD.md
    REQUIREMENTS.md
    ARCHITECTURE.md
    PROJECT_STRUCTURE.md
    ROADMAP.md
    TIMELINE_ESTIMATE.md

  apps/
    web/                 # optional front-end
    cli/                 # optional CLI

  services/
    api/                 # orchestration backend

  llm/
    inference/           # model runtime wrappers
    prompts/             # prompt templates

  rag/
    ingestion/           # doc loaders + chunking
    embeddings/          # embedding pipeline
    vector_store/       # DB integration

  tools/
    function_registry/  # list of tools

  eval/
    datasets/
    benchmarks/

  configs/
    models.yml
    rag.yml

  scripts/
    bootstrap.sh
    seed_docs.sh
```

## Why this structure
- Keeps inference, RAG, tools, and evaluation separated
- Lets you iterate: start with chat → add RAG → add tools

