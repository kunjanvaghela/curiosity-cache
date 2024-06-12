
- Fully managed service
- Choice of Models
- Flexible Fine-tuning
- Dedicated AI Clusters


## Pretrained Models:
#### Generation
- command
- command-light
- llama 2-70b-chat

#### Summarization
- command

#### Embedding
- embed-english-v3.0embed-multilingual
- embed-english-light-v3.0embed-multilingual
- embed-english-light-v2.0


## Dedicated AI Clusters




## Generation models
#### Parameters for Generation models
1. Temperature: Hyperparameter that controls the randomness of the LLM output.
2. Top p: To pick the next token from the top 'k' tokens in its list, sorted by probability.
3. Top k: Picks from the top tokens based on the sum of their probabilities, excludes tokens with lesser probability than mentioned after summing the top.
4. Stop Sequences: Models stop generating text after the given string is encountered.
5. Frequency Penalty: Penalizes tokens that have already appeared in the preceding text (including prompt), and scales based on frequency.
6. Presence Penalty: applied the penalty regardless of frequency.
7. Show Likelihoods: A new token is given a likelihood nr between 0 and -15. Higher the number, more likely to follow the current token.

#### Generation Models
- Tokens:
	- How an entity is represented. One word can be one token, or multi


## Summarization Models
#### Parameters for Summarization models
1. Temperature: Hyperparameter that controls the randomness of the LLM output.
2. Length: Length of the generated Summary: Short/Medium/Long
3. Format: Free-form/Bullets
4. Extractiveness: How much to reuse the input in the summary. High extractiveness means reuses sentences verbatim; lower means more paraphrasing.



## Embedding Models
#### Embedding Models
- Embedding:
	- numerical representation of the piece of text converted to number format in vector format.
- Word Embeddings:
	- Captures properties of the word
- Semantic Similarity:
	- Used to compute numerical similarity, which means that semantically similar.
	- Methods:
		- Dot similarity
		- Cosine similarity
- Sentence Embeddings:
	- A sentence embedding assosciates every sentence with a vector of numbers.

#### Parameters for Embedding models
?
