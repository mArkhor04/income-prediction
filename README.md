# Adult Census Income Prediction

## Overview
This project predicts whether an individual earns more than $50K per year using demographic and work-related features from the UCI Adult Census dataset. The goal is to apply machine learning to tabular, real-world data, extract insights, and identify the most influential factors impacting income.

## Dataset
- Source: [UCI Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
- Records: 48,842
- Features: 14 (numerical & categorical)
- Target: `income` (0 = <=50K, 1 = >50K)

## Approach
1. Data Cleaning:
   - Replaced missing values (`?`)
   - Removed duplicates
   - Encoded target variable
2. Feature Engineering:
   - One-hot encoding for categorical variables
   - Scaling for numerical features
3. Handling Class Imbalance:
   - SMOTE for Random Forest and XGBoost
   - Class weights for Logistic Regression
4. Model Training:
   - Logistic Regression
   - Random Forest
   - XGBoost
5. Evaluation:
   - Accuracy, F1-Score, ROC-AUC
   - Confusion matrix and ROC curve visualizations
6. Feature Importance:
   - Top features identified from tree-based models

## Results
- **Best Model:** XGBoost (SMOTE)
- Achieved high ROC-AUC and F1-Score
- Key features influencing income:
  - Capital-gain
  - Age
  - Hours-per-week
  - Education
  - Occupation

## Business Insights
- Older individuals working longer hours are more likely to earn >50K
- Higher education levels strongly correlate with higher income
- Capital gains significantly increase the probability of high income
- This insight can guide socio-economic policy, taxation analysis, and targeted marketing campaigns

## Tools & Technologies
- Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Imbalanced-learn
- Google Colab for experimentation

## Repository Structure
