# Credit Risk Assessment
This project aims to build a model that assesses the risk involved in lending a loan to individuals, based on various financial and demographic features. The model is trained on data that includes details such as the individual's savings and checking account balances, loan duration, and income level, among other attributes.

# Table of Contents
1. Project Overview
2. Libraries and Dependencies
3. Data Preprocessing
4. Model Architecture
5. Results and Observations
6. Future Improvements

# Project Overview
The goal of this project is to create a model to predict credit risk, assessing whether an individual presents a "good" or "bad" credit risk for loan approval. The dataset is imbalanced, with 700 records of "good credit" and 300 records of "bad credit," reflecting the associated risk levels.<b/>

# Libraries and Dependencies
The following libraries were used:

 * NumPy and Pandas: For data manipulation and preprocessing.
 * Scikit-Learn (sklearn) and Imbalanced-Learn (imblearn): For model building, preprocessing, and handling class imbalance with SMOTE.
 * TensorFlow: For building and training the deep learning model.

# Data Preprocessing
 * Exploratory Data Analysis (EDA): Performed to understand feature distributions and relationships.
 * Handling Imbalance: Used Synthetic Minority Oversampling Technique (SMOTE) to synthetically create samples for the minority class, balancing the dataset to a total of 1400 data points.
 * Scaling and Encoding: Applied feature scaling and encoded categorical variables to prepare the data for training.
 * Data Splitting: Divided the dataset into training, validation, and test sets.

# Model Architecture
The model consists of a deep learning architecture with stacked LSTM layers, followed by dense layers for classification. A learning rate of 0.01 was selected, which provided the most favorable results during initial testing.

Key Parameters:
 * Learning Rate: 0.01
 * Architecture: Stacked LSTM layers with additional dense layers for prediction

# Results and Observations
While the model achieved satisfactory accuracy on the training set, the performance on validation and test sets was poor. This suggests overfitting, where the model performs well on training data but fails to generalize to unseen data.

Evaluation Summary:
 * Training Accuracy: High
 * Validation and Test Accuracy: Low, indicating overfitting


# Future Improvements
To enhance the model's performance and reduce overfitting:

 * Increase Data Points: Expanding the dataset may improve generalization, even with SMOTE applied.
 * Add Feature Variety: Introduce new features to capture additional dimensions of credit risk.
 * Experiment with Other Models: Test various machine learning and other deep learning models to find one better suited to this problem.
