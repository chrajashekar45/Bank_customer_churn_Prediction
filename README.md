# Bank Customer Churn Prediction

Predicting customer churn is a critical task for financial institutions, enabling proactive retention strategies and minimizing revenue loss. This repository presents a comprehensive end-to-end machine learning solution to predict whether a customer will leave a bank, leveraging real-world banking data.

---

## Table of Contents

- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Project Overview](#project-overview)
- [Key Steps & Methodology](#key-steps--methodology)
- [Results & Insights](#results--insights)
- [How to Run](#how-to-run)
- [Technologies Used](#technologies-used)
- [Conclusions & Next Steps](#conclusions--next-steps)
- [Author](#author)

---

## Problem Statement

Banks lose significant revenue when customers close their accounts (“churn”). Predicting churn enables targeted interventions, offering competitive products and services to retain valued customers. This project implements a predictive analytics pipeline to identify customers at risk of churning based on their demographics, transaction patterns, and product/service usage.

---

## Dataset

- **File:** `Churn Modeling.csv`
- **Rows:** 10,000 customers
- **Features:** Demographics, account properties, and activity metrics
    - `CreditScore`
    - `Geography` (France, Spain, Germany)
    - `Gender`
    - `Age`
    - `Tenure`
    - `Balance`
    - `NumOfProducts`
    - `HasCrCard`
    - `IsActiveMember`
    - `EstimatedSalary`
    - `Exited` (Target: 1 = churned, 0 = retained)

---

## Project Overview

1. **Data Exploration & Preprocessing:**  
   Comprehensive EDA including missing value checks, feature distributions, and outlier analysis. Categorical features are encoded and data is normalized as appropriate.

2. **Feature Engineering & Selection:**  
   Selection of impactful features using correlation analysis and domain knowledge. 

3. **Model Development:**  
   Implementation of several machine learning algorithms including Logistic Regression, Decision Trees, Random Forests, and advanced classifiers. Hyperparameter tuning using techniques like grid search or cross-validation.

4. **Evaluation & Interpretation:**  
   Models evaluated with accuracy, precision, recall, F1, and ROC-AUC. Confusion matrices and feature importances are visualized for business insights.

---

## Key Steps & Methodology

- **Data Cleaning:**  
  Removing redundant features (e.g., RowNumber, CustomerId, Surname), checking for data consistency.

- **Encoding Categorical Variables:**  
  One-Hot Encoding/Label Encoding for `Geography` and `Gender`.

- **Handling Imbalances:**  
  Strategies considered for class imbalance (e.g. SMOTE, class weighting).

- **Model Training & Testing:**  
  - Splitting data into train/test sets.
  - Training classifiers and comparing baseline to advanced models.
  - Hyperparameter tuning.

- **Performance Metrics:**  
  Accuracy, ROC-AUC, Precision/Recall, and F1 Score.

---

## Results & Insights

- **Key Churn Indicators:**  
  Customers’ age, balance, tenure, number of products, credit card holding, and activity status are highly indicative of churn probability.
- **Best Model:**  
  (Fill in based on analysis — e.g., “Random Forest achieved ROC-AUC of 0.86 with strong recall for churned customers.”)
- **Business Impact:**  
  The framework allows the bank to prioritize customer retention efforts for high-risk segments, improving both customer experience and bottom line.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/chrajashekar45/Bank_customer_churn_Prediction.git
   cd Bank_customer_churn_Prediction
   ```

2. Install dependencies (recommended: use a virtual environment):
   ```bash
   pip install -r requirements.txt
   ```
   *(or manually ensure packages like pandas, numpy, scikit-learn, matplotlib, seaborn, etc. are installed)*

3. Open and Run the Jupyter Notebook:
   ```bash
   jupyter notebook Bank_customer_churn_Prediction.ipynb
   ```

---

## Technologies Used

- Python 3.x
- Jupyter Notebook
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## Conclusions & Next Steps

- The model effectively identifies potential churned customers, providing actionable insights for retention.
- Further improvements could include:
  - Incorporation of more customer behavioral data
  - Ensemble models and deep learning
  - Deployment as an API or dashboard for real-time scoring

---

