## CNN Classifying Fashion MNIST
Simple convolutional neural network (CNN) classifying clothing images from the Fashion MNIST dataset.
# Problem Overview
Fashion MNIST is a popular dataset having thousands of pictures of clothes. It has been widely used to develop machine learning models for computer vision. The dataset is composed of 28x28 images in grayscale. Its popularity comes from being a "sibling" of the MNIST dataset of handwritten digits used in the paper that originally proposed the LeNet CNN. Although being similar, Fashion MNIST was conceived as a substitute for the original MNIST dataset. It is agreed by many that MNIST is too simple, overused and not really able to represent the challenges in computer vision. Hence, Fashion MNIST was created and is now included in most machine learning libraries.

In Fashion MNIST we have 10 classes, just like in the original MNIST dataset. The main difficulty introduced by the new dataset is that some classes are composed of images that are very similar to each other (shirt and t-shirt classes, for instance). Other than that, the dataset also has a lot more images, 70,000. Not many algorithms are able to achieve a great performance of above 99% accuracy, as it is the case with original MNIST. Next table has a summary on Fashion MNIST's classes:

Class	Label
0	T-shirt/top
1	Trouser
2	Pullover
3	Dress
4	Coat
5	Sandal
6	Shirt
7	Sneaker
8	Bag
9	Ankle boot

Analysis Introduction
CNNs are the number 1 option for image classification since CNN models started dominating the ILSVRC computer vision competition. In this project, we stick to the current state of affairs and build a simple CNN archictecture with the objective of achieving above 90% accuracy classifying Fashion MNIST.

We show how a simple CNN with 3 convolutions and 4 fully connected layers can achieve 91% in accuracy, even without preprocessing the Fashion MNIST images. The model is built and evaluated using only TensorFlow and Scikit-learn APIs. We also visually evaluate the results of our model with an image grid having actual and predicted labels for a couple of random images:

fashion_mnist_classified2

Besides that, we use a confusion matrix to support our analyses, where the main diagonal represents our model's correct prediction.
