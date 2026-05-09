# Telecom-Dataset-analysis-and-ML-model
📊 Telecom Customer Churn Analysis
📌 Project Overview

This project focuses on analyzing telecom customer data to identify patterns and factors that lead to customer churn. Using data analysis and machine learning techniques, the goal is to predict whether a customer will churn and help businesses take proactive actions.

📂 Dataset Information
Total Records: 7,043
Total Features: 21
Null Values: 0 (No imputation required)
Duplicates: 0
🔧 Data Preprocessing
Converted total_charges from object → float
Converted senior_citizen from 0/1 → No/Yes
Renamed columns (CamelCase → snake_case)
Verified dataset integrity using:
df.info()
df.isnull().sum()
📊 Exploratory Data Analysis (EDA)
🔍 Key Analysis Performed
Univariate Analysis (Histograms, Count Plots)
Bivariate Analysis (Bar Charts, Scatter Plots)
Outlier Detection (Boxplots using IQR method)
📈 Key Insights
26.5% customers churned → Class imbalance present
Month-to-month contracts have highest churn
Electronic check payments show higher churn rates
Fiber optic users + low tenure + no add-ons → High churn risk
🤖 Machine Learning Models
Model	Test Accuracy	Precision	Recall	F1 Score
Logistic Regression	80.6%	0.66	0.56	0.60
Decision Tree	72.6%	0.63	0.54	0.58
Random Forest	80.6%	0.68	0.51	0.58
Gradient Boosting 🏆	85.1%	0.77	0.65	0.70
KNN (k=7)	76.0%	0.54	0.50	0.52
XGBoost	80.4%	0.66	0.54	0.59
SVM (RBF Kernel)	79.8%	0.71	0.48	0.57
🏆 Best Model
Model: Gradient Boosting
Accuracy: 85.1%
F1 Score: 0.70
AUC Score: 0.914
📉 Model Evaluation
ROC Curve Analysis
Confusion Matrix
AUC Comparison
📊 AUC Scores
Gradient Boosting: 0.914 (Best)
Random Forest: 0.887
Logistic Regression: 0.842
XGBoost: 0.835
⚙️ Pipeline Used
ColumnTransformer
StandardScaler (Numerical Features)
OneHotEncoder (Categorical Features)
Classifier Models
📌 Key Business Insights
Customers with short tenure are more likely to churn
Contract type plays a major role in retention
Payment method impacts customer loyalty
Targeting high-risk customers can reduce churn significantly
🚀 Future Improvements
Hyperparameter tuning (GridSearch / RandomSearch)
Handling class imbalance (SMOTE, class weights)
Deploy model using Flask / Streamlit
Real-time churn prediction dashboard
🛠️ Tech Stack
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
XGBoost
📎 How to Run
👨‍💻 Author

Prabhat Prajapati
