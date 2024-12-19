
# Credit Card Fraud Detection Using Logistic Regression

## Overview
This project aims to detect fraudulent credit card transactions using a Logistic Regression model. The dataset is highly imbalanced, with most transactions being legitimate. To address this, undersampling was performed, and a robust classification model was built to identify fraudulent activities accurately.

---

## Dataset
The dataset used, `creditcard.csv`, consists of credit card transactions made in September 2013. Key features include:

- Time: Seconds elapsed between each transaction and the first transaction in the dataset.
- V1 to V28: Principal Component Analysis (PCA) transformed features (non-interpretable individually).
- Amount: The transaction amount.
- Class: Binary label indicating the transaction type:
  - `0`: Legitimate
  - `1`: Fraudulent
    

## Project Workflow

1. Data Loading & Exploration
- Load and inspect the dataset structure.
- Identify missing values and review basic statistics.
- Analyze the class distribution (legitimate vs fraudulent transactions).

2. Under-Sampling
- The dataset is highly imbalanced, with legitimate transactions far outnumbering fraudulent ones.
- A subset of legitimate transactions is sampled to balance the class distribution.

3. Data Preprocessing
- Split the dataset into features (`X`) and the target variable (`Y`).
- Divide the data into training and testing sets using an 80-20 split, ensuring class balance via stratified sampling.

4. Model Training
- Train a Logistic Regression model on the balanced training dataset.

5. Model Evaluation
- Evaluate model performance on both training and testing datasets using accuracy scores and other metrics.


## Dependencies
Ensure the following Python libraries are installed:
- `numpy`
- `pandas`
- `scikit-learn`

## Results
The Logistic Regression model achieved 92.89% accuracy on the test data, demonstrating its effectiveness in identifying fraudulent transactions despite the dataset's initial imbalance.

