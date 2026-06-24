# SummerInternship-Projects
# Project 1.Churn Prediction Model
# 📊 Telecom Customer Churn Prediction Model

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Tools-Jupyter%20Notebook-orange.svg)](https://jupyter.org/)
[![Framework](https://img.shields.io/badge/Framework-Scikit--Learn-green)](https://scikit-learn.org/)

An end-to-end Machine Learning project to predict customer churn for a telecom company using the **IBM Telco Customer Churn Dataset**. This model helps identify customers who are at a high risk of leaving, enabling the company to take proactive retention measures.

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description & Source](#dataset-description--source)
- [Key Features & Workflow](#key-features--workflow)
- [Technologies Used](#technologies-used)
- [Installation & Usage](#installation--usage)
- [Model Performance](#model-performance)
- [Key Insights](#key-insights)
- [What I Learnt From This Project](#what-i-learnt-from-this-project)
- [Future Improvements](#future-improvements)

---

## 🚀 Project Overview
In the telecom industry, acquiring new customers is often significantly more expensive than retaining existing ones. This project focuses on analyzing customer demographics, account information, and service usage patterns to build a predictive binary classification model. 

The ultimate goal is to flag "at-risk" customers with high accuracy and recall, allowing marketing teams to target them with special offers or incentives.

---

## 📅 Dataset Description & Source
The project utilizes the industry-standard **IBM Telco Dataset**, which contains information on 7,043 customers and 21 features.

*   **Data Source:** [Kaggle - Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) / IBM Base Samples.

### Feature Categories:
*   **Demographics:** Gender, Senior Citizen status, Partner, and Dependents.
*   **Customer Account Info:** Tenure, Contract type (Month-to-month, One year, Two year), Payment Method, Paperless Billing, Monthly Charges, and Total Charges.
*   **Services Signed Up For:** Phone service, Multiple lines, Internet service (DSL, Fiber optic, No), Online Security, Online Backup, Device Protection, Tech Support, Streaming TV, and Streaming Movies.
*   **Target Variable:** `Churn` (Whether the customer left within the last month: Yes/No).

---

## 🛠️ Key Features & Workflow

### 1. Data Cleaning & Preprocessing
*   Handled missing values (e.g., converting empty spaces in `TotalCharges` to numeric and imputing).
*   Encoded categorical variables using **One-Hot Encoding** and **Label Encoding**.
*   Feature scaling using **StandardScaler** to normalize continuous metrics like `Tenure` and `MonthlyCharges`.

### 2. Exploratory Data Analysis (EDA)
*   Visualized churn distribution against contract types, payment methods, and tenure.
*   Identified high correlation between Fiber Optic internet users, Month-to-Month contracts, and high churn rates.

### 3. Model Building & Evaluation
*   Split data into Training and Testing sets (typically 80/20 or 75/25).
*   Handled class imbalance using techniques like **SMOTE** (Synthetic Minority Over-sampling Technique) if necessary.
*   Trained multiple classifiers (e.g., Logistic Regression, Random Forest, Gradient Boosting, or XGBoost).
*   Evaluated models using **ROC-AUC score, Precision, Recall, and F1-Score** to ensure balanced performance.

---

## 💻 Technologies Used
*   **Language:** Python
*   **Libraries:** 
    *   Data Manipulation: `pandas`, `numpy`
    *   Visualization: `matplotlib`, `seaborn`
    *   Machine Learning: `scikit-learn`, `imblearn` (SMOTE)

---

## ⚙️ Installation & Usage

### Prerequisites
Make sure you have Python installed. Then, clone this repository:

```bash
git clone [https://github.com/AmaanShaikh2006/SummerInternship-Projects.git](https://github.com/AmaanShaikh2006/SummerInternship-Projects.git)
cd SummerInternship-Projects
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook
