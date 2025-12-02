# Customer-churn-prediction
RAHUL KUDURU
# 📘 Customer Churn Prediction using Ensemble Learning & Explainable AI

This project focuses on predicting customer churn using advanced ensemble learning techniques and Explainable AI (XAI) methods. The goal is to help telecom companies identify customers who are likely to leave and understand the reasons behind their churn behavior using SHAP explainability.

1. Project Overview**

Customer churn is one of the biggest challenges in the telecom industry. Retaining customers is more cost-effective than acquiring new ones, making churn prediction an essential task.

In this project, we:

* Preprocessed the **Telco Customer Churn** dataset
* Handled missing values and categorical variables
* Built multiple ML models
* Selected the best model based on performance
* Applied **XGBoost** for high-accuracy churn prediction
* Used **SHAP (Explainable AI)** to interpret the model
* Visualized insights and key contributors to churn

---

2. Objectives

* Predict whether a customer will churn (Yes/No)
* Identify significant factors influencing churn
* Build an accurate and explainable ML model
* Evaluate performance using accuracy, precision, recall, and F1 score
* Provide actionable insights for business decision-making

---

3. Project Architecture**

```
ChurnPredictionProject/
│
├── data/                   # Dataset (Excel file)
├── notebooks/              # Jupyter notebook for end-to-end model building
├── models/                 # Trained models (if saved)
├── src/                    # Optional scripts (preprocessing, training, etc.)
├── reports/                # Project report, PPT, documentation
├── README.md               # Project description
└── test.py                 # Test file (optional)
```

---

4. Tools & Technologies

### **Programming**

* Python

### **Libraries**

* pandas
* numpy
* seaborn
* matplotlib
* scikit-learn
* xgboost
* shap

### **Environment**

* VS Code
* Jupyter Notebook

### **Version Control**

* Git & GitHub

---

5. Methodology

### **Step 1: Data Loading**

* Loaded dataset from `data/Telco_customer_churn.xlsx`
* Checked missing values and data types

Step 2: Data Cleaning**

* Converted “Total Charges” to numeric
* Removed unnecessary columns (location-based fields)

Step 3: Encoding**

* Applied **One-Hot Encoding** for categorical features

Step 4: Splitting the Data**

* Train-test split (80/20 ratio)

Step 5: Model Training**

Models used:

* Logistic Regression
* Random Forest
* XGBoost (best performing)

Step 6: Evaluation**

* Achieved accuracy ~ **93%** (Random Forest)
* XGBoost achieved ~ **80%** depending on parameter tuning
* Avoided overfitting by cross-checking results

Step 7: Explainable AI**

Used **SHAP** to:

* Interpret feature contributions
* Identify top churn factors (e.g., contract type, support services)

---

6. Results**

### **Best Model:**

✔ **Random Forest Classifier**
✔ **Accuracy:** ~93%
✔ Balanced performance across precision, recall, and F1-score

### **Insights**

* Month-to-month contract users churn more often
* Higher monthly charges increase churn probability
* Lack of tech support increases churn risk
* Paperless billing customers show different churn patterns

---

7. Discussion**

### **Challenges Faced**

* Missing values in “Total Charges”
* Handling large number of categorical features
* Preventing XGBoost installation errors on macOS (fixed using Homebrew)

### **How Challenges Were Solved**

* Cleaned and type-converted fields
* Used One-Hot Encoding for categories
* Installed libomp to fix XGBoost runtime issues
* Used SHAP to ensure model transparency

---

#8. Conclusion

This project successfully demonstrates how machine learning and explainable AI can be combined to create a powerful churn prediction system. The model not only delivers strong accuracy but also provides business-friendly insights into **why** customers churn, enabling telecom companies to take targeted retention actions.

---

9. References

* Kaggle Telco Customer Churn Dataset
* scikit-learn documentation
* XGBoost official docs
* SHAP documentation
* Python official documentation




