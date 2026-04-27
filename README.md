# 📊 From Data to Retention: Telecom Churn Analysis & Prediction

> **End-to-end churn management for the telecom industry — combining Power BI data storytelling with Python machine learning to understand, predict, and prevent customer churn.**

---

## 🚨 The Problem

**26.54% of telecom customers were churning — and the business had no way to know who would leave next.**

This project solves that in two steps: first understanding *why* customers leave, then predicting *who* will leave next — giving the business a chance to act before revenue is lost.

---

## 🗂️ Repository Contents

| File | Description |
|---|---|
| `Customer_Churn_Analysis_Dashboard.pbix` | Business Analysis Dashboard — 5 pages of visual storytelling (Power BI) |
| `Customer_Churn_Prediction_Dashboard.pbix` | ML Predictions Dashboard — Risk segmentation & churn probability (Power BI) |
| `Customer-Churn-Predictions.ipynb` | Full Python ML pipeline — EDA, preprocessing, modeling, output |
| `Telco-Customer-Churn.csv` | Source dataset — 7,043 customers, 21 columns (IBM Sample) |
| `churn_predictions_output.csv` | Model output — Churn_Prediction & Churn_Probability for every customer |
| `Data-StoryTelling.pdf` | Complete data storytelling report with business insights |

---

## 🔍 Project Overview

This is a **two-part end-to-end solution**:

### Part 1 — Business Analysis Dashboard (Power BI)
Explores *why* customers are churning across **5 pages** of visual storytelling:

| Page | Focus |
|---|---|
| 1. Customer Overview | Churn rate snapshot and customer base summary |
| 2. Why Are Customers Leaving? | Contract type and payment method analysis |
| 3. Customer Behavior & Churn Patterns | Tenure and monthly charges vs churn |
| 4. Service Impact on Churn | Online security, tech support, streaming services |
| 5. Revenue Impact | Monthly charge distribution across churned vs retained |

### Part 2 — ML Predictions Dashboard (Power BI)
Predicts *who* will churn next using a **Random Forest classifier** across **3 pages**:

| Page | Focus |
|---|---|
| 1. ML Predictions Overview | Total predicted churn, avg probability, predicted churn rate |
| 2. Churn Probability Analysis | Probability distribution, tenure vs probability, charges vs risk |
| 3. Risk Segmentation | High / Medium / Low risk breakdown + Top 20 at-risk customers table |

---

## 📊 Key Results

| Metric | Value |
|---|---|
| Overall Churn Rate | **26.54%** |
| Customers Predicted to Churn | **1,780** |
| High Risk Customers | **1,442** |
| Medium Risk Customers | **461** |
| Low Risk Customers | **5,129** |
| Average Churn Probability | **0.27** |
| Top Churn Drivers | Tenure · Monthly Charges · Contract Type |

---

## 🤖 ML Pipeline

```
Raw Data (7,043 records)
       ↓
Data Cleaning
  • Handled nulls
  • Dropped customerID
  • Converted TotalCharges to numeric
       ↓
Encoding
  • LabelEncoder for all categorical variables
       ↓
Modeling
  • Logistic Regression (baseline)
  • Random Forest Classifier (final model)
  • class_weight=balanced for imbalance handling
  • Threshold = 0.3 for better churn recall
       ↓
Output: Churn_Prediction + Churn_Probability per customer
       ↓
Power BI Dashboard (Risk Segmentation + Action Table)
```

---

## 💡 Key Findings

- 📌 **Month-to-month contracts** are the #1 churn driver — these customers churn at a far higher rate than annual or two-year contract holders
- 📌 **The first 12 months** of a customer relationship are the most critical retention window — churn drops steadily as tenure increases
- 📌 **Higher monthly charges** consistently push churn probability up across all risk categories
- 📌 **Customers without tech support or online security** show significantly higher churn rates than those with these services

---

## 🎯 Recommended Actions

1. **Contact the 1,442 High Risk customers immediately** with personalized retention offers
2. **Incentivize month-to-month customers** to upgrade to longer-term contracts
3. **Focus retention efforts within the first 12 months** of a new customer relationship
4. **Offer better value to high-paying customers** showing early churn signals

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Language | Python 3.8+ |
| Data Manipulation | Pandas, NumPy |
| Machine Learning | Scikit-learn (Logistic Regression, Random Forest) |
| Visualization | Power BI |
| Notebook | Jupyter Notebook |
| Version Control | Git & GitHub |

---

## 📂 Dataset

| Detail | Info |
|---|---|
| File | `Telco-Customer-Churn.csv` |
| Records | 7,043 customers |
| Features | 21 columns — gender, tenure, MonthlyCharges, Contract, PaymentMethod, Churn, etc. |
| Target Variable | Churn (Yes / No) |
| Source | IBM Sample Telecom Dataset |

---

## 👩‍💻 Author

**Brunda K** — Data Scientist Aspirant

- 📧 [brundak777589@gmail.com](mailto:brundak777589@gmail.com)
- 💼 [linkedin.com/in/brunda-k](https://linkedin.com/in/brunda-k)
- 🐱 [github.com/Brunda7k](https://github.com/Brunda7k)

---

> *"Dashboard 1 tells us what is happening and why. Dashboard 2 tells us who to save — and when. Together they form a complete end-to-end churn management solution that is both analytically rigorous and business ready."*
