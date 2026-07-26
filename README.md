# HR Employee Attrition Modeling

A machine learning project that predicts employee turnover using classification models, helping organizations identify attrition drivers and take proactive retention action.

---

## Overview
Employee attrition is a costly problem for organizations. This project performs an end-to-end analysis of the IBM HR Analytics dataset — from raw data exploration to a predictive model with actionable business recommendations.

---

## Workflow
1. **Data Understanding** — Loaded and profiled the dataset (26 numeric + 9 categorical features, target: Attrition Yes/No)
2. **Cleaning & Prep** — Checked for missing values and duplicates (none found), removed constant columns (EmployeeCount, Over18, StandardHours), and engineered readable categorical features (Age_Group, Education level, Distance bands, Satisfaction levels)
3. **Exploratory Analysis** — Examined attrition patterns across age, income, tenure, department, and job role
4. **Visualization** — Used Plotly to explore relationships between attrition and factors like education, income, satisfaction, and overtime
5. **Predictive Modeling** — Trained a Logistic Regression model (80/20 split) to predict attrition and rank feature importance

---

## Key Insights
- Overall attrition rate: **16.1%** (~1 in 6 employees)
- **Overtime is the #1 driver** — employees working overtime attrite at ~30% vs ~10% for those who don't
- Employees who leave tend to be younger, lower-paid, and have less tenure
- Lower education levels combined with lower pay show higher attrition — a compounding financial effect
- MaritalStatus and StockOptionLevel are meaningful predictors — single employees and those with low/no stock options leave more
- Job and environment satisfaction confirmed as strong predictors both visually and in the model

---

## Results
| Metric | Score |
|---|---|
| Model | Logistic Regression |
| Train/Test Split | 80/20 |
| Accuracy | 87% |
| Key Predictor | Overtime (3x attrition rate) |

---

## Business Recommendations
- Limit or better compensate mandatory overtime
- Expand stock option offerings for junior and mid-level staff
- Target retention programs at early-career, single employees
- Invest in workplace satisfaction — feedback loops, career growth, healthy environment

---

## Tech Stack
`Python` `pandas` `NumPy` `scikit-learn` `Plotly`

---

## Dataset
IBM HR Analytics Employee Attrition & Performance — publicly available on Kaggle.
- 1,470 employee records
- 35 features
- Binary target: Attrition (Yes / No)

---

## How to Run
```bash
git clone https://github.com/yourusername/hr-attrition-modeling
cd hr-attrition-modeling
pip install -r requirements.txt
jupyter notebook hr_attrition.ipynb
```

---

## Author
**Mo'men Mamdouh**
https://www.linkedin.com/in/mo-men-mamdouh-3457aa311/ · https://github.com/momenmamdouh1996 · momenmamdouh122@gmail.com
