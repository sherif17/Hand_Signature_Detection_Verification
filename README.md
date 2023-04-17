
# Handwritten Signature Detection and Verification
This project is designed to identify whether a handwritten signature is real or forged and detect the signature in a document. It consists of two parts:

* Signature Detection
* Signature Verification

## Signature Verification 

  The dataset for signature verification can be found [here](https://drive.google.com/file/d/1WqIhqp9JJ65SZPs9v868P_-SBCVTR2By/view). It contains images of signatures from 5 different people (personA, personB, personC, personD, personE). Each person's dataset has a training and a testing folder, each containing 40 and 8 images respectively.
  
  ![image](https://user-images.githubusercontent.com/43541909/232468859-d8c584bf-9dc5-4c80-a5ae-86814ef430c7.png)


We created a Siamese model for signature verification and achieved a test accuracy of 93% on the 40 test images.

 ## Signature Detection
The dataset for signature detection can be found [here](https://drive.google.com/file/d/1gew1zSfSZKiUKGPGc3bpGXbO03HvE9-_/view). It contains training and testing images with corresponding detection labels. Each image in the training set has a corresponding text file with the same name as the image. The text file contains one or more rows, each representing the bounding box of a single signature. Each row has 4 values: x1, y1, x2, y2.

![image](https://user-images.githubusercontent.com/43541909/232469374-0ae15338-8f63-4475-b838-fc95d716a6ca.png)


To detect signatures, we trained a model on the training set and achieved a precision of X%, recall of Y%, and F1-score of Z% on the testing set.

## Requirements
The following packages are required to run the code:

* Tensorflow
* Yolo 5
* Keras
* OpenCV
* Numpy
* Usage

To run the signature verification code, run the signature_verification.py file with the path to the image and the path to the trained model as arguments.

To run the signature detection code, run the signature_detection.py file with the path to the image and the path to the trained model as arguments.

## Credits
This project was developed by [Sherif Ahmed] as part of a [Advanced Computer Vision at ITI].
