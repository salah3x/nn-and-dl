# Neural Networks and Deep Learning

Notes from [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/), a book by **Michael Nielsen**.

Code examples of algorithms used to classify handwritten digits from the MNIST data set. (using Python 3.8)

1. `mnist_loader`

    A python module used to load and split the MNIST data set into training, validation and testing sets.

2. `mnist_average_darknes`

    A naive classifier for recognizing handwritten digits from the MNIST data set. 
    The program classifies digits based on how dark they are.

3. `mnist_svm`

    A classifier program for recognizing handwritten digits from the MNIST data set, using an SVM classifier.

4. `network`

    A module that implement the `stochastic gradient descent` learning algorithm for a feedforward neural network. Gradients are calculated using `backpropagation`.
    
    The model uses the `quadratic cost function(MSE)` and the `sigmoid activation function` for all the layers (except the input layer of course).
