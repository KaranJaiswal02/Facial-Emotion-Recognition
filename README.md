# Facial Emotion Recognition

This repository contains an implementation of a Facial Emotion Recognition system. The system leverages machine learning techniques to classify human facial expressions into distinct emotional categories such as happiness, sadness, anger, and surprise.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)

## Introduction

Facial emotion recognition plays a crucial role in numerous applications such as human-computer interaction, mental health monitoring, and sentiment analysis. This project implements a system that detects emotions from facial images using modern deep learning techniques.

## Features

- **Real-time Emotion Detection**: Recognize emotions in real-time from webcam feeds.
- **Pre-trained Models**: Leverages pre-trained models for improved accuracy and faster training.
- **User-friendly Interface**: Simple interface for testing and visualizing results.

## Technologies Used

 - opencv-python
 - deepface
 - tf_keras

## Dataset

The system is trained on the [FER2013 dataset](https://www.kaggle.com/msambare/fer2013), which contains 35,887 grayscale, 48x48 pixel face images labeled with one of seven emotions:

1. Angry
2. Disgust
3. Fear
4. Happy
5. Sad
6. Surprise
7. Neutral

## Model Architecture

The model architecture is based on a Convolutional Neural Network (CNN) to effectively extract spatial features from the input images. Key layers include:

- Convolutional layers with ReLU activation
- MaxPooling layers for downsampling
- Dropout layers to prevent overfitting
- Fully connected layers for classification

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/KaranJaiswal02/Facial-Emotion-Recognition.git
   cd Facial-Emotion-Recognition
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset and place it in the `data/` directory.

4. Run the training script:
   ```bash
   python train.py
   ```

## Usage

To use the system for real-time emotion detection:

1. Ensure your webcam is connected.
2. Run the script:
   ```bash
   python detect.py
   ```
3. The interface will display the detected emotion on the screen.

## Results

The model successfully detects all 7 emotions demonstrates robust performance in real-world scenarios.


