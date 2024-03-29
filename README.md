# credit-risk-classification
Supervised Learning


## Overview of the Analysis
The purpose of this analysis is to evaluate the performance of machine learning models applied to a loan dataset. The aim is to predict whether a loan will be healthy (0) or high-risk (1) based on available financial information. The analysis involves exploring the dataset, preprocessing the data, training machine learning models, and evaluating their performance.

### Variables to predict
- loan_status: This variable represents the status of the loan, with 0 indicating a healthy loan and 1 indicating a high-risk loan.
- Other features: These are the independent variables used to predict the loan status, including attributes like credit score, income, loan amount, debt-to-income ratio, and employment status.

### Machine Learning Process
Data Preprocessing: The dataset was loaded into a Pandas DataFrame, and the features and labels were separated. 

Model Training: A logistic regression model was instantiated and trained using the training data. 

Model Evaluation: The trained model's performance was evaluated using the testing data. This evaluation involved generating a confusion matrix and printing a classification report to assess the model's accuracy, precision, recall, and F1-score for both healthy and high-risk loans.

### Method used
Logistic Regression: Logistic regression was employed as the primary machine learning algorithm for this analysis. It is a popular choice for binary classification tasks and is well-suited for interpreting the relationship between the independent variables and the probability of a particular outcome.

## Results
Logistic Regression Model:
- Accuracy: 0.99
- Precision (0 - healthy loan): 1.00
- Precision (1 - high-risk loan): 0.85
- Recall (0 - healthy loan): 0.99
- Recall (1 - high-risk loan): 0.91

## Summary
The logistic regression model outperforms with an accuracy of 0.99, indicating that it correctly predicts loan statuses for 99% of the cases in the dataset. In terms of precision, the model achieves a perfect score (1.00) for predicting healthy loans (0), meaning that all instances classified as healthy loans are indeed healthy. For high-risk loans (1), the precision score is slightly lower at 0.85, implying that 85% of the loans predicted as high-risk are truly high-risk. The recall scores indicate that the model captures 99% of actual healthy loans and 91% of actual high-risk loans.

Considering the task of predicting loan statuses, both precision and recall are crucial metrics. In this context, correctly identifying high-risk loans (1) is particularly important to mitigate potential financial losses. While the model's precision for high-risk loans is slightly lower than for healthy loans, its high recall ensures that a significant portion of actual high-risk loans is captured.

Therefore, based on its strong performance across accuracy, precision, and recall metrics, the logistic regression model is recommended for use in predicting loan statuses. However, it's essential to continually monitor and refine the model's performance, particularly in identifying high-risk loans, to ensure its effectiveness in real-world scenarios.