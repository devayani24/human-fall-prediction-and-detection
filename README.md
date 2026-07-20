# Human Fall Prediction & Detection

A 2D CNN-based classification model that predicts falls in elderly and bed-ridden patients from time-series sensor data, aimed at alerting caretakers in real time and reducing fall-related injury risk.

## Overview

Falls in elderly and bed-ridden patients are a major preventable health risk. This project builds a machine learning model that detects and predicts fall events from sensor data, with the goal of triggering real-time caretaker alerts.

## Approach

**Data preparation**
- Balanced the dataset across fall/non-fall labels to prevent the model from overfitting toward the majority class.
- Standardised all features to ensure internal consistency and comparability across the dataset.
- Reshaped input into time-series frames (minimum 0.4s windows) to capture the temporal pattern of a fall event.
- Split data 80/20 for training and testing.

**Model architecture — 2D CNN**
- Layers: Conv2D, Fully Connected
- Activation: ReLU, Softmax
- Optimiser: Adam
- Loss function: Sparse categorical crossentropy
- Dropout layer included to reduce overfitting

## Results

Trained over 20 epochs, with performance tracked via accuracy/loss learning curves and evaluated using a confusion matrix.

![Frame preparation](https://user-images.githubusercontent.com/76246283/119127787-5de05680-ba52-11eb-949c-a93a79cab995.png)
![Model architecture](https://user-images.githubusercontent.com/76246283/119127824-6a64af00-ba52-11eb-97e5-b11616467d06.png)
![Accuracy curve](https://user-images.githubusercontent.com/76246283/119127717-486b2c80-ba52-11eb-8fcc-d01cb7c0af4d.png)
![Loss curve](https://user-images.githubusercontent.com/76246283/119127731-4dc87700-ba52-11eb-948b-260b1208c489.png)
![Confusion matrix](https://user-images.githubusercontent.com/76246283/119127665-38ebe380-ba52-11eb-9497-1e596318d85e.png)

## Tech Stack

Python, TensorFlow/Keras, pandas, NumPy, scikit-learn (StandardScaler, LabelEncoder)
