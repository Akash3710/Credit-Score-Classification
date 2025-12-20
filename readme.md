Credit Score Classification

This project aims to classify individuals into credit score categories (Good, Standard, Poor) using financial and demographic attributes. The goal is to predict a person’s creditworthiness through effective data preprocessing, feature extraction, encoding, and machine learning models.

Project Workflow
1. Data Cleaning & Preprocessing

Handled missing values using mean/median imputation for numerical features and mode imputation for categorical features.

Detected and treated outliers in key variables such as Annual Income, Outstanding Debt, and Monthly Balance.

Converted date-related columns into usable formats where applicable.

2. Exploratory Data Analysis (EDA)

Analyzed distributions of important numerical features including Annual Income, Outstanding Debt, and Monthly Balance.

Used a correlation heatmap to examine relationships between variables.

Visualized categorical features such as Occupation, Credit Mix, and Payment Behaviour.

Insight: Higher income levels and balanced debt ratios are strongly associated with Good credit scores.

3. Feature Extraction

Categorical Encoding

Applied Label Encoding for ordinal features like Credit_Mix.

Used One-Hot Encoding for nominal features such as Occupation and Payment_Behaviour.

Feature Scaling

Applied StandardScaler to numerical features (Annual_Income, Outstanding_Debt, Monthly_Balance) to maintain uniform scale.

Feature Engineering

Created derived features such as spending level and payment value from payment behaviour data.

Target Encoding

Converted Credit_Score into numeric classes:

Good → 2

Standard → 1

Poor → 0

4. Model Building & Training

Split the dataset into training and testing sets.

Trained multiple classification models:

Logistic Regression

Decision Tree

Random Forest

XGBoost

5. Model Evaluation

Evaluated models using F1-score.

Best Performing Model: XGBoost, due to its effectiveness in handling complex and imbalanced financial data.

Results

F1-score: 0.75
