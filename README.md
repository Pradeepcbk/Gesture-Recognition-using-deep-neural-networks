# Gesture-Recognition-using-deep-neural-networks
A project for activity recognition using deep neural networks

Here, Gestures are recorded using an android application (3d-accelerometer readings) - PhonePi. The dataset is stored in the folder - Training_Data.

#### Features are extracted as per the paper https://link.springer.com/chapter/10.1007/978-3-642-02830-4_4 in the file Feature_Extraction.py and stored in the file FeaturesSet.xlsx

This file - FeaturesSet.xlsx is re-arranged to get training data in sheet 0 and test data in sheet 1 of arrays.xlsx

The algorithm to build, train and predict the gestures using deep-neural networks (using Keras on top of Tensorflow) is implemented in DNN.py

2 Classes for 2 different gestures "UP" and "DOWN" are created.

#### Concept of checkpoints are used for storing the trained weights. The same is being loaded to avoid the training time at the time of prediction. For more information on this: https://www.tensorflow.org/guide/checkpoints

10-fold validation approach is used to determine the percentage of correct results - 95%

The original project which is modified here is present here: https://www.slideshare.net/PradeepSiddagangaiah/gesture-recognition-usinginertialsensors
