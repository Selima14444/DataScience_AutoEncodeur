# Autoencoder Project

## Overview
This project focuses on generating, encoding, and processing messages using a neural network autoencoder. 
The primary steps include generating random messages, applying one-hot encoding, converting the data to PyTorch tensors, constructing and training an autoencoder, and visualizing the learned constellation.

## Prerequisites
Ensure you have the following libraries installed:

- NumPy
- PyTorch
- Matplotlib

## Steps
**1. Generate Random Messages**
   
Generate a vector containing 100,000 random messages. Each message is an integer in the set {1,2,…,𝑀}, where 𝑀 is determined based on a specified 𝑘 value.

**2. One-Hot Encoding**

Apply one-hot encoding to each message. The resulting matrix will have dimensions 𝑁×𝑀.

**3. Convert to PyTorch Tensor**
   
Convert the one-hot encoded matrix to a PyTorch tensor for further processing.

**4. Define Autoencoder**
   
Define the autoencoder model using PyTorch. The autoencoder consists of an encoder that reduces the dimensionality of the input data and a decoder that reconstructs the input data from its encoded form. Additional layers, such as normalization and noise layers, are incorporated to enhance the learning process.

**5. Train the Model**
    
Prepare the data for training by creating a custom dataset and data loaders. Define the training and testing functions to train the autoencoder and evaluate its performance. Use cross-entropy loss as the loss function and Adam optimizer for training. Split the dataset into training and testing sets, and train the model for a specified number of epochs.

**6. Plot the Learned Constellation**

Visualize the learned constellation by plotting the encoded representations using Matplotlib. Compare this constellation with a traditional M-PSK constellation used in digital communications.

## References
- [Autoencoder Research Paper](https://arxiv.org/pdf/1702.00832)
- [PyTorch Normalization Documentation](https://pytorch.org/docs/stable/generated/torch.nn.functional.normalize.html)
  
This README provides a comprehensive guide to implementing and training an autoencoder model for message encoding and decoding tasks.
