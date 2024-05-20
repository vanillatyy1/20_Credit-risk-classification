# 20_Credit Risk Classification

## 1) Executive Summary:

The credit risk classification project aimed at predicting the likelihood of loan defaults using machine learning models. We utilized logistic regression to analyze a dataset containing various financial attributes of borrowers. The model achieved good accuracy and provided valuable insights into the prediction of both healthy and high-risk loans. However, further validation and potential exploration of alternative models,especially for high-risk loans predictions, are recommended to ensure practical applicability.

**Links:**

[credit_risk_classification.ipynb](https://github.com/vanillatyy1/20_Credit-risk-classification/blob/2c6783aeefc3b996c985948dcdb4c8b1cf62477b/credit_risk_classification.ipynb)

[credit_risk_classification_report](https://github.com/vanillatyy1/20_Credit-risk-classification/blob/2c6783aeefc3b996c985948dcdb4c8b1cf62477b/credit_risk_classification_report.md)


## 2) Project Objectives:

**Predict Credit Risk:**

Develop a predictive model to classify loans as either healthy (low risk of default) or high-risk (high likelihood of default)

**Evaluate Model Performance:**

Assess the accuracy, precision, recall, and overall effectiveness of the model in predicting credit risk

**Provide Business Insights:**

Offer actionable recommendations based on the model’s performance to aid in credit risk management

## Resource Requirements

- Technologies: Jupyter Notebook, Python and relevant libraries Pandas, Numpy, Scikit-learn

## Results

```
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

```

## Takeaways

**Good Accuracy and Precision:** 

The logistic regression model achieved an accuracy of 99%, with perfect precision for healthy loans and good precision for high-risk loans. This indicates the model’s high reliability in correctly classifying loan statuses.

**Model Improvement:** 

Despite the model’s strong performance, further validation with additional data and exploration of other algorithms like decision trees or random forests could enhance robustness. Continuous monitoring and refinement are also recommended to maintain effectiveness in real-world applications.