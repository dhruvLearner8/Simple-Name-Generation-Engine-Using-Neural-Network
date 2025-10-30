#Makemore-Inspired Name Generator

A simple name generation project inspired by Andrej Karpathy’s makemore series.
The project explores character-level language modeling, starting from basic count-based bigram models to a small neural network that learns to generate realistic names.

This project is built step-by-step following Karpathy’s educational approach:

Bigram Model (Statistical):
Uses simple frequency counts of character pairs to generate random names.

Neural Network (Learned):
Implements a tiny neural net trained on the same dataset of names to predict the next character, one at a time.

Both models output synthetic “names” that resemble the training data.

##Bigram Model

Loaded and preprocessed a text dataset of names

Built a character vocabulary and mapping between characters ↔ indices

Computed count matrices and bigram probabilities

Implemented sampling from the probability distribution to generate random names

Added smoothing to handle unseen character pairs

Visualized the bigram probability matrix using matplotlib

##Neural Network Model

Implemented data preparation pipeline (inputs and targets)

Built a simple feedforward neural network from scratch using PyTorch

Embedding layer

Hidden layer with non-linear activation (e.g. ReLU or Tanh)

Output layer predicting next character logits

Wrote the training loop manually (forward pass, loss computation, backward pass, optimizer step)

Used cross-entropy loss for next-character prediction

Implemented sampling from the trained model to generate new names

Tuned hyperparameters (learning rate, batch size, number of iterations)

Compared results between the bigram model and the neural network
