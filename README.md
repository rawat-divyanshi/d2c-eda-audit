# D2C Customer Churn Intelligence - Data Audit & EDA

## Project Overview

This repository contains the Data Audit and Exploratory Data Analysis (EDA) phase of the D2C Customer Churn Intelligence project.

The objective is to understand customer purchasing behavior, product performance, customer satisfaction, delivery experience, and support interactions before building customer segmentation and churn prediction models.

---

## Dataset Description

### Orders Dataset

Contains customer transaction information including:

- Order ID
- Customer ID
- Order Date
- Product Category
- Quantity
- Gross Amount
- Discount Percentage
- Delivery Days
- Return Status
- Customer Rating

### Support Tickets Dataset

Contains customer support interaction data including:

- Ticket ID
- Customer ID
- Ticket Date
- Issue Type
- Support Channel
- Resolution Hours
- Sentiment Score
- Reopened Status

---

## Project Structure

```text
d2c-eda-audit/
│
├── data/
│   ├── orders.csv
│   └── support_tickets.csv
│
├── notebooks/
│   └── eda_audit.ipynb
│
├── visuals/
│
├── business_memo.md
├── data_quality_report.md
├── README.md
└── requirements.txt
```

---

## Analysis Performed

### Data Audit

- Dataset structure inspection
- Data type validation
- Missing value analysis
- Summary statistics
- Data quality assessment

### Exploratory Data Analysis

- Product category distribution
- Revenue by category
- Returned vs Non-returned orders
- Customer rating distribution
- Delivery days vs ratings
- Support issue analysis
- Reopened ticket analysis
- Sentiment score distribution
- Resolution time by support channel
- Correlation analysis

---

## Key Findings

- Skin Care generated the highest number of orders and revenue.
- Most customers provided high ratings (4–5 stars).
- Product return rates were relatively low.
- Late delivery was among the most common support issues.
- Most support tickets were resolved without reopening.
- Customer sentiment varied, with some tickets showing negative sentiment.
- Correlation between delivery days, ratings, discounts, and revenue was generally weak.

---

## Business Insights

1. Negative customer sentiment may indicate future churn risk.
2. Delivery-related issues can impact customer satisfaction.
3. Returned orders may signal unmet customer expectations.
4. Reopened support tickets require special attention.
5. Revenue concentration in a few categories increases business risk.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Future Work

- RFM Customer Segmentation
- Customer Retention Strategy
- Churn Prediction Model
- FastAPI Churn Scoring API

---

Capstone Project: D2C Customer Churn Intelligence & Retention API