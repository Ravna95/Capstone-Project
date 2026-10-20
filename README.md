Prepared by Ravna

📊 #  DataCo Supply Chain Performance Analysis #


Improving Delivery Efficiency, Sales and Profitability Through Business Analytics


<img width="733" height="384" alt="image" src="https://github.com/user-attachments/assets/4cdca9e1-8699-4472-8b6d-2739840ff161" />




   
9 CSV Datasets · 5 Research Objectives · 3 Planned Dashboards

</div>

📌 Project Overview

This capstone project uses nine interconnected DataCo Supply Chain Analytics datasets and the accompanying Data Dictionary to examine sales trends, delivery performance, product profitability, geographic markets and customer segments. 
Python and Pandas will be used for data preparation and exploratory data analysis (EDA). 
Power BI will be used to build interactive dashboards that support business decisions.

Project type: Business Analytics


Tools: Python · Pandas · Matplotlib · Google Colab · Power BI · GitHub 

Dataset repository: [Ravna – Capstone Project](https://github.com/RavnaSrikanth/Ravna---Capstone-Project)

Link to Jupyter Notebook in Google Colab: https://colab.research.google.com/drive/1eMJr6zUDOovSVQi-Qaihhl-L1ErGP24V?usp=sharing


🧭 # Project Navigation

· Problem Statement 
· Research Objectives 
· Dataset Description 
· Methodology 
· KPIs 
· EDA 
· Power BI 
· Deliverables

🎯 2. Problem Statement

DataCo handles orders across different products, shipping modes and geographical markets. Late deliveries and low-profit transactions may affect operational efficiency and business outcomes. Without integrated reporting, it can be difficult to compare delivery performance and understand which products, customer segments and markets contribute to sales and profitability.

Main research question: How can DataCo use historical order, shipping, sales and profitability data to identify performance patterns and support improvements in supply chain decision-making?
The analysis will identify measurable patterns and opportunities; it will not assume that the available data can prove the causes of delivery delays.

📋 3. Research Objectives

The project focuses on five research objectives:

Objective 1: Analyse Overall Sales Performance
- Calculate total sales revenue and order volume.
- Examine monthly and yearly sales trends.
- Identify products and categories contributing the highest sales.
  
Objective 2: Evaluate Delivery Performance
- Calculate the percentage of late deliveries.
- Compare actual shipping days with scheduled shipping days.
- Compare delivery performance across shipping modes.
  
Objective 3: Analyse Product and Category Profitability
- Identify the most and least profitable products and categories.
- Compare revenue and profit across departments.
- Examine associations between discounts and profitability.
  
Objective 4: Evaluate Geographical Sales and Delivery Performance
- Compare revenue and profitability across markets and regions.
- Identify geographical areas with higher late-delivery rates.
- Examine regional differences in supply chain performance.
  
Objective 5: Analyse Customer Segment Performance
- Compare sales contributions across customer segments.
- Examine customer ordering patterns and purchase frequency.
- Identify segments contributing the highest revenue and profitability.
  
🗂️ 4. Dataset Description

The project uses nine CSV datasets, with record counts verified from the supplied files, and one Data Dictionary.

No.	Dataset	Records	Columns	Description

1	Customers.csv	20,652	11	Customer information and segments

2	Orders.csv	65,752	11	Order information, statuses and delivery measures

3	Order Items.csv	180,519	15	Line items, quantities, sales, discounts and profit fields

4	Products.csv	118	7	Product names, categories, prices and status

5	Categories.csv	51	3	Product category reference

6	Departments.csv	11	2	Product department reference

7	Shipping.csv	65,752	3	Shipping modes and related shipment information

8	Geography.csv	64,990	9	Markets, regions, countries and cities

9	Payment Types.csv	4	2	Payment method reference


Data Dictionary.docx documents the meaning of the fields and helps identify table relationships. Record counts represent rows in individual files, not distinct customers or orders across the entire model; they should not be added together as a business total.

🛠️ 5. Project Methodology

Phase 1: Data Collection and Understanding

- Load all nine datasets from GitHub using Python Pandas.
- Inspect columns, row counts, data types and sample records.
- Compare fields and identifiers with the Data Dictionary.
  
Phase 2: Data Cleaning and Preprocessing
- Examine missing values, duplicate records and invalid values.
- Convert date fields to suitable date/time types.
- Check key uniqueness and referential integrity.
- Exclude unnecessary customer names, addresses, email addresses and password fields from analytical outputs.
- Document all cleaning decisions instead of automatically deleting records.
  
Phase 3: Data Integration
- Relate orders to order items, customers, shipping, geography and payment methods.
- Relate products to categories and departments.
- Validate join cardinality and row counts to prevent double-counting.
- Prepare clean analytical tables for Power BI.
  
Phase 4: Exploratory Data Analysis (EDA)
- Analyse sales trends and order volumes.
- Examine late delivery rates and shipping mode performance.
- Compare profitability by product, category and department.
- Compare markets and regions.
- Evaluate customer segments and ordering patterns.
  
Phase 5: Reporting and Visualisation
- Produce explanatory Python charts.
- Build interactive Power BI dashboards with filters.
- Document verified insights and practical recommendations.
  
📈 6. Key Performance Indicators (KPIs)

KPI	Purpose
Total Sales Revenue	Overall sales performance
Total Orders	Distinct order volume
Total Profit	Overall profitability using validated profit fields
Profit Margin (%)	Profit relative to sales
Late Delivery Rate (%)	Share of orders classified as late
Average Actual Shipping Days	Observed shipping duration
Average Scheduled Shipping Days	Planned shipping duration
Sales by Category	Product category contribution
Sales by Market	Geographical contribution
Sales by Customer Segment	Segment contribution


Calculation note: Profit fields and order-level measures will be checked against the Data Dictionary and their actual values before aggregation. A line-item table can repeat order-level values, so naive sums may overstate results.

🔍 7. Exploratory Data Analysis

7.1 Sales Performance
Evaluate revenue, distinct order volume, trends and high-performing products and categories.

7.2 Delivery Performance
Evaluate delivery statuses, late-delivery rates and actual versus scheduled shipping duration.
7.3 Shipping Mode Efficiency

Compare late-delivery rates and shipping durations by shipping mode.

7.4 Product and Category Profitability
Compare profit and revenue across products, categories and departments; explore discount relationships.

7.5 Geographical Performance
Compare sales, profit and delivery outcomes across markets and regions.

7.6 Customer Segments
Compare sales, order frequency and profitability by customer segment.

📊 8. Power BI Dashboard Development

Dashboard 1 — Sales and Profitability: Total sales, total orders, total profit, profit margin, sales trends, product/category comparisons and department performance.
Dashboard 2 — Shipping and Delivery: Late-delivery rate, delivery status, actual versus scheduled shipping days, shipping-mode comparisons and trends.
Dashboard 3 — Customer and Geography: Customer-segment revenue, purchase frequency, market sales, regional profitability and delivery comparisons.

Dashboards will provide interactive filters for relevant dates, markets, product categories and customer segments. Dashboard development is a project deliverable rather than a separate research objective.

💡 9. Key Findings and Business Insights
To be completed after analysis. Each finding will state the calculation, supporting chart or table, business interpretation and any relevant limitations. No results from reference projects will be copied.

✅ 10. Business Recommendations
To be finalised after analysis. Recommendations may address recurring delivery delays, shipping-mode performance, low-profit products and categories, regional differences, customer segment reporting and management visibility. Only recommendations supported by verified findings will be presented as conclusions.

⚠️ 11. Project Limitations
- Historical results may not reflect current business conditions.
- Missing geographical values may limit regional comparisons.
- Delivery status and late-delivery risk must be interpreted consistently.
- Profit fields may exist at different transaction levels and require careful aggregation.
- Observed relationships do not establish the causes of delays or profit differences.
  
🌱 12. Future Improvements and Project Reflection
12.1 Future Improvements
- Delivery monitoring: Extend reporting to highlight recurring late-delivery patterns.
- Predictive analytics: Consider a future model to estimate late-delivery risk, with proper validation.
- Profitability analysis: Investigate discounts, product performance and margin patterns in more detail.
- Dashboard automation: Explore scheduled refreshes when a suitable regularly updated data source is available.
- Customer analysis: Extend customer-segment and purchase-frequency reporting.
  
12.2 Project Reflection
This capstone offers an opportunity to apply Python, data cleaning, data integration, EDA and Power BI skills to supply chain data. The final reflection will describe what was learned, what challenges were encountered and how they were resolved after the project is completed.
12.3 Future Learning Goals

Develop stronger skills in Python, SQL and Power BI to improve business analytics, reporting and decision support.

🏁 13. Conclusion

The project aims to transform nine related DataCo datasets into a structured analysis of sales, delivery efficiency, profitability, geography and customer segments. Final conclusions will be written after the findings are validated and presented in Python and Power BI.

📦 14. Project Deliverables

- Jupyter Notebook (.ipynb) containing data preparation, analysis and charts.
- Power BI report (.pbix) containing interactive dashboards.
- Nine source CSV files and Data Dictionary (.docx).
- Project README (.md) documenting methodology and findings.
- Final PowerPoint presentation (.pptx).
- Practical Performance project ZIP for submission, with PowerPoint submitted separately according to course instructions.
Project status: Planning and data-understanding stage.
Next step: Validate dataset fields, relationships and data quality in Google Colab.

