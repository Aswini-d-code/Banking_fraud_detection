# Banking Fraud Detection using Logistic Regression

This project focuses on detecting fraudulent transactions in a banking dataset using Logistic Regression.
It includes full data preprocessing, feature engineering, machine learning modeling, visual analytics using Power BI & Excel, and insights derived from both SQL and Python analysis.

---

## Dataset Overview

- No missing values.
- All columns have appropriate data types.
- Data includes transaction type, amount, device used, and fraud labels.

---

## Tools Used

- **Python (Jupyter Notebook)** – Preprocessing, SMOTE, ML modeling
- **SQLite** – SQL-based exploratory analysis
- **Excel** – Initial data cleaning and pivot table visualizations
- **Power BI** – Interactive dashboards and visual insights

---

## Key Insights

- **Fraud Count**: ~3000 fraudulent transactions detected.
- **Transaction Amount**: Most frauds occur between ₹3,000 and ₹8,000.
- **High-Risk Types**: `Withdrawal` (29.49%) and `Online Payment` (29.00%) have the highest fraud percentages.
- **High-Risk Devices**: `Mobile` and `ATM` are most associated with fraud.
- **Credit Score Segments**: Fraud mostly occurred in users with **poor to fair** credit scores (Excel & Power BI visualizations used to segment and analyze).

---

## Feature Engineering

- Label encoding applied to categorical features.
- Credit score segmented into groups: Poor, Fair, Good, etc.
- Standard scaling applied to numeric features.
- Used **SMOTE** to handle class imbalance.

---

## Model: Logistic Regression

- **Accuracy**: `67.47%`
- **Recall (Fraud Cases)**: `72%` 
- **Precision (Fraud Cases)**: `45%`
- **Confusion Matrix**:
  - True Negatives: 1412
  - False Positives: 737
  - False Negatives: 239
  - True Positives: 612

**Insight**:  
The model effectively identifies fraudulent transactions with a high recall of 72%, making it suitable for fraud detection.

---

## SQL Analysis (Using SQLite)

Analyzed fraud trends by transaction type:

| Transaction Type | Total Transactions | Fraud Transactions | Fraud % |
|------------------|--------------------|---------------------|---------|
| Withdrawal        | 2547               | 751                 | 29.49%  |
| Online Payment    | 2517               | 730                 | 29.00%  |
| Deposit           | 2420               | 682                 | 28.18%  |
| Transfer          | 2516               | 675                 | 26.83%  |

**Insight**: Withdrawals and online payments have the highest fraud rates.

---

## 📁 Files Included

- `Bank_fraud_detection.ipynb` – Python code for EDA + ML modeling
- `Bank_fraud_detection.xlsx` – Excel analysis, pivot tables, and charts
- `Bank_fraud_detection.pbix` – Power BI interactive dashboard
- `Bank_fraud_dataset.csv`
- `README.md` – Project summary and documentation

---

## ✅ Conclusion

This project demonstrates a complete fraud detection pipeline with data cleaning, visual analytics (Excel + Power BI), SQL exploration, and
machine learning. Logistic Regression performed effectively, especially in identifying frauds with a strong recall.

---

