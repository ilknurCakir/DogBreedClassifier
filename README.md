# DogBreedClassifier




Classifying dog images according to their breed.
tensorflow is used in the project. 



First, classifier decides if the picture is of human or dog. If it is of dog,
then it predicts the breed. If it is of human, it outputs the dog breed he 
most resembles. If it is neither dog or human, it gives a warning message to 
feed another picture of a dog. It also gives the most probable class ResNet50
predicts. The dictonary of imagenet categories to human-readable text is 
obtained from the link https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a . 
It is named resnet_dict in the notebook.



Model that does not use transfer learning achieves 5% accuracy with 20 epochs
training. 



The model uses transfer learning. It employs network ResNet50 that is 
pretrained on imagenet dataset which includes 1000 categories. 



It gets bottleneck features from ResNet50 model. Uses bottleneck features as 
an input to classifier. The classifier part is called 'model'. It receives 
bottleneck features as an input and outputs class probabilities. The most 
probable class is the one with the highest probability.



The trained model gives around 80% accuracy. 



The relevant blogpost can be found 
https://medium.com/@ilknur.chakir/transfer-learning-in-image-classification-5633ca985958


