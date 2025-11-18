# customer-profitability-retention
End-to-end Customer Profitability &amp; Retention Analysis (Python + SQL + Power BI)

📊 Customer Profitability & Retention Analysis
End-to-end Data Analytics Project (Python • SQL • Power BI)

This project analyzes customer profitability, retention patterns, churn behavior, and at-risk segments using the Online Retail II dataset.
It demonstrates a full-stack data analyst workflow:

✔ Data Cleaning & Transformation (Python)
✔ SQL-style aggregations & cohort preparation
✔ Customer segmentation using RFM
✔ Profitability & retention deep-dive
✔ Interactive Power BI Dashboard
✔ Business insights + recommended actions

This is a real-world, industry-ready analysis suitable for retail, e-commerce, or subscription-based companies.

⭐ Dashboard Preview
(Full interactive PBIX available in repo)

🧠 Executive Summary

Goal: Identify which customers drive profit, who is at risk of churn, and how retention evolves over time — enabling better targeting and marketing ROI.

Key Insights:

40.8% churn (180 days) → high customer leakage

Top 10% customers contribute 63.9% of total revenue → concentration risk

Post-2010 cohorts show declining retention → customer loyalty weakening

3,000+ customers active in last 90 days → strong core segment

Significant “At-Risk” RFM group → win-back opportunity

High-value customers (top 1%) generate ~32% total profit

These insights directly support
📈 Retention strategy,
🎯 Profit optimization, and
💰 Marketing spend allocation.

🗂 Project Architecture
customer-profitability-retention/
│
├── data/
│   ├── sample_clean_transactions.csv
│   ├── customers_summary.csv
│   ├── at_risk_customers.csv
│
├── dashboard/
│   └── customer_profitability.pbix
│
├── notebook/
│   └── 01_data_cleaning_and_sqlite.ipynb
│
├── visuals/
│   ├── Top10 Profit.png
│   ├── Total Profit.png
│   ├── customer revenue vs order frequency.png
│   └── dashboard.png
│
└── README.md

🔧 Tech Stack
Component	Tools Used
Data Cleaning	Python (Pandas, NumPy), Colab
Database	SQLite (via pandas to_sql)
Analytics	SQL-style aggregations, Cohort Analysis, RFM Segmentation
Visualization	Power BI Desktop
Version Control	Git + GitHub
🧹 Data Cleaning & Preparation (Python)

Performed in 01_data_cleaning_and_sqlite.ipynb.

✔ Steps Completed

Handled missing values (InvoiceDate, CustomerID)

Removed invalid or negative transactions

Extracted invoice month for cohorts

Fixed inconsistent date formats

Converted InvoiceDate to datetime safely

Created customer-level summary table:

Total revenue

Number of orders

Avg order value

Recency (days since last transaction)

Generated “At-Risk Customer” file (RFM logic)

Final Cleaned Files (Included):

clean_transactions.csv (full dataset)

sample_clean_transactions.csv (GitHub-friendly)

customers_summary.csv

at_risk_customers.csv

📈 Analytics Performed
### 1. Cohort Retention Analysis

Tracks customer retention for each acquisition month across 12 months.

2. Customer Profitability Analysis

Revenue per customer

Profit contribution

Cumulative profit curve

Top 1% & top 10% revenue concentration

3. RFM Segmentation

Creates customer groups such as:

High Value

At-Risk

Loyal

Low-Value

New

4. Churn Analysis

Using 60d / 90d / 180d inactivity thresholds.

5. Scatter Analysis: Customer Revenue vs Order Frequency

Bubble = Avg Order Value.

📊 Power BI Dashboard
Pages Included:

Executive Summary KPIs
(Total Customers, Revenue, Profit, Churn, Active Customers)

Customer Behavior & Segmentation

Cohort heatmap

RFM cards

At-Risk customer table

Profitability & Deep Dive

Top 10 customers by profit

Profit by cohort

Distribution charts

The .pbix file is included for recruiters to explore.

💡 Business Recommendations
1. Reduce churn (40.8%)

Trigger personalized email campaigns for customers inactive for 60–90 days.

Launch loyalty rewards tied to order frequency.

2. Protect the top 10% customers

Since they contribute 63.9% of revenue, offer:

VIP pricing

Early access to new products

Dedicated support

Handcrafted win-back offers if inactive

3. Fix declining cohort retention

Improve first-purchase experience

Provide onboarding (tutorial emails, bundle offers)

Introduce subscription-like benefits

4. Monetize high AOV group

Create product bundles to raise order frequency.

🚀 How to Recreate This Project Locally
1. Clone the repo
git clone https://github.com/ishwara24/customer-profitability-retention.git

2. Install Python dependencies
pip install pandas numpy matplotlib seaborn

3. Run the notebook

Open:

notebook/01_data_cleaning_and_sqlite.ipynb

4. Open the Power BI Dashboard

File → Open →
dashboard/customer_profitability.pbix

⭐ Why This Project Matters (Recruiter-Friendly Section)

This project demonstrates:

✔ SQL + Python + Power BI in one workflow

(A critical skill for data analyst roles)

✔ Ability to clean 1M+ rows of messy real-world data

(Not just toy datasets)

✔ Strong business storytelling

(turning data → insights → strategy)

✔ Dashboard design skill

(highly valued in analytics & product teams)

✔ End-to-end ownership

(from raw dataset → insights → dashboard → repo)

This is a hire-ready, industry-standard analytics project.

🙋‍♀️ Author

Ishwara Sinha
Data Analyst (Python, SQL, Power BI)
📧 [Add your email here if you want]
🔗 [LinkedIn link]
