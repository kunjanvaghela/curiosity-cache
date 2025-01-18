
Vector: a sequence of numbers, called dimensions, used to capture the important features of the data.

Vector Embeddings: generally represent the semantic content of data, not the underlying words or pixels.



Embedding Distance:
1. Dot Product
	- Takes magnitude and angle both into consideration.
2. Cosine Distance
	- Takes only angle into consideration
	- Might be useful when orientation is more important than magnitude. Magnitude might represent the strength/frequency as well based on the context.



Some Vector Search algorithms:
1. KNN
2. ANN algorithms like:
	1. HNSW
	2. FAISS
	3. Annoy



Vector Databases Examples:
1. Faiss
2. Pinecone
3. Oracle AI Vector Search
4. Chroma
5. Weaviate



Important Features of Vector Databases:
1. Accuracy - captures nuance relationships better than traditional dbs.
2. Latency - Optimized for retrieval of high dimensional data.



Role of Vector Databasses with LLMs
1. Cheaper than fine-tuning LLMs, which can be expensive to update.
2. Real-time updated knowledge base.
3. Cache previous LLM prompts/responses to improve performance and reduce costs.