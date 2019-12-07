# COMP4651-Topics-Classifier
We would like to create a classifier that can be used to identify the 
topics of a question to facilitate a module of our Final Year Project.
We experimented multiple common algorithm for text classification, including **DecisionTree, K Nearest Neighbors, Random Forest, Linear SVC, Logistic Regression and Deep Learning (MLP and RNN)**

# Methodology
For the aforementioned models except the Deep Learning Models (RNN), we interchangeably used word2vec to produce a word embedding and TF-IDF to produce sentence vectors to feed in the algorithm.
The RNN models contains an embedding layer to come up with a self-trained embeddings, while one version of RNN contain an extra layer of Attention and and the other does not.

# Result
RNN without Attention perform the best in our case. It archieves about an average of 0.85 accuracy. The detail results can be refered to the report.
Some other insights include word2Vec performs generally worse than TF-IDF, probably because of the data points are too sparse in word2Vec while our dataset contain limited amount of unique words and mainly academic phrases.
