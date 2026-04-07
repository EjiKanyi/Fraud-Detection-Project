# Fraud Detection Model

## Problem Statement
Financial fraud is a growing concern in mobile money platforms, where millions of transactions occur daily across various types including CASH-IN, CASH-OUT, DEBIT, PAYMENT, and TRANSFER. The objective of this project is to build a machine learning model that accurately detects fraudulent transactions while minimizing false alarms.

## Dataset
The dataset contains 6.3 million financial transaction records for fraud detection. Some records were flagged false by existing algorithms.

| Feature | Description |
|---------|-------------|
| type | Type of transaction (CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER) |
| amount | Amount of the transaction |
| nameOrig | Customer who started the transaction |
| oldbalanceOrg | Initial balance of sender before transaction |
| newbalanceOrig | New balance of sender after transaction |
| nameDest | Recipient of the transaction |
| oldbalanceDest | Initial balance of recipient before transaction |
| newbalanceDest | New balance of recipient after transaction |
| isFraud | Whether the transaction is fraudulent (1) or not (0) |

## Project Structure
1. Analysis_model.ipynb
2. fraud_detection.py
3. fraud_detection_pipeline.pkl
4. requirements.txt
5. README.md

## Project Workflow
1. Exploratory Data Analysis (EDA)
2. Feature Engineering
3. Model Building and Evaluation
4. Model Comparison
5. Deployment

## Models Used
| Model | Precision | Recall | F1-Score | AUC-ROC |
|-------|-----------|--------|----------|---------|
| Logistic Regression | 0.02 | 0.94 | 0.04 | 0.9888 |
| Random Forest | 0.96 | 0.78 | 0.86 | 0.9950 |
| XGBoost | 0.47 | 0.99 | 0.64 | 0.9993 |

Selected Model: Random Forest had the  best balance between precision and recall.

## How to Run the App
1. Clone the repository:
https://github.com/EjiKanyi/Fraud-Detection-Model.git

2. Install the required libraries:
pip install -r requirements.txt

3. Run the Streamlit app:
streamlit run fraud_detection.py

## Live Demo 

## Tools and Libraries
-> Python

-> Pandas

-> Scikit-learn

-> XGBoost

-> Streamlit

-> Matplotlib

-> Seaborn

-> Joblib