- Built on Transformer Architecture:
  - Encoders -> Embedding
  - Decoders -> Text Generation
- Will be based on “Attention is all you need” paper
- Models of each type come in a variety of sizes (# of parameters).

![[LLM Model Ontology.png]]
### Encoders:

1. Converts a sequence of words to an embedding (vector representation).
2. Usage:
   - Vector representations can be used to consume in other models for tasks such as Classification/Regression.
   - Vector Search/Semantic Search
3. Examples: MiniLM, Embed-light, BERT, RoBERTA, DistillBERT, SBERT, etc.

### Decoders:

1. Take a sequence of words and output the next word.
2. Only generates a single token at a time, hence done repeatedly.
3. Examples: GPT-4, Llama, BLOOM, Falcon

### Encoders-Decoders:

1. Encodes a sequence of words and uses the encoding to output the next word.
2. Examples: T5, UL2, BART, etc.