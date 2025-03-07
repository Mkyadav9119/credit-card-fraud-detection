# Fraud Detection in Credit Card Transactions

## Objective

This project focuses on predicting fraudulent credit card transactions using machine learning techniques. The goal is to analyze customer transaction data, collected as part of a research collaboration between Worldline and the Machine Learning Group, to identify fraudulent activity.

The dataset, sourced from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud), consists of 284,807 transactions, of which only 492 are fraudulent. Given the highly imbalanced nature of the data, pre-processing steps are essential before building predictive models.

## Importance of Fraud Detection

With the growing use of digital payment systems, fraud detection has become a critical challenge for financial institutions. Unauthorized transactions cause significant financial losses and erode customer trust. Fraudulent activities lead to increased operational costs for businesses and potential identity theft for individuals. 

According to the [Nilson Report](https://nilsonreport.com/upload/content_promo/The_Nilson_Report_Issue_1164.pdf), global losses due to credit card fraud were projected to reach $30 billion by 2020. Detecting fraud in real-time can significantly mitigate financial risks for businesses and consumers alike.

## Understanding Credit Card Fraud

Fraudulent activities in credit card transactions involve unauthorized access to cardholder information for financial gain. Some common fraudulent practices include:

- **Card skimming** – Copying data from a card's magnetic strip
- **Creating counterfeit cards** – Altering legitimate card information
- **Lost or stolen card misuse** – Unauthorized transactions using misplaced or stolen cards
- **Online fraud** – Phishing scams and identity theft for unauthorized online purchases

## Dataset Overview

The dataset used for this analysis contains transaction records of European cardholders over two days in September 2013. The data has been anonymized using Principal Component Analysis (PCA) to protect confidentiality. The key attributes include:

- **Time** – Seconds elapsed since the first transaction
- **Amount** – Value of the transaction
- **Class** – Label indicating fraud (1) or legitimate transaction (0)
- **V1-V28** – Principal components derived from PCA

The dataset is highly skewed, with fraud accounting for only 0.172% of all transactions. To ensure balanced learning, appropriate resampling techniques will be applied.

## Project Workflow

### 1. Data Exploration
- Load the dataset and examine its structure
- Identify missing values and check data distribution
- Perform exploratory analysis to detect patterns in fraudulent transactions

### 2. Data Preprocessing
- Handle class imbalance using oversampling or undersampling techniques
- Apply feature selection methods to retain important predictors
- Scale and normalize numerical variables to ensure model stability

### 3. Model Training and Evaluation
- Implement machine learning algorithms such as Logistic Regression, Decision Trees, Random Forest, and Neural Networks
- Use k-fold cross-validation to ensure reliable model performance
- Optimize hyperparameters to enhance predictive accuracy

### 4. Performance Metrics
Since fraud detection requires a focus on correctly identifying fraudulent transactions, evaluation metrics include:

- **Precision & Recall** – To balance false positives and false negatives
- **F1-score** – A harmonic mean of precision and recall
- **ROC-AUC Score** – To measure model effectiveness in distinguishing fraud from non-fraud

By leveraging advanced machine learning techniques, this project aims to improve the accuracy and efficiency of fraud detection in credit card transactions.

