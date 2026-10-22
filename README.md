Prepared by Ravna

📊 #  DataCo Supply Chain Performance Analysis #


***Optimizing Shipping Mode Profitability & Cost Efficiency Through Business Analytics***


<img width="733" height="384" alt="image" src="https://github.com/user-attachments/assets/4cdca9e1-8699-4472-8b6d-2739840ff161" />


# DataCo Supply Chain Performance Analysis
### Optimizing Shipping Mode Profitability & Cost Efficiency Through Business Analytics

**Programme:** NTUC LearningHub SCTP Associate Data Analyst  
**Project Type:** Business Analytics  
**Data Source:** DataCo Supply Chain Datasets  
**Tools:** Python, Pandas, Matplotlib, Google Colab, Power BI, GitHub

---

# 1. Project Overview

This capstone project analyzes DataCo supply chain operations using nine related datasets and a data dictionary. The study focuses on:

- Sales performance
- Shipping mode profitability
- Cost efficiency
- Product and category profitability
- Customer segment performance

Python is used for data preparation, exploratory data analysis (EDA), and machine learning, while Power BI is used to develop interactive dashboards for business decision-making.

---

# 2. Problem Statement

DataCo utilizes multiple shipping methods:

- Standard Class
- Second Class
- First Class
- Same Day

While faster shipping methods improve customer satisfaction, higher shipping costs and excessive discounts may reduce profitability.

### Research Question

**How can DataCo analyze transaction revenues, discounts, and fulfillment costs across shipping modes to identify the most profitable logistics strategies and reduce low-margin shipments?**

---

# 3. Research Objectives

## Objective 1: Analyze Overall Sales Performance

- Calculate total sales revenue and order volume.
- Examine monthly and yearly sales trends.
- Identify top-performing products and categories.

## Objective 2: Evaluate Shipping Mode Performance & Fulfillment Efficiency

- Compare actual and scheduled shipping duration.
- Evaluate shipping consistency across modes.
- Measure fulfillment efficiency.

## Objective 3: Analyze Product, Category and Department Profitability

- Identify the most profitable products.
- Identify the least profitable products.
- Compare revenue and profit across departments.
- Analyze discount impact on profitability.

## Objective 4: Analyze Shipping Mode Profitability & Cost Efficiency

- Compare revenue and profit margins across shipping modes.
- Evaluate operational cost efficiency.
- Build a predictive model to classify profitable and unprofitable shipments.

## Objective 5: Analyze Customer Segment Performance & Purchasing Patterns

- Compare sales contributions across customer segments.
- Evaluate customer profitability.
- Examine purchasing behavior and shipping preferences.

---

# 4. Dataset Description

| No | Dataset | Records | Description |
|----|----------|---------:|------------|
| 1 | Customers.csv | 20,652 | Customer information and segments |
| 2 | Orders.csv | 65,752 | Order information and delivery measures |
| 3 | Order Items.csv | 180,519 | Sales, discounts, quantities and profit |
| 4 | Products.csv | 118 | Product information |
| 5 | Categories.csv | 51 | Product category reference |
| 6 | Departments.csv | 11 | Product department reference |
| 7 | Shipping.csv | 65,752 | Shipping modes and shipment details |
| 8 | Geography.csv | 64,990 | Markets, regions, countries and cities |
| 9 | Payment Types.csv | 4 | Payment method reference |

The Data Dictionary provides field definitions and dataset relationships.

---

# 5. Project Methodology

## Phase 1: Data Collection and Understanding

- Load all datasets using Python.
- Review data structure and data types.
- Validate dataset relationships.

## Phase 2: Data Cleaning and Preprocessing

- Check for missing values.
- Remove duplicates.
- Correct invalid records.
- Convert date fields.
- Verify key integrity.

## Phase 3: Data Integration

- Merge datasets using relevant keys.
- Validate joins.
- Build analytical tables.

## Phase 4: Exploratory Data Analysis (EDA)

- Analyze sales and profit trends.
- Evaluate shipping performance.
- Study customer purchasing behavior.
- Measure discount impact.

## Phase 5: Predictive Modeling

- Build Random Forest classification models.
- Predict profitable vs unprofitable shipments.
- Evaluate model performance.

## Phase 6: Reporting & Visualization

- Create visualizations in Python.
- Develop interactive Power BI dashboards.
- Present business recommendations.

---

# 6. Key Performance Indicators (KPIs)

| KPI | Purpose |
|------|---------|
| Total Sales Revenue | Overall sales performance |
| Total Orders | Order volume |
| Total Profit | Business profitability |
| Profit Margin (%) | Relative profitability |
| Profitability by Shipping Mode | Shipping performance comparison |
| Average Discount Rate (%) | Discount analysis |
| Fulfillment Cost Efficiency Index | Cost efficiency evaluation |
| Average Actual vs Scheduled Delivery Days | Delivery performance |
| Model Accuracy (%) | Model performance |
| Precision, Recall, F1-Score | Classification performance |
| Feature Importance | Key profitability drivers |

---

# 7. Exploratory Data Analysis (EDA)

## 7.1 Sales Performance

- Revenue trends
- Order volume trends
- Top products and categories

## 7.2 Shipping Mode Profitability & Cost Efficiency

Compare:

- Revenue
- Profit
- Profit Margin
- Cost-to-Profit Ratio

across:

- Standard Class
- Second Class
- First Class
- Same Day

## 7.3 Discount Impact on Shipping Margins

Analyze relationships between:

- Discount rate
- Shipping mode
- Profit margin

## 7.4 Product and Category Profitability

Evaluate:

- Product profitability
- Category profitability
- Department performance

## 7.5 Predictive Modeling

Develop a Random Forest classifier using:

- Shipping Mode
- Discount Rate
- Product Category

Target:

- High-Margin Shipment
- Low-Margin Shipment

---

# 8. Power BI Dashboard Development

## Dashboard 1: Sales & Profitability

- Total Sales
- Total Orders
- Total Profit
- Profit Margin
- Sales Trends
- Category Performance

## Dashboard 2: Shipping Performance

- Profit by Shipping Mode
- Shipping Cost Efficiency
- Discount Analysis
- Delivery Performance

## Dashboard 3: Customer & Geography Analysis

- Customer Segment Revenue
- Purchase Frequency
- Market Sales
- Regional Profitability

---

# 9. Key Findings and Business Insights

To be completed after analysis.

Key findings will include:

- Supporting visualizations
- Calculations
- Business interpretation
- Study limitations

---

# 10. Business Recommendations

Recommendations will focus on:

- Shipping pricing strategies
- Discount optimization
- Product profitability improvement
- Regional logistics optimization
- Executive reporting enhancements

---

# 11. Project Limitations

- Historical data may not reflect current business conditions.
- Shipping costs may not represent actual carrier costs.
- Predictive models rely on historical patterns.
- Profit calculations require careful aggregation.
- Correlation does not imply causation.

---

# 12. Future Improvements

## Shipping Optimization

- Integrate real-time carrier pricing.

## Predictive Analytics

- Improve forecasting models.

## Profitability Analysis

- Conduct SKU-level analysis.

## Dashboard Automation

- Implement scheduled refresh processes.

---

# 13. Conclusion

This project transforms multiple DataCo datasets into a comprehensive analysis of sales performance, shipping profitability, cost efficiency, and customer behavior. The insights generated will support data-driven decisions that improve operational efficiency and profitability.

---

## Repository Structure
