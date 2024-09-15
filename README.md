
## Abstract

This project focuses on the classification of the BLOODMINST dataset using both Deep Neural Networks (DNN) and Convolutional Neural Networks (CNN). The dataset consists of 17,092 3-channel images across 8 classes. We normalized the pixel values and split the data into training, validation, and test sets.

### Part 1: DNN
We implemented a DNN with a simple architecture:
- Layer 1: 128 neurons, ReLU activation
- Layer 2: 64 neurons, ReLU activation
- Output: SoftMax activation for classification

The DNN achieved around 80% accuracy.

### Part 2: CNN
We built a CNN with two convolutional layers, each followed by MaxPooling, a dense layer of 128 neurons, and Dropout to prevent overfitting. The output layer used SoftMax for classification. We evaluated different activation functions (ReLU, ELU, Tanh, and Sigmoid), with ReLU, ELU, and Tanh showing superior performance in terms of both accuracy and loss.

The models were trained using the Adam optimizer and sparse categorical cross-entropy loss function. ReLU, Tanh, and ELU functions demonstrated the best results compared to Sigmoid.
