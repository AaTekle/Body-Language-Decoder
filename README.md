# Body Language Decoder

Welcome to my Body Language Decoder project! This project aims to decode human emotions and reactions by analyzing facial expressions and gestures using computer vision techniques and machine learning. The project leverages the power of Python, Mediapipe, OpenCV (cv2), csv, NumPy, Pandas, scikit-learn (sklearn), and pickle to create an interactive and insightful tool for understanding body language.

![](https://github.com/AaTekle/Body-Language-Decoder/blob/main/gif/0816.gif)


## Table of Contents

- [Introduction](#introduction)
- [Technical Overview of Mediapipe](#technical-overview-of-mediapipe)
- [Creating the Dataset](#creating-the-dataset)
- [Real-Time Facial Expression Analysis](#real-time-facial-expression-analysis)
- [Probability Box/Function](#probability-boxfunction)
- [Future Enhancements](#future-enhancements)

## Introduction

Body language is a crucial aspect of human communication, conveying emotions and reactions that may go unspoken. This project dives into the realm of computer vision and machine learning to decode these non-verbal cues, providing insights into human behavior.

## Technical Overview of Mediapipe
![MediaPipe](https://editor.analyticsvidhya.com/uploads/53474logo_horizontal_color.png)
Mediapipe, developed by Google, is a Computer Vision library that provides a wide range of pre-trained models for various computer vision tasks, ex. facial landmark detection. It allowed me to easily extract facial landmarks from images / video streams, enabling accurate tracking of key points on the face, such as eyes, nose, mouth, and eyebrows. This technology forms the backbone of this project, enabling me to analyze and interpret facial expressions.

## Creating the Dataset

Data is needed pre-training, Utilized the `csv` module to collect and organize the coordinates of facial landmarks provided by Mediapipe. I captured and labeled facial landmarks of my own various emotional states, creating a dataset. The coordinates were created in real time while I displayed emotional states, it was cool that I got to create the dataset in such an interactive way in real time, seeing my facial expressions being translated into thounsands of numerical values (coordinates).

## Real-Time Facial Expression Analysis

The core functionality of the Body Language Decoder lies in its real-time facial expression analysis. By leveraging OpenCV (cv2), I captured video frames from a webcam feed and process them using the Mediapipe facial landmark model. The coordinates of facial landmarks are then saved to the dataset, creating a dynamic representation of facial expressions over time.

## Probability Box/Function

Used NumPy to construct and display a probability box or function within the Body Language Decoder. This visual representation offers users an intuitive way to understand the likelihood of different emotions being expressed based on the facial landmark data.

## Conclusion:

Thank you for exploring my Body Language Decoder project. I hope this tool provides insight into CV when it comes to decoding human expression. If you have any questions or suggestions, please feel free to reach out to me!
