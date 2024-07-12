# Next Word Prediction using LSTM
This repository contains a project that demonstrates how to build and train a Long Short-Term Memory (LSTM) neural network to predict the next word in a sequence. The project is implemented using Python and TensorFlow/Keras.

# Dataset
The dataset used for training the model should be a plain text file containing a large corpus of text. The text is preprocessed to create sequences of words, which are then used to train the LSTM model. You can use any text corpus for this purpose.

# Model Architecture
The LSTM model is built using Keras and consists of the following layers:

An embedding layer to convert words into dense vectors of fixed size.
One or more LSTM layers to capture the sequential dependencies.
A dense layer with a softmax activation function to predict the probability distribution of the next word.

# Training
The training process involves the following steps:

Preprocess the text data to create input sequences.
Tokenize the text and convert words to integer sequences.
Pad the sequences to ensure uniform length.
Split the data into training and validation sets.
Define and compile the LSTM model.
Train the model using the training data.
Save the trained model to disk.
# Prediction
To predict the next word, the trained model takes a sequence of words as input and outputs the word with the highest probability. The prediction process involves the following steps:

Load the trained model.
Tokenize and pad the input sequence.
Use the model to predict the next word.
Convert the predicted integer back to a word.
