# Hollywood-Actors
## Can we predict if an actor won the Oscar based on the career article in Wikipedia?

I analyze the "Holywood Actors" articles in Wikipedia. I choose to use the list of actors that appears on ['Hollywood Walk of Fame motion picture stars'](https://en.wikipedia.org/wiki/List_of_actors_with_Hollywood_Walk_of_Fame_motion_picture_stars). This is not a complete list of actors but it represents significant stars in the Hollywood industry. The list includes around 900 actors 200 of them were nominated to Oscar and another 200 won an Oscar. 
I wanted a model that classify actors that 'won' the Oscar, 'nominated' to Oscar and 'did not won or nominated to the oscar' will demonstrate some of my skills in data processing and modeling. 
Due to obviously limited time, I focus my efforts on efficient preprocessing that will enhance the signal. 
 * I perform basic cleaning of the data 
 * Used nltk sentence tokenizer as an input to create stem words.
 * Remove stop words
 * Perform word embodied as part of the deep neural network. These steps allow me to reduce the dimension of the problem, and work with relatively clean data. Which is particularly important for this data set which is quite small. 
 * I choose to use an artificial recurrent neural network (RNN) architecture of the type Long short-term memory (LSTM).  [LSTM](https://en.wikipedia.org/wiki/Long_short-term_memory) networks are well-suited to classifying, processing and making predictions based on time series data.
