# Loan-Default-and-Customer-Risk-Analysis
## Project Overview
Financial institutions face significant challenges in managing credit risk and maintaining healthy loan portfolios. This project analyzes 200,000 consumer loan records to identify default patterns, evaluate borrower risk characteristics, assess portfolio performance, and develop an interactive risk analytics dashboard.

The project combines Python, MySQL, and Power BI to transform raw loan data into actionable business insights that support lending and risk management decisions.

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
├── images/
├── README.md
└── requirements.txt
```

---

## Author

Belyne Lissa Bochere

Data Analytics | Business Intelligence | Risk Analytics
