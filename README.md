# Credit Risk Intelligence & Loan Portfolio Analysis

A business-focused analysis of historical consumer lending data, designed to help decision-makers understand portfolio composition, distinguish patterns of credit risk and identify where lending and monitoring practices may warrant closer review.

This work was presented to paying clients. The public repository uses the historical LendingClub dataset rather than confidential client records, so the analytical approach can be reviewed without disclosing proprietary information.

## Dashboard preview

<img width="1322" height="736" alt="Credit risk and loan portfolio analysis dashboard" src="https://github.com/user-attachments/assets/f6c1aac8-4cf2-4d08-a4f4-bcd4c6d4dff7" />

## The business challenge

Lending decisions involve balancing portfolio growth with the risk that borrowers may not repay. When performance is reviewed only through overall repayment figures, important differences between loan segments can be overlooked.

This analysis explores four management questions:

1. **Portfolio health and exposure:** How are loans distributed across repayment and delinquency stages?
2. **Credit quality and risk differentiation:** How does historical default performance vary across credit grades?
3. **Borrower and loan characteristics:** How do loan purpose, borrower characteristics and pricing relate to observed outcomes?
4. **Risk-informed financial decisions:** What should management investigate, monitor or review based on the patterns?

## What the analysis found

The analysis covers **200,000 historical loan records** from the LendingClub 2007–2018 dataset.

### 1. Portfolio health

| Risk stage | Loan records | Share of analysed records |
|---|---:|---:|
| Performing* | 163,629 | 81.81% |
| Defaulted | 35,091 | 17.55% |
| High risk | 785 | 0.39% |
| Watchlist | 495 | 0.25% |
| **Total** | **200,000** | **100%** |

*Performing combines loans recorded as **Current** and **Fully Paid**. These are different states: one represents loans still being repaid, while the other represents loans that have been repaid.

The defaulted share represents the proportion of records classified as defaulted in this historical analysed sample. It is not a current default rate, a forecast, or a measure of financial loss.

### 2. Credit quality and risk differentiation

Historical default rates increased across the loan-grade categories:

| Loan grade | Historical default rate |
|---|---:|
| A | 5.16% |
| B | 11.59% |
| C | 19.50% |
| D | 27.52% |
| E | 34.45% |
| F | 42.65% |
| G | 50.39% |

The pattern shows a clear relationship between loan grade and historical repayment outcomes in the analysed records. Grade G had almost ten times the default rate of Grade A.

**Business implication:** Credit-grade performance can help management identify segments that may warrant closer review of assessment criteria, risk appetite and monitoring intensity. The observed relationship should not be treated as proof that grade alone causes default.

### 3. Borrower and loan characteristics

Default rates also varied by stated loan purpose. Examples include:

| Loan purpose | Historical default rate |
|---|---:|
| Renewable energy | 26.79% |
| Small business | 26.24% |
| House | 24.16% |
| Moving | 21.44% |
| Medical | 19.46% |
| Debt consolidation | 18.82% |
| Credit card | 14.46% |
| Car | 14.23% |

These differences provide starting points for further segment review. Category sizes should be considered before drawing conclusions, since a percentage based on a small number of loans may be unstable.

Average interest rates also differed by risk stage:

| Risk stage | Average interest rate |
|---|---:|
| Performing | 11.83% |
| Defaulted | 14.73% |
| High risk | 15.32% |
| Watchlist | 15.37% |

Higher average rates in delinquent and defaulted groups raise a useful management question: does loan pricing adequately reflect risk while remaining affordable to borrowers? These averages alone do not establish whether pricing compensates for losses or contributes to repayment pressure.

### 4. Risk-informed financial decisions

The findings can support management discussions and further investigation in areas such as:

- Reviewing credit-grade performance and lending criteria.
- Strengthening monitoring of loans moving into early delinquency.
- Investigating loan-purpose segments with higher observed default rates.
- Assessing pricing alongside repayment outcomes and borrower affordability.
- Improving portfolio reporting so decision-makers can distinguish current, repaid, delinquent and defaulted loans.

These are **decision-support recommendations**, not claims of realised savings, reduced defaults or increased profitability. The project analyses historical data and does not measure the impact of implementing these actions.

## Analytical approach

The workflow covered:

1. **Data preparation in Python:** selecting relevant fields, handling missing values, standardising selected variables, cleaning loan-term values and preparing the analytical dataset.
2. **Risk-stage classification:** grouping loan statuses into Performing, Watchlist, High Risk and Defaulted categories.
3. **Data storage and querying:** using MySQL as part of the data workflow.
4. **Business analysis:** comparing portfolio composition, credit grades, loan purposes and interest rates across risk stages.
5. **Reporting:** presenting portfolio patterns and comparisons in an interactive Power BI report.

## Dashboard

The Power BI report brings the analysis together through portfolio overview, risk distribution, loan-grade performance, borrower segmentation and loan-purpose comparisons.

**Project files**

- [Open the Power BI report](./Loan%20and%20Customer%20risk%20analysis.pbix)
- [View the Python analysis notebook](./Loan%20Analysis.ipynb)
- [View the processed loan sample](./loan_sample.xlsx)
- [View the loan fact table](./loan_fact_table.xlsx)

## Tools and technologies

- **Python:** Pandas, NumPy, Jupyter Notebook
- **MySQL:** data storage and querying
- **Power BI:** interactive reporting and data visualisation
- **Excel:** processed data files

## Dataset and scope

The public analysis uses the LendingClub historical loan dataset covering 2007–2018. It includes **the first 200,000 records** from the source data; this is not documented as a random sample and may not represent the full LendingClub population or other lending portfolios.

The public files are historical third-party data and do not contain confidential records from the paying clients to whom this work was presented. The original source file is not included in this repository because of its size. Processed files are provided for reference.

### Important interpretation limits

- The results describe historical records, not a live lending portfolio.
- The 200,000-record selection may contain selection bias because it uses the first records rather than a documented random sample.
- The Performing category combines Current and Fully Paid loans.
- The analysis reports loan counts and observed rates; it does not establish current outstanding-balance exposure, realised financial losses, or recoveries.
- Associations in the data should not be interpreted as causal relationships or as a predictive credit-scoring model.
- Findings from this dataset should be validated against an institution's own portfolio before being used to change lending policy.

## Project structure

```text
Loan-Default-and-Customer-Risk-Analysis/
├── Loan Analysis.ipynb
├── Loan and Customer risk analysis.pbix
├── loan_fact_table.xlsx
├── loan_sample.xlsx
├── requirements.txt
└── README.md
```

## Professional focus

Business Intelligence | Performance Analytics | Credit Risk Intelligence

**See Beyond Numbers — turn data into clearer decisions.**
