# HR Workforce Risk & Attrition Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![PowerBI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)
![ML](https://img.shields.io/badge/ML-Random%20Forest-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## Overview
This project analyzes employee attrition at IBM using a dataset of 1,470 employees.
The goal was to identify why employees are leaving, who is most at risk,
and what it is costing the business — then build a machine learning model
to predict future attrition before it happens.

**Bottom line: Attrition is costing this company $6.8 million per year.
This project shows exactly where it is coming from and what to do about it.**

---

## Key Findings

| Finding | Number |
|---|---|
| Overall attrition rate | 16.1% |
| Highest risk department | Sales — 20.6% |
| Overtime workers attrition | 30.5% vs 10.4% |
| Salary gap (leavers vs stayers) | $2,046/month |
| Youngest age group (18-25) | 34.8% attrition |
| Total cost of attrition | $6.8 Million |
| Model accuracy | 76.5% |
| Model recall for leavers | 41% |

---

## Project Structure
```
hr-attrition-analysis/
│
├── Hr Analytics.ipynb                           # Full Python analysis notebook
├── WA_Fn-UseC_-HR-Employee-Attrition.csv        # Original dataset
├── hr_attrition_clean.csv                       # Cleaned dataset
├── hr_attrition_model.pkl                       # Saved Random Forest model
├── HR Workforce Risk & Attrition Dashboard.pbix # Power BI dashboard
├── HR_Attrition_Analysis_Report.pdf             # Full analysis report
└── README.md
```

---

## Tools & Technologies

- **Python** — Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Machine Learning** — Random Forest, SMOTE for class imbalance
- **Power BI** — Interactive 4-page dashboard
- **Jupyter Notebook** — Development environment via Anaconda
- **GitHub** — Version control and portfolio

---

## Analysis Steps

1. **Data Loading** — Loaded IBM HR dataset (1,470 rows, 35 columns)
2. **Data Audit** — Verified zero missing values, checked data types
3. **Data Cleaning** — Dropped useless columns, encoded categorical variables
4. **Exploratory Analysis** — Attrition by department, age, overtime, salary
5. **Cost Model** — Calculated $6.8M total cost using 6x monthly salary formula
6. **Correlation Analysis** — Identified key drivers of attrition
7. **ML Model** — Built Random Forest with SMOTE balancing
8. **Model Tuning** — Improved recall from 10% to 41%
9. **Dashboard** — Built 4-page Power BI dashboard
10. **Report** — Written analysis with recommendations

---

## Machine Learning Model

- **Algorithm:** Random Forest Classifier
- **Training data:** 80% (1,176 rows)
- **Test data:** 20% (294 rows)
- **Class balancing:** SMOTE applied to training set
- **Final accuracy:** 76.5%
- **Recall for leavers:** 41%

### Top 3 Features Driving Attrition:
1. Monthly Income (19.8%)
2. Years in Current Role (12.6%)
3. Age (11.3%)

---

## Recommendations

**Immediate (0-3 months)**
- Reduce mandatory overtime in Sales department
- Benchmark and adjust entry-level salaries
- Run stay interviews for employees without promotion in 4+ years

**Medium-term (3-12 months)**
- Build career progression paths for Sales Representatives
- Introduce flexible working for long-commute employees
- Create retention packages for $3,000-$5,000 salary band

**Long-term (12+ months)**
- Deploy live attrition risk dashboard for HR managers
- Restructure compensation bands to close $2,046/month gap
- Invest in mentorship programs for 18-35 age group

---

## Dataset
IBM HR Analytics Employee Attrition dataset — available on Kaggle.
1,470 employee records across 35 features.

---

## Author
**Anitha Morampudi**
[GitHub](https://github.com/AnithaMorampudi)
