# search-engine
AI Search Engine with NLP embeddings

| Project         | Elasticsearch-based | Purpose                  | Embedding Support | License    |
| --------------- | ------------------- | ------------------------ | ----------------- | ---------- |
| **Haystack**    | Yes                 | RAG, semantic search     | ✔️ Strong         | Apache-2.0 |
| **OpenSearch**  | Fork of ES          | Vector DB, search engine | ✔️ Native         | Apache-2.0 |
| **Jina**        | Optional ES backend | Neural search            | ✔️ Strong         | Apache-2.0 |
| **BEIR**        | Yes                 | Benchmark & pipelines    | ✔️ Strong         | MIT        |
| **SearchUI**    | Yes                 | UI framework             | Works with ES     | Apache-2.0 |
| **LAION tools** | Yes (some)          | Open embedding search    | ✔️                | Mixed      |

# retrieval
The ingestion pipeline (document extraction, clean/normalize, chunking)

The embedding extraction (which embedding model, batching)

The vector store integration (ChromaDB or Pinecone: how to create collections/indexes, upsert embeddings, store metadata)

The sparse store integration (if using Elasticsearch: index mapping, Language analyzer, docs ingestion)

The retrieval logic (how to query vector store + sparse store, merge scores)

The generation step (LLM prompt, context assembly, citation)

The metadata handling (source ids, chunk ids, page numbers etc)