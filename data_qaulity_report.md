# Data Quality Report

## Dataset Overview

The project contains two datasets:

1. orders.csv
2. support_tickets.csv

The datasets were examined for structure, missing values, data types, and consistency before performing exploratory data analysis.

---

## Orders Dataset

### Basic Information

- Total Records: 10,009
- Key Fields:
  - order_id
  - customer_id
  - order_date
  - category
  - quantity
  - gross_amount
  - discount_pct
  - delivery_days
  - returned
  - rating

### Data Quality Findings

- No duplicate order IDs detected.
- Numerical columns contain valid values.
- Product categories are consistently formatted.
- Ratings range between 1 and 5.
- Return status is stored as a binary variable (0 = Not Returned, 1 = Returned).
- A small number of rating values are missing.

### Missing Values

- Rating column contains missing values.
- Other important columns appear complete.

---

## Support Tickets Dataset

### Basic Information

- Total Records: 1,921
- Key Fields:
  - ticket_id
  - customer_id
  - ticket_date
  - issue_type
  - support_channel
  - resolution_hours
  - sentiment_score
  - reopened

### Data Quality Findings

- No missing values detected.
- Ticket IDs are unique.
- Support channels are consistently recorded.
- Sentiment scores fall within expected range (-1 to 1).
- Reopened tickets are stored as binary values.

---

## Data Cleaning Performed

- Verified dataset structure and column names.
- Checked data types for all variables.
- Examined summary statistics.
- Reviewed categorical value distributions.
- Investigated missing values.
- Validated numerical ranges.

---

## Conclusion

The datasets are generally clean and suitable for exploratory data analysis and churn modeling. Only minor missing values were observed in the rating column, while all other critical fields showed good data quality and consistency.