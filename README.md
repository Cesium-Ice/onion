# Onion or Not?

Dataset of The Onion articles and real "Onion-like" news articles from the subreddit r/NotTheOnion. The Onion articles are labeled 1 and the r/NotTheOnion articles are labeled 0.

I decided to do this project as my first foray into NLP because I am a fan of both the onion and r/nottheonion. 

The dataset was extracted using pushshift API and the article titles were cleaned and one-hot encoded before being used to train some models. 

Models Used: 
Global Pooling
LTSM
Bidirectional LSTM
CNN

After the model were trained the training and validation accuracy and losses were plotted and the accuracy was calculated to evaluate the model results.

Currently, the best performing models are Bidirectional LSTM (0.855 accuracy on test set) and CNN (0.831 accuracy on test set)

Next Steps:
- I would like to try using Word2Vec to create the word vectors instead of just one-hot encoding to see if I can improve the model accuracy
- I would like to set up a website to let users classify whether articles are from the onion or not and compare their performance to that of the trained models


