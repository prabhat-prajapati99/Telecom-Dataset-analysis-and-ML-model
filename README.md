# Telecom-Dataset-analysis-and-ML-model

# 📊 Telecom Customer Churn Analysis

## 📌 Project Overview
This project analyzes telecom customer data to identify churn patterns and predict customer behavior using machine learning models. The goal is to help businesses reduce customer churn by identifying high-risk customers.

---

## 📂 Dataset Information
- **Total Records:** 7,043  
- **Total Features:** 21  
- **Null Values:** 0  
- **Duplicate Records:** 0  

---

## 🔧 Data Preprocessing
- Converted `total_charges` from object → float  
- Converted `senior_citizen` from 0/1 → Yes/No  
- Renamed columns (CamelCase → snake_case)  
- Verified data using:
  - `df.info()`
  - `df.isnull().sum()`

---

## 📊 Exploratory Data Analysis (EDA)
- Univariate & Bivariate Analysis  
- Outlier Detection using IQR  

### 🔍 Key Insights
- 26.5% customers churned (class imbalance)  
- Month-to-month contracts have highest churn  
- Electronic check payment → high churn  
- Low tenure + no add-ons → high churn risk  

---

## 🤖 Machine Learning Models

| Model                | Accuracy | Precision | Recall | F1 Score |
|---------------------|---------|----------|--------|----------|
| Logistic Regression | 80.6%   | 0.66     | 0.56   | 0.60     |
| Decision Tree       | 72.6%   | 0.63     | 0.54   | 0.58     |
| Random Forest       | 80.6%   | 0.68     | 0.51   | 0.58     |
| Gradient Boosting 🏆 | **85.1%** | 0.77   | 0.65   | **0.70** |
| KNN (k=7)           | 76.0%   | 0.54     | 0.50   | 0.52     |
| XGBoost             | 80.4%   | 0.66     | 0.54   | 0.59     |
| SVM (RBF Kernel)    | 79.8%   | 0.71     | 0.48   | 0.57     |

---

## 🏆 Best Model
**Gradient Boosting**
- Accuracy: 85.1%  
- F1 Score: 0.70  
- AUC Score: 0.914  

---

## 📉 Model Evaluation
- ROC Curve  
- Confusion Matrix  
- AUC Score Comparison  

---

## ⚙️ Pipeline
- ColumnTransformer:
  - StandardScaler (Numerical Features)
  - OneHotEncoder (Categorical Features)
- ML Models  

---

## 📌 Business Insights
- Short tenure customers churn more  
- Contract type strongly impacts churn  
- Payment method influences retention  
- Targeting high-risk users can reduce churn  

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/telecom-churn-analysis.git
cd telecom-churn-analysis
pip install -r requirements.txt
jupyter notebook
