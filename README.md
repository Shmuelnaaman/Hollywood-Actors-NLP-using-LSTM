# Hollywood-Actors NLP using LSTM implemented with TensorFlow and Keras
### Can we predict if an actor won the Oscar based on the career article in Wikipedia?

#### Methods used for the analysis
LSTM, Topic Extraction, Cosine Similarities, TfIdf

## Introduction:
#### Since the performance of the naive model is not satisfactory, here I try another approach that is more elegant (LDA_LSTM_TFIDF.ipynb).
The main reason for the low performance of the naive model is the multi topics in the "Holywood Actors" Wikipedia articles. Some of the topics are not relevant to the target variable. Therefore introduces noise and reduce the performance. 
Here I try a different approach to improve the performance. The idea is to extract and identifies the main topics in the articles using unsupervised learning. That will allow us to choose only relevant input for the model. 
I use the same list of actors that appears on 'Hollywood Walk of Fame motion picture stars' to choose articles. This is not a complete list but it includes most of the significant actors in the Hollywood industry. I also improve the articles extraction so most of the actors have articles. The list includes around 900 actors 200 of them were nominated to Oscar and another 350 won or nominated to an Oscar. 
#### The model classifies actors that won or nominated to the Oscar as one category and the other actors as the second category.
Overview:
I focus my efforts on efficient but basic preprocessing that will enhance the signal. 
I perform basic cleaning of the data, remove numbers, stop words, tokenize words.
Latent Dirichlet allocation (LDA) and Non-Negative Matrix Factorization (NMF) is implemented to identifies 5 different topics in the articles. 
TfIdf and Cosine Similarities are used to identifies the 4 sentences in each document that are most relevant to the target variable "Oscar". 
Only these 4 sentences will be used as input for the model. 
I choose to use an artificial recurrent neural network (RNN) architecture of the type Long short-term memory [LSTM](https://en.wikipedia.org/wiki/Long_short-term_memory). LSTM networks are well-suited to classifying, processing and making predictions based on time series data.
These steps allow me to reduce the dimension of the problem and obtain better results despite the relatively small dataset. 

 
### Reference
#### # [Extracting the names of actors and the oscar nomination](https://pypi.org/project/wikipedia/) ,  https://qxf2.com/blog/web-scraping-using-python/
#### # [Extracting the articles](https://pypi.org/project/Wikipedia-API/0.2.0/)
#### # [Model](https://github.com/udacity/deep-learning/blob/master/sentiment-rnn/Sentiment_RNN_Solution.ipynb)
