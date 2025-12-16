# 🏦 Credit Risk Modeling: Predictive & Prescriptive Analytics

![Python](https://img.shields.io/badge/Python-Scikit%20Learn-blue?style=flat&logo=scikitlearn) ![Status](https://img.shields.io/badge/Status-Complete-success?style=flat) ![Domain](https://img.shields.io/badge/Domain-BFSI%20%2F%20Banking-green?style=flat)

## 📖 Executive Summary

**Goal:** Answer _"Who will default?"_ and _"What credit policy should we adopt?"_

This project is a high-level financial analysis pipeline designed to minimize Non-Performing Assets (NPA). It goes beyond standard machine learning by not only predicting loan defaults but also recommending a specific **Risk Threshold Strategy** to balance risk vs. revenue.

The solution integrates **Diagnostic Analytics** (understanding root causes of default), **Predictive Modeling** (calculating probability of failure), and **Prescriptive Analytics** (defining the optimal acceptance rate).

---

## 💼 Business Problem & Objectives

Banks face a classic trade-off:

- **Risk:** Approving bad loans leads to financial loss (Default).
- **Opportunity:** Rejecting good loans leads to lost interest income.

**The Objective:** Build a data-driven framework to:

1.  **Diagnose:** Identify key drivers of financial stress (e.g., Debt-to-Income Ratio).
2.  **Predict:** Score every applicant on their likelihood of default (0% to 100%).
3.  **Prescribe:** Recommend an optimal "Cut-off Score" that maximizes profitability, not just model accuracy.

---

## 🛠️ Tools & Technologies Used

This project relies on Python's scientific stack for statistical rigor and decision science.

| Component               | Tool / Library                    | Usage                                                                                       |
| :---------------------- | :-------------------------------- | :------------------------------------------------------------------------------------------ |
| **Data Processing**     | `Pandas`, `NumPy`                 | Handling financial records and feature engineering.                                         |
| **Diagnostic Viz**      | `Matplotlib`, `Seaborn`           | Correlation matrices (Heatmaps) to find relationships between Income and Default.           |
| **Predictive Modeling** | `Scikit-Learn`                    | Logistic Regression & Decision Trees for binary classification.                             |
| **Handling Imbalance**  | `Imbalanced-learn`                | Using SMOTE (Synthetic Minority Over-sampling) to handle rare default events.               |
| **Strategy**            | `Scikit-Plot`, `Precision-Recall` | Visualizing the trade-off between Risk (False Negatives) and Opportunity (False Positives). |

---

## 🔎 The Analysis: Tri-Layer Approach

This project demonstrates the full spectrum of data science in banking:

### 1️⃣ Phase 1: Diagnostic Analytics ("Why do defaults happen?")

_Focus: Root Cause Analysis_

- **Technique:** Correlation Analysis & Hypothesis Testing.
- **Key Question:** "Does a high 'Debt-to-Income' ratio actually correlate with default in our historical data?"
- **Insight:** "Applicants with less than 2 years of employment stability show a 40% higher default rate."

### 2️⃣ Phase 2: Predictive Analytics ("Who will default?")

_Focus: Future Probability_

- **Technique:** Logistic Regression (for interpretability) and Random Forest (for performance).
- **Key Question:** "What is the probability (0.0 to 1.0) that Applicant X will fail to repay?"
- **Metric Focus:** **Recall** (Sensitivity). In banking, missing a defaulter (False Negative) is much more expensive than rejecting a good customer.

### 3️⃣ Phase 3: Prescriptive Analytics ("What should we do?")

_Focus: Decision Science & Strategy_

- **Technique:** Profit/Loss Simulation & Threshold Tuning.
- **The Logic:**
  - _Cost of Default:_ -$50,000 (Average Loan Loss)
  - _Profit from Good Loan:_ +$5,000 (Interest Income)
- **The Recommendation:** "Set the approval threshold at Probability < 0.25. While this rejects 10% of good customers, it avoids 85% of bad loans, resulting in a net profit increase of $2.5M."

---

## 📂 Repository Structure

```text
03_BFSI_Credit_Risk/
├── data/                              <-- Raw loan application data
├── analysis/
│   ├── 01_EDA_and_cleaning.ipynb      <-- (Diagnostic) Correlations & Pattern finding
│   └── 02_risk_prediction_model.ipynb <-- (Predictive) Model Training & Evaluation
├── strategy_report/
│   └── Credit_Risk_Strategy.pdf       <-- (Prescriptive) The Executive Recommendation
└── README.md
```

---

## 🗝️ Key Metrics & Concepts

- **Confusion Matrix:** Understanding Type I (False Positive) vs Type II (False Negative) errors in a financial context.

- **ROC-AUC Score:** Measuring how well the model separates good borrowers from bad ones.

- **Feature Importance:** Which variable matters most? (Credit Score vs. Annual Income).

- **Gini Coefficient:** A standard metric in credit scoring to measure inequality/discrimination capability of the model.

---

## 🚀 How to Navigate

1.  **Start with the Diagnosis:** Open `analysis/01_EDA_and_cleaning.ipynb` to see the health of the data.

2.  **Review the Model:** Open `analysis/02_risk_prediction_model.ipynb` to see the machine learning workflow.

3.  **See the Decision:** Read `strategy_report/Credit_Risk_Strategy.pdf` (or the summary in the notebook) to understand the final business recommendation.

---

### 📫 Contact & Feedback

- **GitHub:** [sonimonish00](https://github.com/sonimonish00)
