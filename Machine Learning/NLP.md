
## Glossary:
1. Stemming: is a process that stems or removes last few characters from a word, often leading to incorrect meanings and spelling. Stemming is used in case of large dataset where performance is an issue.
2. Lemmatization: considers the context and converts the word to its meaningful base form, which is called Lemma. Lemmatization is computationally expensive since it involves look-up tables and what not.
3. 


# Text Classification

1) Preprocessed data and converted it into numerical representations
2) Apply clustering algorithms to the resulting embeddings to group documents into clusters.
3) Compare performance of the different embedding approaches.


#### Data Preprocessing
- Remove:
	- stopwords
	- white characters
	- get tokens using 'nltk.word_tokenize({text})'
	- lowercase all the characters and then strip

#### Embedding Techniques:
1. TF-IDF Vectorization (Term frequency inverse document frequency)
	1. calculates the importance of words in a sentence by taking into account how often they appear in the sentence and how rare they are in the entire corpus of sentences. 
	2. ``sklearn.feature_extraction.text import TfidfVectorizer``
2. Sentence Transformer
	1. are deep learning models that can encode natural language sentences into high-dimensional vector representations.
	2. They are trained using a pre-training and fine-tuning approach and have achieved state-of-the-art performance on several natural language processing tasks.
3. GloVe
	1. is a word embedding technique that represents words as dense vectors in a high-dimensional space.
	2. It captures both local and global context, making it useful for various tasks.
	3. To cluster sentences using GloVe, one approach is to concatenate the word vectors in a sentence, form a matrix, and then apply a clustering algorithm such as k-means. The resulting clusters can reveal common themes or patterns in the data.
	4. `` torchtext.vocab.GloVe(name='840B', dim=300, **kwargs)
4. BERT — CLS token for sentence context
	1. pre-trained deep learning model that can be fine-tuned for various natural language processing tasks.
	2. One of the main innovations of BERT is its ability to represent both the left and right context of a word, allowing it to better capture the meaning of a sentence.



#### Choosing the Right Model for Text Classification
1. **k-NN** is easy to implement and understand but can be slow with large datasets and high-dimensional spaces.
2. Logistic Regression is a good starting point for its simplicity and interpretability.
3. SVMs are effective for high-dimensional spaces, but may be slower for large datasets.
4. Random Forest and Gradient Boosting methods are robust and can handle various types of data well.
5. Neural Networks can capture complex patterns, especially useful for large datasets with intricate structures.


