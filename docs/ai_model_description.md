AI Model Description – Wheat Quality Prediction
1. Overview

The AI model is designed to predict the quality of wheat stored inside the smart silo using environmental sensor data (temperature, humidity, CO₂ level).
The goal is to detect early signs of degradation or contamination and support automated decision-making inside the smart silo system.

2. Input Features

The model uses the following sensor measurements as input:

Temperature (°C)

Humidity (%)

CO₂ concentration (ppm)

These features are collected in real-time through the IoT system.

3. Machine Learning Approach

The model was developed using the following steps:

✔ Data Preprocessing

Cleaning missing values

Normalizing features

Balancing the dataset using SMOTE to handle class imbalance

✔ Model Architecture

A Deep Neural Network (DNN) was trained using TensorFlow.
The architecture includes:

Dense layers

ReLU activation functions

Softmax output for 3-class classification

✔ Training Settings

Optimizer: Adam

Loss: Categorical Crossentropy

Epochs: 50

Train/Test Split: 80/20

4. Output Classes

The model predicts the wheat quality as one of:

Class 0: Low-quality or potentially contaminated grain

Class 1: Medium-quality / acceptable

Class 2: High-quality grain

5. Model Evaluation
✔ Confusion Matrix

✔ Interpretation

The model achieved:

79 correct predictions for Class 0

95 correct predictions for Class 1

98 correct predictions for Class 2

Only a small number of samples were misclassified, showing a strong ability to generalize and high robustness.

6. Accuracy & Performance

Overall Accuracy: ~95%

Precision / Recall: High for all three classes

The model is stable and performs well on unseen data.

7. Integration in Smart Silo System

The trained model is exported as a .h5 file and is used inside FastAPI to:

Predict grain quality in real time

Generate weekly AI-based reports

Trigger alarms when poor-quality patterns are detected

This enables the smart silo system to combine IoT + AI into a fully automated solution.
