Credit Score Classification

This project aims to classify individuals into credit score categories (Good, Standard, Poor) based on their financial and demographic attributes. By applying data cleaning, feature extraction, encoding, and machine learning models, we can predict the creditworthiness of a person.

Project Workflow
1. Data Cleaning & Preprocessing

Handled missing values using mean/median  for numerical columns and mode for categorical columns.

Detected and treated outliers in income, debt, and balance columns.

Converted date columns into usable formats (if applicable).

2. Exploratory Data Analysis (EDA)

Distribution analysis of key features like Annual Income, Outstanding Debt, Monthly Balance.

Correlation heatmap to understand relationships between variables.

Plots for categorical features (Occupation, Credit Mix, Payment Behavior).

Insights: Higher income and balanced debt ratios are strongly linked with good credit scores.

3. Feature Extraction

Categorical Encoding:

Used Label Encoding for ordinal variables like Credit_Mix.

Used One-Hot Encoding for nominal variables like Occupation, Payment_Behaviour.

Feature Scaling: Applied StandardScaler on numerical features (e.g., Annual_Income, Outstanding_Debt, Monthly_Balance) to bring them to the same scale.

Feature Engineering: Created derived features such as spending level and payment value from payment behaviour

Target Encoding: Converted Credit_Score into numeric classes (Good → 2, Standard → 1, Poor → 0).

4. Model Building & Training

Split data into train-test sets.

Trained multiple classification models:

Logistic Regression

Decision Tree

Random Forest

XGBoost


5. Model Evaluation

Metrics used:  F1-score

Best performing model: XGBoost, due to its ability to handle imbalanced and complex financial data.

📈 Results

F1- score = 0.75
