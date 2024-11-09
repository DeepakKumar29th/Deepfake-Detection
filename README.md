# DeepFake Video Detection

This project, named DeepFake Video Detection, aims to identify whether a given video is genuine or deepfake. The solution is implemented using a pre-trained machine learning model and is served as a web application using Flask. The project can be easily run on both local machines and cloud platforms.

# Introduction

With the rise of AI-generated content, detecting deepfake videos has become increasingly important. This project leverages deep learning to detect manipulated videos using TensorFlow and Keras. The goal is to provide a reliable tool for identifying deepfake content in videos.

# Project Architecture

The project is divided into two main parts:

DeepFake Detection Model: A convolutional neural network (CNN) model trained to classify videos as real or fake.
Web Application: A Flask-based web interface for users to upload videos for analysis.

# Features

-Deepfake Detection: Uses TensorFlow to detect AI-generated manipulations in videos.
-Web Interface: Built with Flask, allowing users to upload videos for analysis.
-Real-Time Results: Provides immediate feedback on whether a video is a deepfake.

# Implementation
Video Detection Code-
The deepfake detection model was developed using TensorFlow. Here's an overview of the core libraries used:

# Importing required libraries

```shell
import tensorflow as tf
import numpy as np
import cv2
```


 -Model Training:The deepfake detection model was trained on a dataset of real and manipulated videos. The model architecture includes several convolutional layers to identify patterns and inconsistencies typical in deepfakes.

-Model Optimization: The training process was optimized using hyperparameter tuning, data augmentation, and regularization techniques to improve accuracy.

# Web Interface with Flask
The project includes a Flask-based web server for users to interact with the model. The web application allows video uploads for real-time deepfake detection.

To run the application, follow these steps:

-Install Dependencies: Make sure you have the required libraries installed:

```shell
pip install tensorflow flask opencv-python
```

-Run the Application: Start the Flask server using the command:

```shell
python app.py
```

Once you see the following URL in the logs: http://127.0.0.1:5000/, open it in your browser.

# Sample Output

The application will display whether the uploaded video is authentic or a deepfake, along with confidence scores.

# Technologies Used

-TensorFlow: For deepfake video analysis.
-Flask: To create a web interface.
-OpenCV: For video processing.
-Jupyter Notebook: For initial model development and testing.

# Deepfake Detection Web Interface
![Screenshot 2024-11-09 001518](https://github.com/user-attachments/assets/e18ef35a-666e-4626-9a7c-d3182e5977cf)

# Uploading Video for Detection
![Screenshot 2024-11-09 130431](https://github.com/user-attachments/assets/8095b6b4-2960-45cd-bb20-40547b7cf436)

# The uploaded vedio is REAL with Confidence: 0.35
![Screenshot 2024-11-09 130644](https://github.com/user-attachments/assets/8ca8d3cb-f680-4ddf-8e6b-b57cb3509823)


# Uploading Video for Detection again!
![Screenshot 2024-11-09 130839](https://github.com/user-attachments/assets/53285465-8eba-4b68-b123-fa6a8bf898fb)


# The uploaded vedio is FAKE with Confidence: 0.64
![Screenshot 2024-11-09 130802](https://github.com/user-attachments/assets/7bd02b8e-f2cd-4b6c-a2d4-394939f38cf1)


