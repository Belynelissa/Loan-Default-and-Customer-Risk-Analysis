# Loan-Default-and-Customer-Risk-Analysis
## Project Overview
This project analyzes consumer lending data to understand loan performance, borrower risk behavior, and key drivers of default.  
It segments loans into **Performing, Watchlist, High Risk, and Defaulted** categories and builds an interactive Power BI dashboard for portfolio monitoring.

The goal is to help financial stakeholders identify risk patterns early and improve credit decision-making.

---

## Business Objectives

The analysis aimed to answer the following questions:

- What proportion of the loan portfolio is performing versus defaulted?
- Which borrower characteristics are associated with higher risk?
- How does loan grade relate to portfolio performance?
- Are interest rates aligned with borrower risk levels?
- Which loan purposes contribute most to portfolio risk?
- How is financial exposure distributed across risk categories?

---

## Tools & Technologies

- Python
  - Pandas
  - NumPy
  - Jupyter Notebook

- MySQL
  - Data storage
  - Querying and data management

- Power BI
  - Dashboard development
  - Data visualization
  - KPI reporting

---

## Dataset

The dataset contains approximately 200,000 consumer loan records and includes:

- Loan Amount
- Loan Term
- Interest Rate
- Loan Grade
- Employment Length
- Annual Income
- Debt-to-Income Ratio (DTI)
- Home Ownership
- Loan Purpose
- Loan Status

After cleaning and preprocessing, a focused analytical dataset was created for risk analysis and dashboard development.

> ⚠️ Note: The original dataset (1.6GB) is excluded from this repository due to GitHub size limits. A processed dataset is included for reference.

---

## Data Preparation

Key preprocessing steps included:

- Selection of relevant analytical variables
- Handling missing values
- Standardization of employment length
- Cleaning loan term values
- Creation of risk categories
- Validation of loan status classifications

### Risk Stage Classification

| Risk Stage | Loan Status |
|------------|------------|
| Performing Loans | Fully Paid, Current |
| Watchlist Loans | In Grace Period, Late (16–30 days) |
| High Risk Loans | Late (31–120 days) |
| Defaulted | Charged Off, Default |

---

## Key Findings

### Portfolio Health

- 81.8% of loans were classified as Performing
- 17.5% of loans were classified as Defaulted
- Less than 1% of loans fell within Watchlist and High-Risk categories

### Risk Drivers

- Loan Grade showed a strong relationship with portfolio performance
- Lower-quality grades experienced significantly higher default rates
- Debt Consolidation and Credit Card loans represented the largest concentration of risk

### Pricing Analysis

- Higher-risk borrowers generally received higher interest rates
- Interest rate increases were not always proportional to realized default risk

### Borrower Characteristics

- Debt-to-Income Ratio (DTI) emerged as an important risk indicator
- Employment Length showed relatively weak predictive power compared to loan grade and purpose

---

## Dashboard

The Power BI dashboard provides:

- Portfolio Overview
- Risk Distribution Analysis
- Exposure Analysis
- Loan Grade Performance
- Borrower Risk Segmentation
- Loan Purpose Risk Assessment

### Dashboard Preview

<img width="1322" height="736" alt="Loan and Customer risk analysis dashboard" src="https://github.com/user-attachments/assets/f6c1aac8-4cf2-4d08-a4f4-bcd4c6d4dff7" />


---

## Project Structure

```text
Loan Default and Customer Risk Analysis
│
├── data/
├── notebooks/
├── dashboard/
├── README.md
└── requirements.txt
```

---

## Author

Belyne Lissa Bochere

Data Analytics | Business Intelligence | Risk Analytics
