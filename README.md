# Udacity-Dog-Breed-Project

The Jupyter-Notebook-File [dog_app.ipynb](dog_app.ipynb) includes my
solution to the Dog-Breed-Classifier-Project in the Deeplearning-Nanodegree. 

## General Description

An algorithm with the following functionality is implemented: Given an arbitrary 
image it first decides if a human or a dog or neither of the two is shown. If the
image shows a dog it then detects the breed of the shown dog. If it shows a person
the algorithm outputs the most resembling dog breed.

## First Part of the Algorithm

As explained above, the algorithm first tries to decide if a given image shows 
a human, a dog or neither of the two. This is done via the following strategies:

* How does the algorithm decide if a human being is shown?: OpenCV's 
  implementation of Haar feature-based cascade classifiers is used to
  recognize faces.
* How does the algorithm decide if a dog shown?: A VGG-16 model which
  is already pre-trained on the ImageNet dataset is used to recognize 
  dogs.
  
## Second Part of the Algorithm

In the second part the algorithm estimates the dog breed of a shown dog
(respectively the most resembling dog breed for a shown person). This is 
done via deep convolutional neural networks. Two different networks get tested:

1. A newly trained newly architectured deep convolutional neural network.
2. A pre-trained VGG-16 model (again pre-trained on the ImageNet dataset).


