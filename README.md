# Customer Profitability & Retention Analysis  
### End-to-End Data Analytics Project (Python • SQL • Power BI)

This project presents a complete customer profitability and retention analysis using the **Online Retail II** dataset.  
It demonstrates a real-world data analyst workflow covering:

- Data cleaning and transformation (Python)
- SQL-style aggregation and cohort preparation
- Customer-level metric creation
- RFM segmentation and churn identification
- Profitability deep dive
- An interactive Power BI dashboard

---

## Project Overview

The goal of this project is to answer key questions such as:

- Which customers contribute most to total revenue and profit?
- What do retention and churn trends look like?
- Which customers are at highest risk of churn?
- How do different cohorts behave over time?
- What operational or marketing actions can improve retention and revenue?

This repository contains the complete pipeline from raw data → insights → dashboard.

---

## Dashboard Preview

A full dashboard screenshot is included in the repo (./dashboard.png).

## Data Cleaning (Python)

Performed in: `01_data_cleaning_and_sqlite.ipynb`

Key steps:

- Loaded Online Retail II raw CSV  
- Converted inconsistent date formats to standard datetime  
- Removed rows with missing or invalid CustomerID  
- Removed negative or cancelled transactions  
- Standardized invoice numbers and stock codes  
- Extracted invoice month for cohort analysis  
- Created customer-level summary dataset:  
  - Total revenue  
  - Number of orders  
  - Average order value  
  - Last transaction date  
  - Recency (days since last activity)  
- Generated at-risk customer list using RFM-based logic

**Output files included:**   
`customers_summary.csv`  
`at_risk_customers.csv`  
`sample_clean_transactions.csv`

---

## Analysis Conducted

### 1. Cohort Retention Analysis
- Monthly retention calculated for each acquisition cohort
- Generates cohort heatmaps (Power BI visual)

### 2. Profitability Analysis
- Total revenue and profit by customer
- Top 1% & Top 10% revenue concentration
- Cumulative profit visualization

### 3. Churn Analysis
- 60/90/180 day inactivity windows used  
- At-risk vs active customers segmented

### 4. RFM Segmentation
Labels customers into:
- High value  
- Loyal  
- At-risk  
- Low value  
- New customers  

### 5. Scatter Analysis
- Revenue vs Order Frequency  
- Bubble size = Average Order Value  

---

## Power BI Dashboard

The included `.pbix` file contains:

- Executive summary cards  
- Cohort heatmap  
- At-risk customer table  
- RFM segment cards  
- Profitability ranking charts  
- Customer behavior scatter plot  
- Slicers (Country, Cohort Month, Segment)

---

## Insights Summary

- 40.8% churn rate at 180 days  
- Top 10% customers contribute 63.9% of total revenue  
- Post-2010 cohorts show weaker retention patterns  
- 3,000+ customers active in last 90 days  
- Significant "At-Risk" group identified via RFM segmentation  
- Heavy revenue concentration among elite customers  

---

## Recommendations

### Improve retention:
- Target customers inactive for 60–90 days with reactivation offers
- Launch a structured loyalty program

### Protect high-value customers:
- VIP benefits, exclusive access, periodic check-ins

### Strengthen early cohort experience:
- First-purchase nurturing sequence
- Personalized recommendations

### Re-engage at-risk customers:
- Targeted win-back campaigns  
- Incentives based on previous buying behavior

---

## How to Use This Repository

### 1. Clone the repository:
git clone https://github.com/ishwara24/customer-profitability-retention.git

shell
Copy code

### 2. Install dependencies:
pip install pandas numpy

makefile
Copy code

### 3. Run the notebook:
Open:
notebook/01_data_cleaning_and_sqlite.ipynb

makefile
Copy code

### 4. Use the dashboard:
Open:
dashboard/customer_profitability.pbix


## Author

**Ishwara Sinha**  
Data Analyst | Python • SQL • Power BI  
linkedin.com/in/ishwara-sinha/


