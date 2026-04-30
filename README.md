# 💳 Credit Risk Scoring & Portfolio Monitoring Dashboard
End-to-end credit risk project combining machine learning, risk scoring, and business-oriented dashboarding to support financial decision-making.

## 🎯 Business Problem

Financial institutions face a critical challenge: identifying high-risk clients early to reduce potential credit losses and improve decision-making.

This project aims to:
- Predict the probability of default (PD)
- Segment clients into actionable risk categories
- Estimate expected losses at portfolio level
- Provide an interactive decision-support dashboard

---

## 📊 Dataset

The dataset contains ~30,000 clients with financial and behavioral variables, including:

- Credit limit
- Payment history (multi-period)
- Billing amounts
- Payment amounts
- Delays and repayment status

A fully cleaned and feature-engineered dataset was used for modeling and business analysis.

---

## ⚙️ Methodology

### 1. Data Preparation & Feature Engineering

Advanced features were created to capture credit behavior:

- Number of late payments
- Maximum delay
- Average delay
- Total bill & total payment
- Payment-to-bill ratios
- Credit utilization patterns

Outliers were handled using percentile capping (1% / 99%) to preserve financial data distribution.

---

### 2. Predictive Modeling (Python)

A **Logistic Regression (L2 Regularization)** model was built to predict default probability.

#### Why Logistic Regression?
- High interpretability (critical in finance)
- Robust to multicollinearity
- Suitable for credit risk scoring

#### Model Pipeline:
- Train/Test split (80/20)
- Feature scaling (StandardScaler)
- Class imbalance handling (SMOTE)
- Performance evaluation

#### Key Metrics:
- ROC AUC ≈ 0.75+
- Strong discrimination between default / non-default
- Improved recall on risky clients after SMOTE

---

### 3. Risk Scoring System

A business-oriented scoring system was developed:

- Probability → Score (0–100)
- Risk segmentation:
  - Low Risk
  - Medium Risk
  - High Risk

This allows:
✔ Easy interpretation  
✔ Operational decision-making  
✔ Client prioritization  

---

## 📈 Power BI Dashboard

An interactive dashboard was built to monitor portfolio risk in real-time.
The dashboard is designed for risk managers and decision-makers.

### Key Features:

- 📊 Default rate by risk level
- 👥 Number of clients per segment
- 💰 Expected Loss estimation (EL = PD × EAD × LGD)
- 📉 Risk score distribution
- 🔍 Drill-down analysis with filters

### Risk Drivers Page:

- Impact of late payments on default probability
- Relationship between delay and risk score
- Behavioral patterns of high-risk clients

---

## 💡 Key Insights

- 🔴 **Late payments are the strongest driver of default risk**
- 📈 Default probability increases sharply with delay
- ⚠️ High-risk clients drive the majority of expected losses
- 📊 Medium-risk segment represents the largest exposure volume
  

---

## 💼 Business Impact

This project demonstrates how data can directly improve financial decision-making:

✔ Early identification of risky clients  
✔ Reduction of expected losses  
✔ Better credit approval strategies  
✔ Portfolio risk monitoring in real-time  
- Improve credit risk monitoring
- Reduce financial losses through early detection
- Support data-driven credit decisions
- Enhance portfolio segmentation strategies

---

## 🧠 Technical Stack

- Python (Pandas, NumPy, Scikit-learn)
- Machine Learning (Logistic Regression, SMOTE)
- Data Visualization (Matplotlib, Seaborn)
- Power BI (DAX, Data Modeling, Dashboarding)
- SQL (data structuring & querying)

---

## 📂 Project Structure
credit-risk-scoring-dashboard/

├── data/
│ └── credit_risk_scoring_results.csv
├── notebook/
│ └── RISK_SCORING_MODEL_CT.ipynb
├── powerbi/
│ └── Credit_risk_score_PBI.pbix
├── README.md

---

## 🚀 Conclusion

This project bridges the gap between **data science and financial risk management**.

It demonstrates the ability to:
- Build interpretable risk models
- Translate data into business decisions
- Design professional dashboards for stakeholders
This project replicates a real-world credit risk workflow used in financial institutions.

## 🚀 Why This Project Matters

This project demonstrates the ability to bridge data science and financial risk management, a key skill required for modern risk analyst roles.
It highlights:
- Strong understanding of credit risk concepts
- Ability to build interpretable models
- Translation of data into business insights
- End-to-end analytical workflow

## 📬 Contact

Open to opportunities in:
 -Quantitative Financial analyst 
 -Financial Risk management
- Financial Risk Analysis
- Credit Risk Modeling
- Data Analytics (Finance / Fintech)
  
