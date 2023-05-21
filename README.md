# Determining-Diabetes-Using-PPG

This project focuses on determining whether a person is diabetic or not based on Photoplethysmography (PPG) signals. PPG signals provide valuable information about the cardiovascular system, and by analyzing specific features extracted from these signals, we can make predictions about a person's diabetic condition.

## Features Extraction

The following features are extracted from the PPG signals to aid in the prediction:

- **Systolic Peak**: The highest point on the PPG waveform corresponding to the systolic phase of the cardiac cycle.
- **Augmented Index**: The ratio of the systolic peak amplitude to the diastolic peak amplitude. It provides insights into arterial stiffness.
- **Adjusted Augmented Index** = 1 - Augmented Index
- **E/A Ratio**: The ratio of the amplitude of the early systolic wave (E wave) to the amplitude of the atrial contraction wave (A wave). It indicates cardiac function.
- **Pulse Interval to Systolic Peak Ratio**: The ratio of the pulse interval (time between two consecutive heartbeats) to the systolic peak amplitude. It captures the temporal relationship between heartbeats.

## Filtering Techniques

To improve the quality and extract relevant information from the PPG signals, the following filtering techniques are employed:

- **5th Order Butterworth Filter**: A band-pass filter is applied to remove artifacts from the PPG signals. The Butterworth filter provides a smooth response while preserving the signal's integrity.
- **2nd Order Derivative Filter**: A derivative filter is used to enhance the sharpness of the PPG waveform, emphasizing its crucial features such as the systolic peak.

## Machine Learning Model

Multiple machine learning models were employed to predict the diabetic condition based on the extracted features from PPG signals. The models used include Linear Discriminant Analysis (LDA), Logistic Regression, Decision Tree, and Support Vector Machines (SVM). Each model offers its unique advantages and characteristics, allowing for a comprehensive evaluation of the predictive performance. Once trained, the model can predict the likelihood of a person being diabetic based on their PPG signal.

## Dataset & Reference

https://figshare.com/articles/dataset/PPG-BP_Database_zip/5459299?file=37560727

## Acknowledgments

We would like to thank the researchers and contributors in the field of PPG signal analysis and diabetic prediction for their valuable work and open datasets that have facilitated this project's development.
