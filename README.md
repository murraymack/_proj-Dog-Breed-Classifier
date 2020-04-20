# _proj-Dog-Breed-Classifier
## Dog Breed Classifier Project

This repository contains a jupyter notebook which runs through building a CNN for classifying dog breeds from a list of 133 breeds.

The original structure of the notebook is sourced from Udacity course curriculum, Deep Learning Nanodegree.

## Reference Data, etc.:

[Haar feature-based cascade classifiers](http://docs.opencv.org/trunk/d7/d8b/tutorial_py_face_detection.html)<br>
[Dog Image Data](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip)<br>
[Human Image Data](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip)<br>

### Hand-made Architecture
The naive architecture coded from scratch was:
>nn.Conv2d(3, 32, 3, stride=2, padding=1)<br>
>nn.Conv2d(32, 64, 3, stride=2, padding=1)<br>
>nn.Conv2d(64, 64, 3, stride=1, padding=1)<br>
        
>nn.MaxPool2d(2, 2)<br>
>nn.Dropout(p=0.25)<br>
        
>nn.Linear(3136,1028)<br>
>nn.Linear(1028,512)<br>
>nn.Linear(512,134)<br>
