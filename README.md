# Loan-Prediction-Model

Overview:
This repository contains my project for the Kaggle Playground Series S5E11 (2025). The goal of this competition is to predict the probability that a borrower will pay back their loan using a synthetic tabular dataset inspired by real-world financial data. The project demonstrates an end-to-end machine learning workflow, including data preprocessing, feature engineering, model training, blending, and submission generation.

Objective:
Build a model that predicts:

“loan_paid_back probability (0 = not paid, 1 = paid)”

The evaluation metric is ROC-AUC, which measures the ranking performance of predicted probabilities.

Dataset:
The dataset is synthetically generated but closely mimics real-world loan data.
It contains:
•	Borrower financial profiles
•	Loan details and terms
•	Credit risk indicators
•	Behavioral features

Files included in this repository:
•	train.csv — Training data with labels
•	test.csv — Test data without labels
•	submission_blend.csv — Kaggle-ready submission file

Technology Stack:
•	Python
•	Pandas / NumPy
•	Scikit-Learn
•	LightGBM / CatBoost
•	Matplotlib / Seaborn
•	Kaggle Notebook

Project Workflow:
1. Data Exploration & Cleaning
•	Handling missing values
•	Encoding categorical variables
•	Outlier detection

2. Feature Engineering
•	Target encoding for categorical features
•	Feature scaling
•	Combining numeric and categorical features

3. Model Training
•	LightGBM (baseline and with TE features)
•	CatBoost (with TE features)
•	K-Fold cross-validation

4. Model Blending
•	Weighted blend of LightGBM + CatBoost predictions for better ROC-AUC

5. Submission Generation
•	Export final predictions as submission_blend.csv

Results
Model	OOF ROC-AUC
LightGBM + TE	X.XXX
CatBoost	X.XXX
Blended Model	X.XXX


Repository Structure
|-- data/
|    |-- train.csv
|    |-- test.csv
|-- notebook.ipynb
|-- submission_blend.csv
|-- README.md

Submission:
The final submission file is ready for Kaggle leaderboard: “submission_blend.csv”

References
“Kaggle Playground Series S5E11"


