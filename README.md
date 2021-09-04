### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Theory background](#theory background)
5. [Acknowledgements](#licensing)

## Installation <a name="installation"></a>

The code should run in Python 3 with no problems. No additional packages are needed. 

Follwoing are the used libraries:
  - os
  - struct
  - numpy
  - sys
  - sklearn

## Project Motivation<a name="motivation"></a>
In this example a very simple Neural Network is set up. The idea behind this to show how a Neural Network is set up and implemented instead of using it as a black box. 

## File Descriptions <a name="files"></a>
The file "Neural Network implementation" is a jupyter file in which all code can be found. 
The training and test set, which are used here is the "mnist_784" dataset which is part of the sklearn package.

The data are images which are saved as vectors in a numpy array. To plot the image, the vectors need to be reshaped (28x28 pixels).

## Theory background <a name="files"></a>
Before the model can be used, it needs to be trained with a training set. In each epoch the training set is shuffled randomly to avoid being trapped in a local minimum. Furtermore, the training set is split into small batches before computing the gradient. This accelerates the learning of the model. 

For the next step, the weights and biases of the NN needs to be initialized. For the weights random numbers are chosen, the biases are filled with zeros. 
With the forward propagation step (inserting weights and biases into the NN), the activation of the output layer can be determined. This is formulated as follows:

Z⁽h⁾: net input of the hidden layer
A⁽h⁾: activation of the hidden layer
Z⁽out⁾: net input of the output layer
Z⁽out⁾: activation of the output layer

For the activation function, the sigmoid activation function is used: \frac1 / (1 + e^{z})

(E=mc^2\)，$$x_{1,2} = \frac{-b \pm \sqrt{b^2-4ac}}{2b}.$$
<img src="https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" title="\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" />


## Licensing, Authors, Acknowledgements<a name="licensing"></a>
The code used here can be find in the book: Python Machine Learning by Sebastian Raschka & Vahid Mirjalili
