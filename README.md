# Face Mask Detection using Python

This project is a real-time face mask detection system that uses a Convolutional Neural Network (CNN) built with Keras to classify faces as either wearing a mask or not. The model is trained on augmented face image data and then integrated with OpenCV to capture live video from a webcam, detect faces using Haar cascades, and make predictions. Detected faces are outlined with colored boxes—green for "mask" and red for "without mask"—providing an efficient way to monitor mask compliance in real-time environments.

## Working

- Model Training Phase
    - A Convolutional Neural Network (CNN) is built using Keras.
    - The model is trained on two classes: mask and without mask.
    - Image augmentation is applied to enhance model robustness.
    - The trained model is saved for later use in real-time detection.

- Real-Time Detection Phase
    - OpenCV captures live video from the webcam.
    - Haar Cascade detects faces in each video frame.
    - Each face is preprocessed and passed to the trained model.
    - The model predicts whether the person is wearing a mask.
    - A colored box (green for mask, red for no mask) and label are displayed on the screen.

## Features
- Real-time mask detection using webcam
- CNN model trained with Keras
- Face detection via Haar Cascade
- Classifies faces as Mask or No Mask
- Color-coded boxes (Green/Red) with labels
- Saves and loads trained model
- Easy exit with Esc key

## Required Modules
- TensorFlow (for model training and prediction)
- OpenCV (for image processing and video capture)
- Keras (for model handling)
- Numpy (for numerical operations
