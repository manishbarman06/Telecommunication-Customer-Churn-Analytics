# 📊 Telco Customer Churn Analysis & Data Preprocessing

This project focuses on analyzing customer retention and churn patterns within a Telecommunications dataset (`7,043` customer records). Using Python's data science ecosystem (`pandas`, `numpy`, `matplotlib`, `seaborn`), the notebook performs data cleaning, feature restructuring, missing value imputation, and Exploratory Data Analysis (EDA) to extract key business insights regarding customer attrition.

---

## 🚀 Key Project Highlights

* **Data Cleaning & Standardization**:
  * Converted numerical fields stored as strings (`Total Charges`) to float types using coercion.
  * Trimmed whitespace across all categorical text variables for clean feature modeling.
  * Imputed missing entries in conditional fields like `Churn Reason` (`No Reason!` assigned to retained customers).
* **Dimensionality & Redundancy Reduction**:
  * Removed unnecessary/redundant geographical indicators (`Country`, `State`, `Count`, `Lat Long`) to streamline downstream analytical tasks.
* **Exploratory Data Analysis (EDA)**:
  * Analyzed overall churn distribution, revealing a **~26.54% churn rate** across the customer base.
  * Inspected unique categories across demographics (`Gender`), billing methods (`Payment Method`), and subscription agreements (`Contract`).

---

## 🛠️ Tech Stack & Libraries Used

* **Language**: Python 3.x
* **Data Manipulation**: `pandas`, `numpy`
* **Data Visualization**: `matplotlib`, `seaborn`
* **Environment**: Jupyter Notebook

---

## 📈 Summary of Dataset Features

The cleaned dataset comprises **29 features** categorized into:

1. **Customer Demographics**: `Gender`, `Senior Citizen`, `Partner`, `Dependents`, `City`, `Zip Code`
2. **Account & Contract Details**: `Tenure Months`, `Contract`, `Paperless Billing`, `Payment Method`, `Monthly Charges`, `Total Charges`
3. **Services Subscribed**: `Phone Service`, `Multiple Lines`, `Internet Service`, `Online Security`, `Online Backup`, `Device Protection`, `Tech Support`, `Streaming TV`, `Streaming Movies`
4. **Churn & Metrics**: `Churn Label`, `Churn Value`, `Churn Score`, `CLTV` (Customer Lifetime Value), `Churn Reason`

---

## 🎯 Next Steps / Future Enhancements

* Perform in-depth bivariate/multivariate visualizations (e.g., Churn vs. Contract Type, Monthly Charges vs. CLTV).
* Feature encoding (One-Hot / Label Encoding) for categorical variables.
* Build predictive Machine Learning models (Logistic Regression, Random Forest, XGBoost) to classify customers at risk of churn.
