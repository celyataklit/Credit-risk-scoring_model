# 💳 Credit Risk Scoring & Portfolio Risk Monitoring

End-to-end credit risk project transforming raw customer and repayment data into a decision-support system for default prediction, client risk segmentation, and portfolio monitoring.
This project transforms raw credit data into a decision-support system to predict default risk, segment clients, and monitor portfolio exposure.

---

## 🚀 Key Results

- Built a machine learning model to predict client default risk (ROC AUC ~0.75)
- Created a risk scoring system from 0 to 100
- Segmented clients into Low, Medium, and High Risk categories
- Identified key behavioral drivers of default risk
- Delivered a Power BI dashboard to monitor portfolio exposure and risk distribution

---

## 🎯 Business Objective

Credit risk teams need to identify risky clients early, understand what drives default behavior, and monitor portfolio-level exposure.

This project answers four business questions:

- Which clients are more likely to default?
- What repayment behaviors indicate higher risk?
- How can clients be segmented by risk level?
- What is the current risk profile of the portfolio?

---

## 💼 Business Value

This project supports credit risk decision-making by turning raw financial data into actionable risk insights.

It helps financial institutions:

- Anticipate potential default before it occurs
- Prioritize monitoring of high-risk clients
- Understand the main factors linked to default behavior
- Segment clients for better portfolio management
- Monitor portfolio risk through an interactive dashboard

---

## ⚙️ Methodology

### 1. Data Preparation & Feature Engineering

The raw dataset was transformed into financial and behavioral risk indicators, including:

- Number of late payments
- Maximum payment delay
- Average payment delay
- Total billed amount
- Total repayment amount
- Payment-to-bill ratios
- Credit utilization proxies

Outliers were handled using percentile capping (1% / 99%) to preserve realistic financial dispersion while reducing the impact of extreme values.

---

### 2. Predictive Modeling

A Logistic Regression model with L2 regularization was used to predict default probability.

This model was selected because it is:

- Interpretable
- Suitable for risk environments
- Easy to translate into business decisions
- Able to provide probability-based outputs

Modeling pipeline:

- Train/test split
- Feature scaling with StandardScaler
- SMOTE applied only on training data to handle class imbalance
- Evaluation using ROC AUC, precision, recall, and classification metrics

Performance:

- ROC AUC ~0.75
- Improved detection of default-risk clients
- Clear separation between lower-risk and higher-risk profiles

---

### 3. Risk Scoring & Client Segmentation

Predicted probabilities were converted into a business-oriented risk score from 0 to 100.

Clients were then segmented into:

- 🟢 Low Risk
- 🟡 Medium Risk
- 🔴 High Risk

This makes the model easier to use for non-technical stakeholders and supports operational credit risk monitoring.

---

## 📊 Power BI Dashboard

The Power BI dashboard was designed to provide both portfolio-level monitoring and risk driver analysis.

---

## 📸 Dashboard Preview

### 🔎 Portfolio Monitoring

![Dashboard Overview](images/dashboard_overview.png)

This page provides a global view of the credit portfolio:

- Number of clients by risk segment
- Default rate by risk level
- Risk score distribution
- Potential exposure and portfolio risk indicators

This helps stakeholders understand the current risk profile of the portfolio.

---

### 📉 Risk Drivers Analysis

![Risk Drivers](images/risk_drivers.png)

This page focuses on the behavioral factors associated with default risk:

- Payment delays
- Late payment frequency
- Risk level distribution
- Relationship between repayment behavior and default probability

This helps identify which behaviors require stronger monitoring and attention.

---

## 💡 Key Insights

- Payment behavior is one of the strongest indicators of default risk
- Clients with repeated delays show higher default probability
- Risk segmentation makes the portfolio easier to monitor and prioritize
- The dashboard provides a clear view of portfolio risk and potential exposure
- The project demonstrates how raw banking data can be transformed into a practical risk decision tool

---

## 🧠 Credit Risk Logic

The project focuses primarily on default prediction, client segmentation, and portfolio monitoring.

A simplified Expected Loss approach was also included to connect the model output to financial risk concepts:

Expected Loss = PD × LGD × EAD

Where:

- PD is estimated by the model
- LGD is assumed at 45%
- EAD is approximated using credit limit

This is used as an additional portfolio risk indicator, not as the main objective of the project.

---

## ⚠️ Limitations

- LGD is assumed and not modeled
- EAD is approximated using credit limit
- Logistic Regression may not capture all non-linear relationships
- The dataset is treated as a static snapshot, not a time-series model

---

## 🛠️ Technical Stack

- Python: Pandas, NumPy, Scikit-learn
- Machine Learning: Logistic Regression, SMOTE
- Visualization: Matplotlib
- Power BI: data modeling, dashboarding, risk KPIs
- Git / GitHub

---
## 📂 Project Structure

```text
credit-risk-scoring-model/

├── images/
│   ├── dashboard_overview.png
│   └── risk_drivers.png
│
├── credit_risk_scoring_results.csv
├── RISK_SCORING_MODEL_CT.ipynb
├── Credit_risk_score_PBI.pbix
├── README.md

---

## 🚀 Conclusion

This project demonstrates a complete credit risk analytics workflow:

- Raw data preparation
- Risk-oriented feature engineering
- Default prediction
- Client risk scoring
- Risk segmentation
- Portfolio monitoring through Power BI

It shows the ability to bridge credit risk, financial analysis, machine learning, and business decision-making.

---

## 📬 Contact

Open to opportunities in:

- Credit Risk Analytics  
- Fraud & Financial Crime Analytics  
- Risk Management  
- Fintech Risk Analytics  
- Financial Decision Science  
