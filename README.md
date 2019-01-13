# DogBreedClassifier

Classifying dog images according to their breed.
tensorflow is used in the project. 

First, classifier decides if the picture is of human or dog. If it is of dog,
then it predicts the breed. If it is of human, it outputs the dog breed he 
most resembles. If it is neither dog or human, it gives a warning message to 
feed another picture of a dog. It also gives the category the imagenet classification dictionary includes.

The model uses transfer learning. It employs network Resnet50 pretrained on imagenet dataset which includes 1000 categories. 

Gets bottleneck features from Resnet50 model. Uses bottleneck features as an 
input to classifier.


