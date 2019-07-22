# Hollywood-Actors NLP using LSTM implemented with TensorFlow and Keras
### Can we predict if an actor won the Oscar based on the career article in Wikipedia?

The model uses LSTM NLP to analyze the "Holywood Actors" articles in Wikipedia. The list of actors was obtained from the Wikipedia page that lists all actors that appear on ['Hollywood Walk of Fame motion picture stars'](https://en.wikipedia.org/wiki/List_of_actors_with_Hollywood_Walk_of_Fame_motion_picture_stars). This is not a complete list of actors but it represents significant stars in the Hollywood industry. 

The list includes around 900 actors 200 of them were nominated to Oscar and another 200 won an Oscar. 
The model classifies actors as 'won' the Oscar, 'nominated' to Oscar or 'did not won or nominated to the oscar'. 

Here, I focus efforts on efficient and quick preprocessing that will enhance the signal. 
 * I perform basic cleaning of the data 
 * Used nltk sentence tokenizer as an input to create stem words.
 * Remove stop words
 * Perform word embodied as part of the deep neural network. 
 
These steps allow me to reduce the dimension of the problem, and work with relatively clean data. Which is particularly important for this data set which is quite small. 

 * I choose to use an artificial recurrent neural network (RNN) architecture of the type Long short-term memory (LSTM).  [LSTM](https://en.wikipedia.org/wiki/Long_short-term_memory) networks are well-suited to classifying, processing and making predictions based on time series data.
 
### Reference
#### # Extracting the names of actors and the oscar nomination : https://qxf2.com/blog/web-scraping-using-python/ , https://pypi.org/project/wikipedia/
#### # Extracting the career : https://pypi.org/project/Wikipedia-API/0.2.0/
#### # Model : https://github.com/udacity/deep-learning/blob/master/sentiment-rnn/Sentiment_RNN_Solution.ipynb
