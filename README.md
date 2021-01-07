# MNIST 

This problem is reffered to as the "Hello World" of deep learning, because for most students it is the first deep learning algorithm they see. The dataset is called MNIST and refers to handwritten digit recognition.
It provides 70,000 images(28x28 pixels) of handwritten digits (1 digit per image). Where input values are from 0 (purely black) to 255 (purely white).
The approach for the deep neural networks is to "Flatten" each image into a vector 784x1. Each pixel corresponds to the intensity of the color.
The goal is to write an algorithm that detects which digit is written. Since there are only 10 digits (0,1,2,3,4,5,6,7,8,9), this is a classification problem with 10 classes.

input_layer = 784 input_units, hidden_layer = 50 hidden_layer_units(2 hidden layers), output_layer = 10 output_units
We will use one-hot-encoding for both the outputs and the targets(because for instance: digit 5 will be represented as 00000100000).
Since we would like to see the probability of a digit being rightfully labeled, we will use a softmax activation function for the output layer.

The MNIST action plan :
- Step 1: Prepare our data and preprocess it.
- Step 2: Outline the model and choose the activation functions you want to employ.
- Step 3: Set the appropriate advanced optimizers and loss function.
- Step 4: Make it learn.
- Step 5: Testing the accuracy of the model regarding the test dataset.