# CIFAR-10-image-classification-using-fully-connected-NN
This is an image classification project using pure python and fully connected nural networks from scratch!
## Problem description
In this problem, we want to classify the images of the CIFAR-10 dataset. This dataset is a smaller version
of the CIFAR-100 dataset, limited to images from 10 different categories.
to reduce the computational complexity, we only use the images of the first 4 classes of this dataset.
The dimensions of the images in this dataset are equal to 32 (length) by 32 (width) by 3 (RGB color channels).


<img width="449" alt="image" src="https://user-images.githubusercontent.com/72692826/178138107-ec802ef4-626a-472b-8578-fef952e65795.png">

## Neural network architecture and details

For this neural network, we consider two hidden layers, each of which has 16 neurons.
So the structure of our neural network will be as follows:

<img width="511" alt="image" src="https://user-images.githubusercontent.com/72692826/178138211-9d8b3e3b-62a4-4490-9d11-ce5fddd82064.png">
The pseudo-code of our neural network learning process according to the Descent Gradient Stochastic method is as follows: 

<img width="617" alt="image" src="https://user-images.githubusercontent.com/72692826/178138433-553ce5a1-4900-47eb-8b6f-05426742b18b.png">

## Feedforward

to calculate the output from the input in neural networks, the following operation
is done in each layer:
<img width="301" alt="image" src="https://user-images.githubusercontent.com/72692826/178138522-cb3d2476-cfb5-4690-bb65-9e4a212eca0e.png">

As a result, in the implementation of the neural network, for the weights between both layers, we consider a k by n matrix that
k is the number of neurons in the next layer and n is the number of neurons in the current layer.
<img width="603" alt="image" src="https://user-images.githubusercontent.com/72692826/178138625-e45d0149-df6e-4e71-b4db-7b48ff417a85.png">

## Backpropagation

As you know, neural network learning process is in fact minimizing the cost function. This is done with the help of Descent Gradient method, where by obtaining the partial derivatives of the cost function
for all the parameters (that is, the same gradient), we make the desired changes on the parameters. Obtaining these derivatives is done with the help of backpropagation.

<img width="257" alt="image" src="https://user-images.githubusercontent.com/72692826/178138726-539795fc-1d2f-48d7-b385-a66b291bef12.png">


<img width="284" alt="image" src="https://user-images.githubusercontent.com/72692826/178138728-3c5c6a57-6b0e-453c-9538-20795a0fcf0e.png">

## Vectorization

So far, we only worked with the first 200 data of the dataset because the execution time of the current training process takes a lot of time and it's not optimal for network learning. To solve this problem, we apply vectorization. This means that instead of using for loops, the desired operation is done in the form
Matrix operations (matrix and vector multiplication and addition, internal multiplication, transposition and applying functions on each element)

## Persian description
you can see the persian project description below:


[CI_project1.pdf](https://github.com/maedemir/CIFAR-10-image-classification-using-fully-connected-NN/files/9078785/CI_project1.pdf)

