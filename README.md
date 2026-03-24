# Bank Customer Churn Prediction

Predicting which bank customers are likely to churn using 
machine learning classification models.

## Dataset
- Source: Kaggle - Bank Customer Churn Prediction Dataset
- 10,000 customers, 14 features

## Workflow
1. Exploratory Data Analysis (EDA)
2. Preprocessing (encoding, feature engineering, scaling)
3. Model Training: Logistic Regression, Random Forest, XGBoost
4. Evaluation: ROC-AUC, Recall, F1, Confusion Matrix
5. Hyperparameter Tuning via GridSearchCV
6. Model Interpretation via SHAP

## Results
| Model | ROC-AUC | Recall | F1 |
|-------|---------|--------|----|
| Logistic Regression | 0.7818 | 0.7125 | 0.5013 |
| Random Forest | 0.8677 | 0.6743 | 0.6317 |
| XGBoost | 0.8736 | 0.5038 | 0.6027 |

XGBoost achieved the best ROC-AUC (0.8736). Random Forest 
is preferred if maximizing Recall is the priority.

## Key Findings
- Age, NumOfProducts, and IsActiveMember are the strongest 
  predictors of churn
- Older, inactive customers with multiple products carry 
  the highest churn risk
