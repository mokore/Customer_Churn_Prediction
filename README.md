# ConnectTel Customer_Churn_Prediction
Data Analysis and Customer Churn Prediction carried out for a telecommunications company ConnectTel

![image](https://github.com/mokore/Customer_Churn_Prediction/assets/159819689/fdb044bf-87c5-4daf-97ce-6a30ce271888)


![image](https://github.com/mokore/Customer_Churn_Prediction/assets/159819689/ab34f6bb-3643-4771-adff-203be7dac2c9)

![image](https://github.com/mokore/Customer_Churn_Prediction/assets/159819689/3060f63a-4844-4b52-a7d9-ca4c73f22d4e)


## Overview
This is a machine learning project for a company in the telecommunications industry, ConnectTel. ConnectTel is a leading telecommunications company at the forefront of innovation and connectivity solutions, with a strong presence in the global market.

## Problem Statement
ConnectTel is faced with customer churn challenges which is a threat to its business sustainbility and growth. Current strategies to retain customer are not working as expected. They wish to overcome this challenge by implementing state of the art churn prediction system leveraging advanced analytics and machine learning techniques.

## Project Objective
The project objectives include unearthing insights from the data provided and develop the most effective machine learning model that accurately predicts customer churn. the aim is to enhance customer loyalty and maintain a competetive edge in the industry.

## Data Sources
ConnectTel customer data required to carry out analytics and predictions was provided by 10Alytics. It consists of 7043 rows and 21 columns. The dataset contains minimal customer features and the telecommunications services they have subscribed to. It also contains specific information on the customers’ loyalty status which confirms if they have churned or not.

# Data Preprocessing
The preprocessing phase involved an indept review of the data to observe its characteristics and confirm if it is in the appropriate form for machine learning application. Missing values were identified and updated, incorrect attribute type specification was also discovered and fixed. Univariate, bivariate and multivariate visualizations were applied which helped to reveal many important insights related to the dataset and uncover the correlations within amongst the attributes.

## Machine Learning Model
Given that the dataset has a label, the customer churn prediction project was treated as a classification problem. Hence, several classisfication algorithms were utilised to build models out of which the best performing model was to be selected as most suitable for the prediction task. The following classification algorithms were used in the model building phase:

- **Extreme Gradient Boost**
- **Random Forest**
- **K-Nearest Neighbors**
- **Support Vector Classification**
- **Stochastic Gradient Descent**
- **Logistic Regression**
- **Decision Tree**
- **Naives Bayes**
- **Linear Support Vector Classification**

## Evaluation Metrics
To assess the performance of the machine learning models, the following evaluation metrics were used:

- **Accuracy:** The overall proportion correctly classified customers (churned and not churned) when compared with the total customers in the test sample.
- **Precision:** The proportion of correctly identified churn customers when compared with the total count of customers classified as churned.
- **Recall:** The proportion of correctly identified churn customers among all the actual churned customers in the test sample.
- **F1 Score:** The harmonic mean of precision and recall, providing a balanced metric for model evaluation.
- **AUC-ROC:** Area under the ROC curve. It is used to evaluate the model's performance across different thresholds. 

## Key Insights
The Logistic Regression Classification model has the highest accuracy of 81.26%. This means that during the test cycle, it produced the highest number of correct predictions (TPs and TNs). From its confusion matrix, the TP is 330 and the TN is 1387 making a combined total of 1717 correct predictions out of 2113. Linear Support Vector classifier ranks second in accuracy with a score of 80.88% while SVC ranks third with a score of 80.41%.

In terms of precision score, SVC ranks first with a score of 69.05% closely followed by Linear SVC's 68.48% with Logistics Regression coming third at 68.46%. Precision is the ratio of the TP to the total positive predictions (TP + FP).

For the recall metric, Naives Bayes scored the most points with a score of 89.72% while SGD Classifier came in at a distant second with 66.72% and Logistic Regression ranked third with 57.49%. Recall is the ratio of the TP to the total actual positives in the test data (TP + FN).

## Conclusion
For this case under review, what is most important for the business will be the ability to correctly predict customers that will churn so that they can apply necessary intervention mechanisms to ensure they continue to retain the customer's patronage. This means the business is expected to be more concerned with the true positives (TP) metric more than any other. The higher the TPs, the higher the number of correctly predicted "churned customers".

Out of the nine models developed, the Naives Bayes model performed best in terms of true positive (TP) predictions where 515 correct churn predictions were made out of 574 churned customers in the test dataset (`89.72%`). Based on this, the Naives Bayes model will be the most suitable for the business to apply despite its lower accuracy score.
