# customer-profitability-retention
End-to-end Customer Profitability &amp; Retention Analysis (Python + SQL + Power BI)

Customer Profitability & Retention Analysis
End-to-End Data Analytics Project (Python • SQL • Power BI)

This project delivers a complete customer profitability and retention analysis using the Online Retail II dataset. It covers the full data analytics pipeline:

Data cleaning & transformation in Python

Customer-level metrics via SQL-style aggregations

Cohort retention analysis

RFM segmentation & churn identification

Profitability deep-dive

Final Power BI dashboard with business insights

📌 Project Overview

The goal is to understand:

Which customers drive the majority of profit

How retention trends change over time

What churn patterns exist

Which segments require attention

Where business value can be increased

This analysis produces actionable insights relevant for retail, e-commerce, and subscription industries.

📊 Dashboard Preview

(Screenshot included in repo)
dashboard.png

📁 Repository Structure
customer-profitability-retention/
│
├── data/
│   ├── sample_clean_transactions.csv
│   ├── customers_summary.csv
│   ├── at_risk_customers.csv
│
├── notebook/
│   ├── 01_data_cleaning_and_sqlite.ipynb
│
├── dashboard/
│   ├── customer_profitability.pbix
│
├── visuals/
│   ├── Top10 Profit.png
│   ├── Total Profit.png
│   ├── customer revenue vs order frequency.png
│   └── dashboard.png
│
└── README.md

🧹 Data Cleaning Summary (Python)

Performed in:
01_data_cleaning_and_sqlite.ipynb

Key steps:

Loaded raw Online Retail II dataset

Removed invalid/negative quantities

Cleaned inconsistent date formats

Parsed timestamps safely

Removed transactions without CustomerID

Created clean_transactions dataset (~1M rows)

Built customer-level summary table:

Total revenue

Number of orders

Average order value

Last transaction date

Days since last activity (Recency)

Identified “At-Risk Customers” using RFM rules

Final output datasets:

clean_transactions.csv

customers_summary.csv

at_risk_customers.csv

🔍 Analytics Performed
1. Cohort Retention Analysis

Retention calculated month-over-month for each acquisition cohort.

2. Profitability Analysis

Revenue & profit per customer

Top 10 customers

Cumulative profit curve

Concentration risk analysis

Top 1% customers

Top 10% customers

3. Churn Analysis

180-day inactivity used as churn threshold.

4. RFM Segmentation

Customer labeled into:

High Value

Loyal

At Risk

Low Value

New Customers

5. Behavioral Analysis

Scatter plot:
Revenue vs Order Frequency (bubble = Avg Order Value)

📈 Power BI Dashboard Features

The dashboard includes:

Executive KPI summary

Cohort heatmap

At-Risk customer table

RFM segmentation cards

Profitability deep dive

Custom slicers for country, cohort month, segment

Interactive filtering

Insights summary pane

Power BI file:
customer_profitability.pbix

💡 Insights Summary

40.8% churn (180 days) → large opportunity to improve retention

Top 10% customers contribute 63.9% of total revenue → high dependency on elite group

Post-2010 cohorts show lower retention → decreasing customer loyalty

3,000+ active customers in last 90 days → strong recurring base

RFM model highlights a significant “At Risk” group needing win-back campaigns

📌 Recommendations
1. Improve Customer Retention

Trigger automated campaigns for 60–90 day inactivity

Introduce loyalty rewards or subscription benefits

2. Protect High-Value Customers

VIP discounts

Early access to new products

Personalized offers

3. Restore Cohort Health

Improve post-purchase experience

Provide product bundles to increase purchase frequency

4. Target “At Risk” Customers

Personalized win-back emails

Offer incentives based on order history

🚀 How to Use This Repository
1. Clone the repo
git clone https://github.com/ishwara24/customer-profitability-retention.git

2. Install dependencies
pip install pandas numpy

3. Run notebook

Open in Jupyter/Colab:

notebook/01_data_cleaning_and_sqlite.ipynb

4. Open Power BI dashboard

Launch:

dashboard/customer_profitability.pbix

👩‍💻 Author

Ishwara Sinha
Data Analyst — Python | SQL | Power BI
linkedin.com/in/ishwara-sinha/
