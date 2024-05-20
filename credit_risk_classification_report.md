# Module 12 Report

## Overview of the Analysis

The purpose of this analysis is to build and evaluate machine learning models to predict credit risk based on financial information. The dataset contains financial attributes of borrowers, such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The goal is to predict the likelihood of a loan default, indicated by the loan_status column where 0 represents a healthy loan and 1 represents a high-risk loan.

The target variable, `loan_status`, has the following distribution:

- Healthy loans (`0`): 75,036 instances
- High-risk loans (`1`): 2,500 instances

The machine learning process involved several stages:

    Data preprocessing: 
    Reading the dataset, separating features and labels, and splitting the data into training and testing sets

    Model training: 
    Fitting logistic regression models to the training data

    Model evaluation: 
    Generating confusion matrices and classification reports to assess model performance

The primary method used in this analysis was logistic regression, a binary classification algorithm commonly used for predicting categorical outcomes.

## Results

Machine Learning Model 1: Logistic Regression

- Accuracy:
 
      99%

- Precision:
    
      Class 0 (Healthy Loan): 100%
      Class 1 (High-Risk Loan): 85%

- Recall:

      Class 0 (Healthy Loan): 99%
      Class 1 (High-Risk Loan): 91%

- F1-Score:

      Class 0 (Healthy Loan): 100%
      Class 1 (High-Risk Loan): 88%

- Support:

      Class 0 (Healthy Loan): 18,765
      Class 1 (High-Risk Loan): 619

- Macro Average:

      Precision: 92%
      Recall: 95%
      F1-Score: 94%

- Weighted Average:

      Precision: 99%
      Recall: 99%
      F1-Score: 99%

## Summary

The logistic regression model demonstrates high accuracy (0.99) in predicting loan statuses. The model achieves perfect precision (1.00) for predicting healthy loans (Class 0), indicating that all loans predicted as healthy are indeed healthy. The recall for healthy loans is also very high at 0.99, meaning the model correctly identifies 99% of healthy loans.

For high-risk loans (Class 1), the precision is 85%, suggesting that 85% of the loans predicted as high-risk are correctly identified. The recall for high-risk loans is 91%, indicating that the model correctly identifies 91% of high-risk loans.

Further analysis is needed to determine its suitability for practical use. Performance may vary depending on the problem being addressed; for example, it may be more critical to accurately predict high-risk loans to mitigate potential losses for the lending institution.

### Recommendation: 

The logistic regression model shows promise for predicting credit risk, but its performance should be validated further with additional data to address class imbalance and possibly compared with alternative models, such as decision trees or random forests. Additionally, ongoing monitoring and fine-tuning of the model may be necessary to ensure the model's practicability.

**Addressing Class Imbalance:**

There are 18,765 instances in the dataset where the loan status is 0 (healthy loan), and 619 instances in the dataset where the loan status is 1 (high-risk loan). This imbalance can affect the model's performance, particularly in accurately identifying high-risk loans.

Utilizing techniques such as the RandomOverSampler to address class imbalance can potentially improve the model's ability to detect and classify high-risk loans more accurately. By increasing the number of instances of the high-risk loan class, the model can be trained on a more balanced dataset, which may enhance its overall effectiveness. However, it is important to carefully consider the overall data quality, class balance, and evaluation metrics to ensure that any adjustments made lead to genuine improvements in model performance.

This approach should be part of a broader strategy of continuous refinement to maintain the model's effectiveness in real-world application.
