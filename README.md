# Telco Customer Churn Analysis

A end-to-end data analysis project to identify why customers are leaving a telecom company and provide actionable business recommendations to reduce churn.

---

## Problem Statement
The company has a **26.6% churn rate** — roughly 1 in 4 customers is leaving. This analysis identifies the root cause of churn and calculates the revenue impact of fixing it.

---

## Tools Used
- **Python** — data cleaning and exploratory data analysis
- **Pandas, Matplotlib, Seaborn** — data manipulation and visualization
- **SQL (SQLite)** — business queries and segmentation
- **Power BI** — interactive dashboard

---

## Dataset
- Source: [Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 7,032 customers, 21 features
- Target column: `Churn` — whether the customer left or not

---

## Key Findings

### Finding 1 — Contract Type is the Biggest Driver
- 88.6% of all churned customers were on month-to-month contracts
- Month-to-month churn rate: **42.7%**
- One year churn rate: **11.2%**
- Two year churn rate: **2.8%**

> The price difference between contract types is small but the churn difference is massive — the problem is lack of commitment, not price.

### Finding 2 — Fiber Optic Customers Churn the Most
- Fiber optic on month-to-month: **54.6% churn rate**
- Fiber optic on two year contract: **7.2% churn rate**
- Fiber optic customers pay $87/month on average — the most expensive service with the highest churn

> Two year fiber optic customers pay even more ($104/month) but churn the least — confirming price is not the issue, contract commitment is.

### Finding 3 — First Month is the Most Critical Period
- 375 customers left in month 1 alone — more than any other month
- Of 235 fiber optic customers who joined, **203 left in month 1 (86.4% churn rate)**
- Of those 203 churners, **200 had no tech support**
- Churn drops from 59.1% in months 1-2 to just 6.6% by months 61-72

> New customers sign up for the most expensive service, get no support when something goes wrong, and leave before they even settle in.

---

## Revenue Impact

| Metric | Value |
|---|---|
| Total churned customers | 1,869 |
| Monthly revenue lost | $139,131 |
| Yearly revenue lost | $1,669,570 |
| Fiber optic month-1 no-support customers | 200 |
| Yearly revenue at risk from this group alone | $186,396 |

---

## Recommendations

**1. Bundle free tech support for new fiber optic customers (first 3 months)**
200 out of 203 fiber optic customers who left in month 1 had no tech support. A free 3 month trial costs far less than losing $186,396 per year from this group alone.

**2. Incentivize month-to-month customers to switch to annual contracts**
Month-to-month customers churn at 42.7% vs 2.8% for two year contracts. Even a small discount to move customers to an annual plan would dramatically reduce churn.

**3. Create an early warning system for months 1-5**
Flag all new customers on fiber optic with no add-ons as high risk and proactively reach out with support offers before they decide to leave.

---

## Dashboard Preview
![Customer Churn Dashboard](customer%20churn%20dashboard.pdf)
---
## Author
Made by Muhammad Aqsam Qurashi 
