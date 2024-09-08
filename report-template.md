# Module 12 Report Template

## Overview of the Analysis

various machine learning models were evaluared to predict loan status from the dataset. The primary goal was to assess the effectiveness of different models in classifying loans as either high-risk or healthy.

## Purpose of the Analysis
The purpose of this analysis was to determine which machine learning model best predicts the risk level of loans based on historical financial data. Several models learned in class were added to show and practice. Accurately predicting high-risk loans is crucial for managing financial risk and making informed lending decisions. Itwas a joyful experience.

## Data Description
The dataset provided included features related to loan details, with the loan_status column as the target variable:

**loan_status:** Indicates whether a loan is high-risk (1) or healthy (0).
We needed to predict this loan_status based on various features provided in the dataset.

## Variables and Predictions
**loan_status:** Binary variable where:
**0 represents** a healthy loan.
**1 represents** a high-risk loan.
The dataset had a relatively balanced distribution between healthy and high-risk loans.
## Stages of the Machine Learning Process
**Data Preparation:**

Loaded the dataset and separated it into features (X) and the target variable (y).
Split the data into training and testing sets using train_test_split.
**Model Training:**

Instantiated and trained several machine learning models on the training data. Models included:
Logistic Regression
Random Forest
AdaBoost
Extra Trees
Gradient Boosting
K-Neighbors
XGBoost
LightGBM

**Model Evaluation:**

Made predictions on the testing set.
Evaluated models using metrics such as accuracy, precision, recall, and F1-score.
Plotted confusion matrices to visualize the performance.

Methods Used (Retrieved from ChatGPT)

Logistic Regression: A basic algorithm for binary classification.
Random Forest: An ensemble method that combines multiple decision trees.
AdaBoost: An ensemble method that combines weak classifiers to improve performance.
Extra Trees: An ensemble method that uses randomly selected features for decision trees.
Gradient Boosting: An ensemble method that builds models sequentially to correct errors of previous models.
K-Neighbors: A non-parametric method that classifies based on proximity to neighbors.
XGBoost: An optimized gradient boosting algorithm that performs well on large datasets.
LightGBM: A gradient boosting framework that uses histogram-based methods for faster training.

Results on the first portion the homework **Logistic Regression** shows a very effective score, however on the second part were all data was used  **XGBoost** lead higher scores in accuracy (0.9952), Precision (0.8734), etc. However **Logistic Regression** rated no far behind but in 4th place for accuracy (0.9946) and  precision (0.8716) -- see graph on the bottom of the code page. 

## Summary

Best Performing Models:

**XGBoost:** This model achieved the highest F1-Score, demonstrating a good balance between precision and recall. It is the most effective at predicting high-risk loans while maintaining high accuracy.
**AdaBoost:** Close behind XGBoost, it also shows strong performance with high precision and recall.

Model Performance Dependence:

For financial risk prediction, it's crucial to have high recall for high-risk loans (to minimize missed predictions). XGBoost and AdaBoost are effective in this regard.
Precision is also important to avoid false positives (healthy loans misclassified as high-risk). XGBoost and AdaBoost provide a good balance here.
Recommendation:

**XGBoost is recommended due to its overall superior performance, particularly in terms of F1-Score, which indicates a good balance between precision and recall.
AdaBoost is also a strong contender and could be considered depending on specific needs or constraints.**

## References: 
**REFERENCES**
Alexander Booth class exercices. Bootcamp: DATA-PT-EAST-APRIL-041524-MTTH-CONSXpert

Bootcamp: DATA-PT-EAST-APRIL-041524-MTTH-CONSXpert Learning Assistant https://bootcampspot.instructure.com/courses/6446/external_tools/313#:~:text=Tutoring%20Sessions-,Xpert%20Learning%20Assistant,-Lucid 

ChatGPT, OpenAI. (2024). Assistance with machine learning model evaluation and analysis. Retrieved from ChatGPT. 
