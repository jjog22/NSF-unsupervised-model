# NSF Research Awards Abstracts
This dataset comprises several paper abstracts, one per file, that were furnished by the NSF
(National Science Foundation). 
The task is developing an unsupervised model which classifies abstracts into a topic (discover
them). The goal is to group abstracts based on their semantic similarity.

## SOLUTION - How to Cluster Documents
We can think of the process of clustering documents in three steps:

1. Cleaning and tokenizing data: this usually involves lowercasing text, removing non-alphanumeric characters, or stemming words.
2. Generating vector representations of the documents: this concerns the mapping of documents from words into numerical vectors—some common ways of doing this include using bag-of-words models or word embeddings.
3. Applying a clustering algorithm on the document vectors: this requires selecting and applying a clustering algorithm to find the best possible groups using the document vectors. Some frequently used algorithms include K-means or Hierarchical Clustering.

## Notes about this work
- In the first version of this model we are going to check the steps of NLP
using Doc2vec and functions from gensim library
- I will use all the words in the documents read from XML files and in this version of experimentation
- I don´t remove stopwords or another kind of cleaning like reducing short words or dimensionality
because we need to make all the steps to implement clustering algorithm and review results at first check 
the results, to make the formation of clusters and similarity with the original data.
- In later versions we can include another techniques and optimize the volume of words with the goal
of getting better results and clustering of the documents in categories (not existent now) and this
we call it like pseudo-categories (with the more representative words in a cluster)
- Of course we need to include in the definition of the best number of clusters known techniques like ELBOW 
### I would make functions and pipelines of this code but my time wasn't enough to spend in better coding and testing another techniques for comparison
