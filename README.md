# Bank Campaign Optimization: Targeting Term Deposit Customers

## Overview

This data science project, titled "Bank Campaign Optimization: Targeting Term Deposit Customers," aims to optimize marketing campaigns for a bank by leveraging extensive exploratory data analysis (EDA), statistical tests, predictive modeling, and threshold moving. The project focuses on understanding customer behavior, optimizing communication strategies, and building a predictive model to identify potential term deposit subscribers.

## Project Structure

### 1. Exploratory Data Analysis (EDA)

#### A. Customer Segmentation:
By clustering customers based on their characteristics and behavior, such as age, profession, education, marital status, and loan status, the project aims to identify distinct customer segments. This segmentation allows the bank to tailor marketing campaigns and strategies to specific customer groups.

#### B. Campaign Optimization:
Analyzing the effectiveness of communication types, the number of contacts performed, the duration of contact, and outcomes of previous campaigns provides insights into successful strategies. This information aids in optimizing future campaign efforts for better results.

### 2. Statistical Tests

#### A. t-test with Cohen's d:
Conducting a t-test helps determine if there's a significant difference between means for customers with and without term deposit subscriptions. Cohen's d provides a standardized measure of effect size, quantifying the practical significance of observed differences.

#### B. Chi-square with Cramer's V:
Chi-square tests and Cramer's V assess the association between categorical variables. Cramer's V quantifies the strength of the association, aiding in the comparison of associations across different tables.

### 3. Predictive Modeling

Building a predictive model involves analyzing features like age, job, marital status, education, balance, and previous campaign outcomes. The model aims to predict whether a customer will subscribe to a term deposit. The machine learning pipeline, column transformers, and grid search with cross-validation ensure an efficient and robust modeling process.

### 4. Model Evaluation

The F1-score is chosen as the evaluation metric for the predictive model, aiming for a balanced model with minimized false negatives and false positives. RandomForestClassifier is identified as the best model with tuned hyperparameters achieving 90% accuracy, F1-score of 0.61, and ROC-AUC score of 0.93 on the test data.

### 5. Threshold Moving

Given the imbalanced nature of the classification problem, threshold moving is conducted to improve classifier performance. The Precision-Recall curve is selected over the ROC-AUC curve due to the project's goal of minimizing false positives and false negatives independently. The optimal threshold of 0.58 is determined from the Precision-Recall curve of the training data. Applying this threshold to test data probabilities results in 91% accuracy, F1-score of 0.55, and ROC-AUC score of 0.93.

## Conclusion

This project provides a comprehensive approach to bank campaign optimization, incorporating customer segmentation, campaign optimization, statistical tests, predictive modeling, and threshold moving. The balanced model, with a focus on minimizing false negatives, is achieved through meticulous analysis and evaluation techniques. The detailed README.md file serves as a guide for understanding the project's processes and outcomes.
