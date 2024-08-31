# Body Language Decoder

Welcome to my Body Language Decoder project! This project aims to decode human emotions and reactions by analyzing facial expressions and gestures using computer vision techniques and machine learning. The project leverages the power of Python, Mediapipe, OpenCV (cv2), csv, NumPy, Pandas, scikit-learn (sklearn), and pickle to create an interactive and insightful tool for understanding body language.

![](https://github.com/AaTekle/Body-Language-Decoder/blob/main/gif/0816.gif)


## Table of Contents

- [Introduction](#introduction)
- [Technical Overview of Mediapipe](#technical-overview-of-mediapipe)
- [Creating the Dataset](#creating-the-dataset)
- [Real-Time Facial Expression Analysis](#real-time-facial-expression-analysis)
- [Probability Box/Function](#probability-boxfunction)

## Introduction

This project uses computer vision and machine learning to decode body language, providing insights into human behavior.

## Technical Overview of Mediapipe
![MediaPipe](https://editor.analyticsvidhya.com/uploads/53474logo_horizontal_color.png)
Mediapipe, developed by Google, is a Computer Vision library that provides a pre-trained models for various computer vision tasks, e.g. facial landmark detection. It allowed me to easily extract facial landmarks from images / video streams, enabling accurate tracking of key points on the face, such as eyes, nose, mouth, and eyebrows. This library forms the backbone of this project, enabling me to analyze and interpret facial expressions.

## Creating the Dataset

Data is needed pre-training, Utilized the `csv` module to collect & organize the coordinates of facial landmarks via Mediapipe. I captured and labeled facial landmarks of my own various emotional states, creating a dataset. The coordinates were created in real time while I displayed emotional states, it was cool that I got to create the dataset in such an interactive way within real time, seeing my facial expressions being translated into thounsands of numerical values (coordinates).

## Real-Time Facial Expression Analysis

OpenCV (cv2) allowed me to capture video frames from a webcam feed and process them using the Mediapipe facial landmark model. The coordinates of facial landmarks are then saved to the dataset, creating a representation of facial expressions (features).

## Probability Box/Function

Used NumPy to construct and display a probability box or function within the Body Language Decoder. This visual representation allows one to understand the likelihood of different emotions being expressed based on the facial landmark data.

## Conclusion:

Thank you for looking at my Body Language Decoder project.
