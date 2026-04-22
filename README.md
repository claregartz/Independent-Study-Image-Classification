# Independent-Study-Image-Classification

This repo contains the report, code and data for my Independent Study in the Fall of 2025.

The central objective of this independent study is to understand how a program can learn to identify the values of
different handwritten digits accurately. I am employing a basic neural network (NN) to
achieve this with the MNIST dataset. This project examines the contribution of linear
algebra and multivariable calculus concepts to the training process. The performance of
the model is based on the accuracy and confidence in the classification of the validation
data.

The entire project is described in main.pdf, train.csv is the dataset, and the ipynb files are code for the different models I created.

To run the notebooks you need to install numpy, pandas, scikit-learn, pytorch and matplotlib. I used pip to install all of them, e.g.
> pip3 install torch torchvision torchaudio

for pytorch for example.

You also need to unzip the file train.csv.zip.

binary-experiments.ipynb shows examples of fitting linear models and logistic regresssion models but using the library solvers as well as gradient descent directly. I also implement logistic regression using pytorch - which is usually used for full neural networks. The goal here was to see how the models and loss functions behaved with the gradient descent approaches. Also I produced plots of the weights to get an intuition for what really was going on.

NNcode.ipynb trains a neural network with two hidden layers to classify the MNIST digits using just the linear algebra code from numpy. In particular it calculates gradients directly and therefore only supports limited neural network architectures.

