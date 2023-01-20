# MNIST-Neural-Net
Built an MNIST Neural Network Classifier with 88% accuracy

This repository contains a Neural Network for the MNIST database, built from the scratch using numpy and math. It is a great way of understanding deep learning concepts. Just through this activity I was able to understand the fundamentals of Neural Networks. 

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

The neural network has a simple two layer architecture. Input layer $\alpha^{[0]}$ will have 784 units corresponding to the 784 pixels in the 28x28 image. A hidden layer $\alpha^{[1]}$ will have 10 units with ReLU activation, and finally our output layer $\alpha^{[2]}$ will have 10 units corresponding to the 10 digit classes with a softmax function

### Forward Propagation
$$ Z^{[1]} = W^{[1]}X+b^{[1]} $$

$$A^{[1]} = g_{ReLU}(Z^{[1]}) $$

$$Z^{[2]} = W^{[2]}A^{[1]}+b^{[2]} $$

$$A^{[2]} = g_{softmax}(Z^{[2]}) $$


### Backward Propagation
$$dZ^{[2]} = A^{[2]} - Y $$

$$dW^{[2]} = \frac{1}{m} dZ^{[2]} A^{[1]T}$$

$$dB^{[2]} = \frac{1}{m} \sum dZ^{[2]}$$

$$dZ^{[1]} = W^{[2]T}dZ^{[2]} \cdot  \* g^{[1]} \prime (z^{[1]})$$

