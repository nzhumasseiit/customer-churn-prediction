# customer-churn-prediction

# Overview
I built a machine learning pipeline to predict customer churn for a telecom company using the Kaggle Telco Customer Churn dataset. The goal was to identify customers likely to leave, helping businesses improve retention of customers. This project showcases my skills in Python, data preprocessing, and machine learning. I included a custom feature and analysis to uncover churn drivers!

# Main Tools
1. Python: pandas, scikit-learn, xgboost, seaborn
2. SQL: pandasql for querying
3. Google Colab


# Approach
1. Exploratory Data Analysis: Analyzed 7,043 customer records, identifying 27% churn rate and issues like missing "TotalCharges"
2. Preprocessing: Cleaned data, encoded categoricals (e.g., Yes/No to 1/0), and scaled numerical features
3. Custom Feature: Added "CostPerMonth" (MonthlyCharges/tenure) to test cost efficiency’s impact on churn
4. Modeling: Trained Logistic Regression, Random Forest, and XGBoost, focusing on recall to catch churners
5. Evaluation: Achieved 55.2% recall with Logistic Regression (15.2% above baseline 40%), 49.1% with Random Forest, and 49.9% with XGBoost
6. Visualization: Plotted churn by payment method and feature importances

# Key Insights
- Short-tenure (<1 year) and month-to-month customers churn more
- High "CostPerMonth" and electronic check users show elevated churn risk

 # Visualizations
![Churn by Payment Method](https://github.com/nzhumasseiit/customer-churn-prediction/blob/main/churn_payment-3.png)
![Top 10 Feature Importances](https://github.com/nzhumasseiit/customer-churn-prediction/blob/main/feature_importance-3.png)

# How to Run
1. Clone this repo.
2. Upload "WA_Fn-UseC_-Telco-Customer-Churn.csv" from Kaggle to Colab
3. Run the notebook ("churn_prediction.ipynb")

[Link to notebook: customer_churn_prediction.ipynb] (https://github.com/nzhumasseiit/customer-churn-prediction/blob/main/Customer_Churn_Prediction-2.ipynb))
