
- Search by meaning (intent and content)

Ways:
- Dense Retrieval: Uses text embeddings
- Re-ranking: Assigns a relevance score.


## Dense Retrieval

1. Find embedding vector corresponding to the query.
2. Find embedding vectors corresponding to each of the responses.
3. Retrieves the vectors closest to the query vector.


## Reranking

- Assigns a relevance score to (query, response) pairs from the initial search results.
- High relevance score pairs are more likely to be correct.
- Implemented through trained LLM.