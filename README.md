# Fake-News-Awareness-NLP
## Dataset - https://www.kaggle.com/c/fake-news/data 

Using this NLP model and Dataset we try to identify Misinformation in articles

MultinomialNB, CountVectorizer, PorterStemmer, and nltk are all tools that can be used in natural language processing (NLP) tasks, including identifying unreliable news articles. Here is how each of these tools are used:

- **MultinomialNB**: Multinomial Naive Bayes (MNB) is a machine learning algorithm that is commonly used in text classification tasks. It is particularly well-suited for NLP tasks, as it can handle sparse feature vectors (i.e., text data with many features but relatively few non-zero values) efficiently. In the context of identifying unreliable news articles, MNB can be trained on a dataset of reliable and unreliable news articles to learn patterns and characteristics that are indicative of each type of article. Once trained, the model can be used to predict whether a new article is reliable or unreliable based on its features.

- **CountVectorizer**: CountVectorizer is a tool in the scikit-learn Python library that can be used to convert text data into numerical feature vectors. It works by tokenizing the text (i.e., breaking it up into individual words or n-grams), counting the occurrence of each token in each document, and then transforming the count data into a sparse matrix of features. In the context of identifying unreliable news articles, CountVectorizer can be used to preprocess the text data by tokenizing the articles and generating a bag of words representation of each article. This bag of words representation can then be fed into a machine learning model, such as MNB.

- **PorterStemmer**: PorterStemmer is a tool in the nltk Python library that can be used to reduce words to their stems (i.e., the base form of the word). This can be useful in NLP tasks, as it can reduce the dimensionality of the feature space and help group similar words together. In the context of identifying unreliable news articles, PorterStemmer can be used to preprocess the text data by reducing each word to its stem before tokenization and counting.

- **nltk**: The Natural Language Toolkit (nltk) is a Python library that provides a wide range of tools for NLP tasks, including tokenization, stemming, and part-of-speech tagging. In the context of identifying unreliable news articles, nltk can be used to preprocess the text data by tokenizing the articles into individual words, removing stop words (i.e., common words like "the" and "and" that are unlikely to be informative), and performing other text processing tasks.

In summary, MultinomialNB, CountVectorizer, PorterStemmer, and nltk are all powerful tools that can be used in combination to build a system for identifying unreliable news articles. The general workflow involve preprocessing the text data with nltk and PorterStemmer, converting the text data into numerical features with CountVectorizer, and training a machine learning model such as MultinomialNB on a dataset of reliable and unreliable news articles. Once trained, the model can be used to predict whether new articles are reliable or unreliable based on their features.
