# Neural Networks and Deep Learning

Notes from [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/), a book by **Michael Nielsen**.

Code examples of algorithms used to classify handwritten digits from the MNIST data set. (using Python 3.8)

> Run `pip install -r requirements.txt` to install the dependencies.

## Misc

1. ### Mnist loader

    A python module used to load and split the MNIST data set into training, validation and testing sets.

2. ### Mnist average darknes

    A naive classifier for recognizing handwritten digits from the MNIST data set. 
    The program classifies digits based on how dark they are.
    
    ```
    $ python mnist_average_darknes.py
    ```

3. ### Mnist SVM

    A classifier program for recognizing handwritten digits from the MNIST data set, using an SVM classifier.

    ```
    $ python mnist_svm.py
    ```

## Deep Learning

4. ### Network

    A module that implement the `stochastic gradient descent` learning algorithm for a feedforward neural network. Gradients are calculated using `backpropagation`.
    
    The model uses the `quadratic cost function(MSE)` and the `sigmoid activation function` for all the layers (except the input layer of course).

    ```
    $ python network.py
    ```

5. ### Network2

    An improvement to the `network` module:
    - Replace the `MSE` with the `cross entropy cost function` to prevent learning slowdown when neurons are saturated (can also be done by adding a `softmax` layer with `minus log-likelihood cost function`).
    - Use `L2 regularization` to reduce the effects of `overfitting` the model.
    - Monitor the training and evaluation accuracy/cost.
    - Save and load the model to/from disk.

    ```
    $ python network2.py
    ```
