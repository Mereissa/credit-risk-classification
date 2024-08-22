# Credit Risk Analysis

## Overview

This analysis involves developing a logistic regression model to predict the risk of default for loans based on historical lending data. The primary goal is to accurately classify loans into two categories: healthy (0) and high-risk (1). The model's performance is evaluated using a classification report and a confusion matrix.

## Results

The logistic regression model was evaluated on the test dataset, and the following performance metrics were obtained:

- **Confusion Matrix:**
[[18663 102]
[ 56 563]]

- **Classification Report:**
            precision    recall  f1-score   support

         0       1.00      0.99      1.00     18765
         1       0.85      0.91      0.88       619

  accuracy                           0.99     19384
 macro avg       0.92      0.95      0.94     19384
weighted avg     0.99      0.99      0.99     19384


### Key Metrics

- **Healthy Loans (`0`):**
- **Precision:** 1.00
- **Recall:** 0.99
- **F1-Score:** 1.00

- **High-Risk Loans (`1`):**
- **Precision:** 0.85
- **Recall:** 0.91
- **F1-Score:** 0.88

- **Overall Performance:**
- **Accuracy:** 0.99
- **Macro Average Precision:** 0.92
- **Macro Average Recall:** 0.95
- **Macro Average F1-Score:** 0.94
- **Weighted Average Precision:** 0.99
- **Weighted Average Recall:** 0.99
- **Weighted Average F1-Score:** 0.99

## Summary

The logistic regression model demonstrates excellent performance in predicting healthy loans, with perfect precision and high recall. For high-risk loans, the model also shows strong performance with good precision and recall. The overall accuracy of 99% underscores the model's effectiveness at classifying both healthy and high-risk loans.

Given the high performance metrics and accuracy, the model is recommended for use in identifying loan risks. Its robust ability to differentiate between healthy and high-risk loans makes it a valuable tool for credit risk analysis.

## Instructions

1. **Read the Data:** The dataset (`lending_data.csv`) was read into a Pandas DataFrame.
2. **Prepare the Data:** Labels were extracted from the `loan_status` column, and features were prepared from the remaining columns.
3. **Split the Data:** The data was divided into training and testing sets.
4. **Train the Model:** A logistic regression model was fitted using the training data.
5. **Evaluate the Model:** Predictions were made on the test data, and the performance was assessed using a confusion matrix and classification report.

For more details or to run the analysis, refer to the provided Jupyter notebook.
