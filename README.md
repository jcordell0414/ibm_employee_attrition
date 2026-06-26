# IBM HR Employee Attrition Analysis

## Overview
Analysis of employee attrition patterns across a 1,470-employee dataset using 
Python, SQL, and Tableau. The goal was to identify which factors most strongly 
correlate with attrition and surface actionable retention insights.

## Tools
- **Python** (pandas, numpy, matplotlib, seaborn) — cleaning, EDA, correlation analysis
- **SQL** (SQLite via Python) — structured business question analysis
- **Tableau** — interactive dashboard

## Dataset
IBM HR Analytics Employee Attrition & Performance Dataset  
1,470 rows | 35 columns  
Source: [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

## Key Findings
1. Sales Representatives leave at 39.8% — nearly 4x the rate of Managers (4.9%)
2. Overtime employees leave at 3x the rate of non-overtime employees (30.5% vs. 10.4%)
3. Attrition peaks at 36% in year one and drops sharply after year five
4. Employees who left earned $2,046 less per month on average than those who stayed
5. Distance from home is the strongest numeric predictor of attrition
6. Single employees leave at more than double the rate of divorced employees

## Dashboard
[View on Tableau Public](https://public.tableau.com/app/profile/jace.cordell/viz/ibm_employee_attrition/Overview?publish=yes)

## Project Structure

```text
employee_attrition_analysis/
│
├── employee_attrition_analysis.ipynb
│
├── 1_data/
│   ├── cleaned/
│   │   └── clean_attrition.csv
│   └── raw/
│       └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── 2_scripts/
│   └── employee_attrition_cleaning.ipynb
│
├── 3_visuals/
│   ├── attrition_by_tenure.png
│   ├── attrition_by_jobrole.png
│   ├── attrition_by_department.png
│   ├── attrition_by_overtime.png
│   ├── income_by_attrition.png
│   └── correlation_with_attrition.png
│
└── 4_report/
    └── employee_attrition_report.pdf
```

## Recommendations
1. Conduct targeted retention reviews for Sales Representatives in their first two years, particularly those working overtime and earning below-median income
2. Audit overtime distribution — the 3x attrition rate points to addressable workload imbalance
3. Evaluate compensation benchmarks for early-career employees given the $2,046 monthly income gap between those who stayed and those who left

  
