# D2C Customer Churn Intelligence - Data Audit & EDA

## Project Overview

This repository contains the Data Audit and Exploratory Data Analysis (EDA) phase of the D2C Customer Churn Intelligence project.

The objective of this phase is to understand customer purchasing behavior, product performance, customer satisfaction, delivery experience, and support interactions before building customer segmentation, retention, and churn prediction solutions.

---

## Dataset Description

The analysis uses two datasets:

### Orders Dataset

Contains customer transaction information such as:

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

Contains customer support interaction information such as:

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

├── data/
│   ├── orders.csv
│   └── support_tickets.csv
│
├── notebooks/
│   └── eda_audit.ipynb
│
├── visuals/
│   ├── average_resolution_time_by_support_channel.png
│   ├── churn_distribution.png
│   ├── customer_acquisition_channels.png
│   ├── customer_distribution_age_group.png
│   ├── customer_distribution_city_tier.png
│   ├── customer_loyalty_tier_distribution.png
│   ├── delivery_days_vs_ratings.png
│   ├── marketing_consent_distribution.png
│   ├── missing_values_customers.png
│   ├── orders_by_category.png
│   ├── preferred_product_categories.png
│   ├── ratings_distribution.png
│   ├── reopened_support_tickets.png
│   ├── returned_vs_non_returned_orders.png
│   ├── revenue_by_category.png
│   ├── sentiment_score_distribution.png
│   └── support_issue_type.png
│
├── business_memo.md
├── data_quality_report.md
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Repository Contents

### Notebook

- Complete data audit and exploratory analysis workflow.
- Data cleaning, validation, summary statistics, and visual analysis.

### Data Quality Report

- Missing value analysis
- Data type validation
- Dataset quality observations

### Business Memo

- Business-focused insights
- Recommendations based on analysis findings

### Visualizations

- Charts and plots generated during EDA for customer, order, and support-ticket analysis.

---

## How to Run

### 1. Clone the Repository

```bash
git clone <repository-url>
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open the Notebook

Navigate to:

```text
notebooks/eda_audit.ipynb
```

Run all cells sequentially.

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
- Returned vs non-returned orders
- Customer rating distribution
- Delivery days vs ratings
- Customer acquisition channel analysis
- Customer city tier analysis
- Customer age group analysis
- Customer loyalty tier analysis
- Support issue analysis
- Reopened ticket analysis
- Sentiment score distribution
- Resolution time analysis
- Correlation analysis

---

## Key Findings

- Skin Care generated the highest number of orders and revenue.
- Most customers provided high ratings (4–5 stars).
- Product return rates were relatively low.
- Delivery-related issues appeared frequently in support tickets.
- Most support tickets were resolved without reopening.
- Customer sentiment varied across support interactions.
- Correlation between delivery days, ratings, discounts, and revenue was generally weak.

---

## Business Insights

1. Negative customer sentiment may indicate future churn risk.
2. Delivery-related issues can directly impact customer satisfaction.
3. Returned orders may signal unmet customer expectations.
4. Reopened support tickets require additional attention.
5. Revenue concentration within a few categories may increase business risk.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Future Work

The next phases of the project include:

- RFM Customer Segmentation
- Retention Strategy Design
- Churn Prediction Modeling
- FastAPI Churn Scoring Service

---

Capstone Project: D2C Customer Churn Intelligence & Retention API