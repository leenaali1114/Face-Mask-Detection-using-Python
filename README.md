# Face-Mask-Detection-using-Python
 A real-time system to detect whether the person on the webcam is wearing a mask or not.


### Download the Dataset
The dataset we are working on consists of 1376 images with 690 images containing images of people wearing masks and 686 images with people without masks.
https://www.kaggle.com/code/ronikdedhia/face-mask-detection

We are going to build this project in two parts. In the first part, we will write a python script using Keras to train face mask detector model. In the second part, we test the results in a real-time webcam using OpenCV.

### Testing The Model in Real-Time
To test our model in real-time, I’ll be using the VideoCapture function in the OpenCV library in Python. The Cascade classifier, designed by OpenCV, was used to detect the frontal face in live video via detectMultiScale. We can use a while loop to continue capturing images from the webcam.

Our machine learning model will then determine whether or not a face mask is worn in real-time. Based on the performance and accuracy of our model, the result of the binary classifier will be indicated by showing a green rectangle superimposed around the section of the face indicating that the person at the camera is wearing a mask, or a red rectangle indicating that the person on camera is not wearing a mask.

