# Module 12 Report Template

## Overview of the Analysis
#### Purpose of the Analysis
The purpose of this analysis was to develop machine learning models that can effectively predict credit risk. The goal was to leverage historical financial data to create models capable of classifying loans as either healthy (low-risk) or high-risk of defaulting. By accurately identifying high-risk loans, financial institutions can make informed lending decisions and manage credit risk effectively.

#### Financial Information and Prediction Variables

The dataset used in this analysis contained financial information related to loans. The variables included various features such as **loan size**, **interest rate**, **borrower's income**, **debt-to-income ratio**, loan status among others. The loan status column was the target variable, indicating whether a loan is healthy (0) or high-risk (1).

To predict credit risk, the machine learning models were trained to classify loans into these two categories based on the available financial information.

#### Methods Utilized

The primary machine learning method employed in this analysis was logistic regression. Logistic regression is a widely-used algorithm for binary classification tasks and was well-suited for predicting credit risk based on the available financial features.

Additionally, the RandomOverSampler resampling method was implemented to mitigate the class imbalance present in the dataset. This technique increased the representation of high-risk loans in the training set, enabling the model to learn from more balanced data and improve its predictive capabilities.

Overall, this analysis involved data preprocessing, model development using logistic regression, evaluation of model performance, and the utilization of resampling techniques to enhance prediction accuracy for credit risk classification.

## Results

**Machine Learning Model 1 (Original Data):**
1. Balanced Accuracy Score: 0.94
2. Precision Score: 0.87
3. Recall Score: 0.89
4. Machine Learning Model 2 (Resampled Data):
5. Balanced Accuracy Score: 0.99
6. Precision Score: 0.87
7. Recall Score: 0.99

## Summary

Based on the results, both Machine Learning Model 1 (trained on original data) and Machine Learning Model 2 (trained on resampled data) have similar precision and recall scores. However, there is a notable difference in the balanced accuracy score and the macro average f1-score.

Machine Learning Model 2 (Resampled Data) outperforms Model 1 (Original Data) in terms of balanced accuracy, with a score of 0.99 compared to 0.94. This indicates that Model 2 has a better overall accuracy in predicting both the healthy (0) and high-risk (1) loan labels.

Additionally, Model 2 shows a significantly higher recall score for the high-risk (1) loan label, with a value of 0.99 compared to 0.89 in Model 1. This means that Model 2 is more successful in identifying actual high-risk loans correctly, minimizing the risk of missing potentially problematic loans.

Considering the importance of correctly identifying high-risk loans to manage credit risk effectively, Model 2 (trained on resampled data) is recommended. It achieves a higher overall accuracy and demonstrates better performance in capturing high-risk loans. By using resampling techniques to address the class imbalance, Model 2 has improved its ability to predict high-risk loans accurately.

It is crucial to note that the choice of the model depends on the problem we are trying to solve. If the primary concern is to minimize false negatives and accurately identify high-risk loans, Model 2 is the preferred option. However, if avoiding false positives and being cautious in classifying loans as high-risk is more critical, the precision score of 0.87 in both models should be taken into consideration.

In summary, the recommendation is to use Machine Learning Model 2 (trained on resampled data) due to its higher balanced accuracy, improved recall for high-risk loans, and overall better performance in predicting credit risk.
