🛍️ Shopnext Store Analysis Dashboard

A comprehensive Power BI dashboard designed to analyze sales, orders, customer behavior, and product performance for Shopnext, an e-commerce platform.

📊 Overview

This dashboard provides detailed insights into:

📦 Product category performance

🕓 Order punctuality (early vs delayed)

💳 Payment method trends

🌍 State-wise customer distribution

📈 Revenue and seasonal trends

⭐ High/low rated product analysis

Built using Power BI with DAX measures for dynamic data modeling and visualizations.

🛠️ Technologies Used
Tool	Purpose
Power BI	Data visualization
DAX (Data Analysis Expressions)	Calculations and measures
Power Query	Data transformation
CSV/Database	Source data
📈 Key Metrics & Visuals
1. KPI Cards

Total Sales: 14.2M

Delayed Orders: 7K

Early Orders: 89K

2. Top 10 Best-Selling Product Categories

Horizontal bar chart showing top-selling categories like health_beauty, watches, and bed_bath_table.

DAX Example:

Total Sales = SUM(Sales[Sale_Amount])

3. Early vs Delayed Orders by Month

Stacked column chart comparing early and delayed orders across each month.

DAX:

Early Orders = CALCULATE(COUNTROWS(Orders), Orders[Delivery_Status] = "Early")
Delayed Orders = CALCULATE(COUNTROWS(Orders), Orders[Delivery_Status] = "Delayed")

4. Product Rating Insights

Top 10 High-Rated Products

Top 10 Low-Rated Products

Visuals sorted by average rating.

DAX:

Average Rating = AVERAGE(Products[Rating])

5. Delayed Orders by Product Category

Bar chart breaking down delays by category like bed_bath_table, sports_leisure, etc.

6. Payment Method Breakdown

Donut chart showing the percentage of payment types:

Credit Card (78%)

Boleto

Voucher

7. State-wise Customer Analysis

Top states by customer count (SP, RJ, etc.)

Customer Count = DISTINCTCOUNT(Customers[Customer_ID])

8. Seasonal Sales Analysis

Quarterly sales comparison:

Q1: 3.56M

Q2: 4.25M

Q3: 3.50M

9. Revenue Trend (2016-2018)

Area chart displaying yearly growth in sales revenue.

📁 Folder Structure (If applicable)
Shopnext-Store-Analysis/
│
├── PowerBI_Report/
│   └── Shopnext_Report.pbix
├── assets/
│   └── shopnext_store_project_visualization.PNG
├── data/
│   └── sales_data.csv
└── README.md

📌 Insights & Takeaways

Majority of orders are early (89K vs 7K delayed)

health_beauty and watches lead in total sales

Credit cards dominate payment preferences

Seasonal spikes observed in Q2 and Q4

Strong customer base in SP and RJ regions

🚀 How to Use

Clone this repository

Open Shopnext_Report.pbix in Power BI Desktop

Refresh data or replace with your own source

Customize visuals or measures as needed

📬 Feedback & Contributions

Found something interesting or want to contribute?
Feel free to open issues or pull requests.
