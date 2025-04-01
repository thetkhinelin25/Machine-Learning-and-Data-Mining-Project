# Human Activity Recognition Using Machine Learning

## About the Project

This project focuses on **Human Activity Recognition (HAR)** using data collected from motion sensors. The raw signal data, gathered from personal digital devices, is used to classify physical activities such as **Walking**, **Jogging**, **Sitting**, **Standing**, **Upstairs**, and **Downstairs**. The goal is to develop and evaluate machine learning models capable of accurately identifying these activities and generalizing well to unseen data.

---

## Project Goal

The main objective is to build a reliable and generalizable machine learning pipeline that can:
- Transform noisy time-series sensor data into informative features.
- Classify physical activities effectively.
- Perform well on both internal test data and external evaluation (Kaggle dataset).

---

## Methodology

The project workflow includes:
- **Exploratory Data Analysis (EDA):** Understand data distribution, feature significance, and multicollinearity.
- **Feature Engineering:** Extract statistical, temporal, and frequency-based features from raw signal data.
- **Data Preprocessing:** Normalize features, encode labels, and balance the dataset.
- **Model Development:** Train and tune multiple models using optimized pipelines.
- **Iterative Improvement:** Loop back to feature selection or preprocessing based on evaluation results.

---

## Models Used

The following models were developed and evaluated:
- **Gradient Boosting Machine (GBM)**
- **Random Forest Classifier (RF)**
- **K-Nearest Neighbors (KNN)**
- **Artificial Neural Network (ANN)**
  - *Generalized ANN (with EarlyStopping)*
  - *Kaggle-Optimized ANN (without EarlyStopping)*

---

## Model Evaluation

Model performance was assessed using:
- **Standard Accuracy** on the test dataset.
- **Balanced Accuracy** to account for class imbalance.
- **Kaggle Leaderboard Accuracy** (using a 48% version of the dataset).

---

## Results

- **Best Overall Model:** ANN with EarlyStopping  
  - **Test Accuracy:** 85.32%  
  - **Balanced Accuracy:** 80.76%  
  - **Kaggle Accuracy:** 90.83%

- A second ANN model (without EarlyStopping) achieved **92.81%** on Kaggle but dropped to **82.52% test accuracy** and **75.5% balanced accuracy**, indicating overfitting.

- **GBM** had the highest test accuracy (**86.45%**) but showed lower balanced accuracy (**78.32%**), suggesting bias toward dominant classes.

---

Feel free to explore the code, notebooks, and results provided in this repository to understand the full development lifecycle of a HAR system using machine learning.
