# RNN
Recurrent neural networks (RNN) are the state of the art algorithm for sequential data and are used by Apple's Siri and and Google's voice search. It is the first algorithm that remembers its input, due to an internal memory, which makes it perfectly suited for machine learning problems that involve sequential data. 


RNN’s can remember important things about the input they received, which allows them to be very precise in predicting what’s coming next. This is why they're the preferred algorithm for sequential data like time series, speech, text, financial data, audio, video, weather and much more. Recurrent neural networks can form a much deeper understanding of a sequence and its context compared to other algorithms.Like FeedForward Neural Networks and Convolutional Neural Networks RNN's utilize training data to learn .They are distinguished by their memory as they take information from prior inputs which  influence the current input and outputs. While traditional Deep Neural networks assume that outputs and inputs are independent on each other . But RNN's output  depend on the prior elements within the sequence.

Through this process, RNNs tend to run into two problems, known as exploding gradients and vanishing gradients. These issues are defined by the size of the gradient, which is the slope of the loss function along the error curve. When the gradient is too small, it continues to become smaller, updating the weight parameters until they become insignificant—i.e. 0. When that occurs, the algorithm is no longer learning. Exploding gradients occur when the gradient is too large, creating an unstable model. In this case, the model weights will grow too large, and they will eventually be represented as NaN. One solution to these issues is to reduce the number of hidden layers within the neural network, eliminating some of the complexity in the RNN model.

Mainly Here we see about LSTM RNN Architecture

# LONG SHORT TERM MEMORY 

This is a popular RNN which was introduced by Sepp  Hochreiter and Juergen Schmidhuber as a solution to vanishing gradient problem .they work to address the issue of long term independencies , i.e. if the previous state that is influencing the current  prediction is not in the  recent past thenn RNN model may not be able to accurately predict the current state.

for the RNN to connect the information. To remedy this, LSTMs have “cells” in the hidden layers of the neural network, which have three gates–an input gate, an output gate, and a forget gate. These gates control the flow of information which is needed to predict the output in the network.  For example, if gender pronouns, such as “she”, was repeated multiple times in prior sentences, you may exclude that from the cell state.



