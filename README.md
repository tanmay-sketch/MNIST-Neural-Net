# MNIST-Neural-Net
Built an MNIST Neural Network Classifier with 88% accuracy

This repository contains an Neural Network for the MNIST database, built just using numpy and math. It is a great way of understanding deep learning concepts. Just through this activity I was able to understand the fundamentals of Neural Networks. 

## STEPS TO BUILD THE NEURAL NETWORK: 

1. Loading the data and splitting the data into training and testing. (Shuffling the data before splitting the data)

2. Creating the functions for different steps in the neural network
	* Initialize parameters
	* Activation Function (ReLU) 
	* Forward Propagation
	* Derivative of Activation function
	* One Hot function
	* Backward propagation
	* Updating the parameters
	* Gradient descent
	* Predictions and Accuracy Functions

3. Running the gradient descent and finding out the accuracy of the model

## Math behind the Neural Network 

The neural network has a simple two layer architecture. Input layer $\alpha^{[0]}$ will have 784 units corresponding to the 784 pixels in the 28x28 image. A hidden layer $\alpha^{[1]}$ will have 10 units with ReLU activation, and finally our output layer $\alpha^{[2]}$$ will have 10 units corresponding to the 10 digit classes with a softmax function

### Forward Propagation
$$ 
Z^{[1]} = W^{[1]}X+b^{[1]}
$$
