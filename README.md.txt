# Credit Default Prediction & Alternative Credit Scoring

## Project Overview
This project builds a loan default prediction framework using LendingClub data. It compares a traditional Logistic Regression benchmark with machine learning models including Random Forest, Support Vector Machine, and XGBoost.

## Business Problem
Traditional credit scoring models may not fully capture non-linear borrower risk patterns or soft information from borrower narratives. This project explores whether machine learning and sentiment-based alternative data can improve credit risk prediction.

## Dataset
- Source: LendingClub loan data
- Target variable: default / non-default loan status
- Features: loan amount, term, interest rate, annual income, debt-to-income ratio, revolving utilization, credit inquiries, public records, and sentiment score
- Alternative data: sentiment score extracted from borrower loan narratives

## Methodology
- Data cleaning and preprocessing
- Default labelling
- Feature engineering
- Sentiment extraction using TextBlob
- Train-test split
- Class imbalance handling
- Model benchmarking

## Models
- Logistic Regression
- Random Forest
- Support Vector Machine
- XGBoost

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- AUC

## Key Findings
XGBoost showed the strongest overall credit risk detection performance based on AUC, Recall, and F1-score. Random Forest achieved high accuracy but lower recall, making it less suitable when the business objective is to detect actual default cases.

## Credit Risk Interpretation
For credit risk modelling, model selection should not rely only on accuracy. Recall, AUC, threshold selection, class imbalance treatment, explainability, and model monitoring are important for practical deployment.

## Notebook
The full analysis is available here: [Credit Default Prediction Notebook](notebooks/credit_default_prediction_alternative_scoring.ipynb)

## Portfolio PDF
A short portfolio summary is available here: [Credit Risk Modelling Portfolio](docs/Credit_Risk_Modelling_Portfolio_Tran_Thu_Thao_My.pdf)
