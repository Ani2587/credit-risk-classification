# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis is to address the issue of class imbalance within the lending dataset and evaluate the performance of a logistic regression model in predicting loan statuses (healthy or high-risk) after resampling the data. Class imbalance refers to situations where one class is significantly more prevalent than another within the dataset.

By examining metrics such as accuracy, precision, and recall, we aim to understand how effectively the model predicts loan statuses and provides insights for decision-making within the company's lending practices. The analysis helps determine the model's reliability and suitability for real-world application, ultimately informing recommendations regarding its integration into the company's lending operations.

#### the distribution of loan statuses
print(df_lending_data["loan_status"].value_counts())
loan_status
0    75036
1     2500


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

### Machine Learning Model 1:
Description of Model 1 Accuracy, Precision, and Recall scores.
Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384


Model Performance Metrics:

Accuracy: Overall accuracy of the model on the test set is approximately 99%.
Precision: Precision for healthy loans (label 0) is 1.00, indicating a low false positive rate.
Precision for high-risk loans (label 1) is 0.87, suggesting that out of the predicted high-risk loans, 87% are actually high-risk.
Recall: Recall for healthy loans (label 0) is 1.00, indicating a low false negative rate.
Recall for high-risk loans (label 1) is 0.89, suggesting that the model correctly identifies 89% of the actual high-risk loans.

### Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
Overview of Analysis Purpose:

The purpose of this analysis is to assess the performance of a logistic regression model trained on oversampled data to predict loan statuses (healthy or high-risk).

Model Performance Metrics:

Accuracy: Overall accuracy of the model on the test set is approximately 100%.
Precision:
Precision for healthy loans (label 0) is 1.00, indicating a low false positive rate.
Precision for high-risk loans (label 1) is .87, indicating a low false positive rate.

Recall:Recall for healthy loans (label 0) is 1.00, indicating a low false negative rate.
Recall for high-risk loans (label 1) is 1.00, suggesting that the model correctly identifies 89% of the actual high-risk loans.


## Summary

The logistic regression model, trained with oversampled data, does a great job at predicting both healthy loans (label 0) and high-risk loans (label 1). It hardly ever makes mistakes when identifying healthy loans. The accuracy for this model is 1.00
