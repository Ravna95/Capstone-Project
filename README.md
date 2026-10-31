
<img width="900" height="400" alt="image" src="https://github.com/user-attachments/assets/6772012c-b0a9-4833-9ba2-25a0f2fe004a" />


Prepared by Ravna


# DataCo Supply Chain Performance Analysis
### Optimizing Shipping Mode Profitability & Cost Efficiency Through Business Analytics

**Programme:** NTUC LearningHub SCTP Associate Data Analyst  
**Project Type:** Business Analytics  
**Data Source:** DataCo Supply Chain Datasets  
**Tools:** Python, Pandas, Matplotlib, Google Colab, Power BI, GitHub

Dataset repository: [Ravna – Capstone Project](https://github.com/RavnaSrikanth/Ravna---Capstone-Project)

Link to Jupyter Notebook in Google Colab: https://colab.research.google.com/drive/1eMJr6zUDOovSVQi-Qaihhl-L1ErGP24V?usp=sharing


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

- Compare revenue and profit contributions across customer segments.
- Evaluate order behaviors and shipping mode preferences by segment.


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

# Objective 5: Predictive Analytics (Linear Regression & Random Forest)

## 1. Objective & Methodology
To analyze how operational factors and financial metrics influence profitability, we implemented and compared two predictive modeling approaches:
- **Dependent Variable (Y):** Order Profit Per Order (Net profit per transaction)
- **Independent Variables (X):**
  - **Categorical Features (One-Hot Encoded):** Shipping Method, Customer Segment, Order Country, and Product Category.
  - **Continuous Numerical Features:** Total Sales, Order Item Discount Rate, Order Item Quantity, and Product Price.

---

## 2. Model Performance & Output

### Linear Regression Model
- **R-squared ($R^2$ Score):** 0.0206 (or approx. 2.1%)
- **Root Mean Squared Error (RMSE):** $100.34

### Model Comparison Table

| Evaluation Criteria | Linear Regression | Random Forest Regressor |
| :--- | :--- | :--- |
| **Model Type** | Parametric / Linear | Non-linear / Ensemble (Decision Trees) |
| **Interpretability** | **High:** Easy to explain exact coefficients. | **Lower (Black Box):** Harder to trace exact mathematical formulas, but highlights feature importance. |
| **Accuracy ($R^2$ Score)** | **Low (approx. 2.1%):** Struggles with complex, non-linear supply chain rules. | **High (often 80%+):** Effectively captures complex interactions and non-linear thresholds. |
| **Handling Noise** | Sensitive to outliers and multicollinearity. | Robust against outliers and irrelevant features. |

---

## 3. Explanation of Results & Observations

- **Linear Regression Insights:** The $R^2$ score of roughly 2.1% indicates that while operational factors (like shipping mode or customer segment) provide high-level context, transaction-level financial metrics are necessary to fully capture order profitability variance.
- **The Role of Financial Drivers:** Combining categorical attributes with numerical transaction drivers accounts for baseline revenue and discounting behavior. However, linear constraints limit predictive power.
- **Business Takeaway:** To maintain strong profit margins, management cannot rely solely on broad categories. They must actively control transaction-level levers—specifically discount rates and pricing strategies—to prevent margin erosion.

---

## 4. Final Conclusion & Recommendation
> *"While Linear Regression provides clear, interpretable coefficients to understand broad operational trends and direct feature weights, Random Forest Regressor is the superior model for predictive accuracy, successfully capturing non-linear cost and pricing interactions in supply chain data."*

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

<img width="1083" height="667" alt="image" src="https://github.com/user-attachments/assets/45624eec-2b01-4489-8f61-a8309901a9e4" />

## Executive Summary & Key Metrics
* **Total Sales Revenue:** $36.78M (Gross revenue generated across the dataset)
* **Total Order Volume:** 65.752K (Distinct customer orders processed)
* **Total Net Profit:** $3.97M (Net benefit/profit after costs)
* **Profit Margin (%):** 10.78% (Exact operational return rate)

---

## Visualizations & Dashboard Components

### 1. Headline KPI Cards (Top Section)
Four KPI cards displaying **Total Sales Revenue** ($36.78M), **Total Order Volume** (65.752K), **Total Net Profit** ($3.97M), and **Profit Margin (%)** (10.78%).

### 2. Sum of Sales by Month (Area / Line Chart)
* **Seasonal Peak:** Sales peak in January at $3.46M.
* **Mid-Year Performance:** Experience a mid-Q1 dip in February ($2.89M) before holding steady between $3.05M and $3.19M from March through October.
* **Year-End Decline:** Sales decline toward the end of the year in November ($2.70M) and hit a low in December ($2.60M).

### 3. Sum of Sales by Category Name (Bar Chart)
* **Top Revenue Drivers:** **Fishing** leads heavily near $7M, followed by **Cleats** (~$4.4M), **Camping & Hiking** (~$4.1M), and **Cardio Equipment** (~$3.7M).
* **Mid-to-Lower Performers:** Categories like **Shop By Sport**, **Computers**, **Electronics**, **Cameras**, **Garden**, and **Children's Clothing** generate significantly lower revenue under $1.5M each.

---

## 💡 Key Takeaway & Strategic Recommendations
> "Our business is highly profitable and driven primarily by sports and outdoor categories—led overwhelmingly by **Fishing**. To maximize future growth, operations should focus on maintaining stock availability for top-performing outdoor and fitness lines while reviewing inventory allocation for lower-volume electronics and apparel categories."


## Dashboard 2: Shipping Performance

- Profit by Shipping Mode
- Shipping Cost Efficiency
- Discount Analysis
- Delivery Performance

<img width="1154" height="684" alt="image" src="https://github.com/user-attachments/assets/06d43dd5-d79e-478b-9f30-7a7b67f53357" />


# Dashboard 2: Shipping Performance

## 1. Profit & Sales by Shipping Method
* **Standard Class Dominance:** Standard Class handles the vast majority of our total sales volume (~$7M+) and generates the highest net profit (~$0.8M).
* **Express & Priority (Second Class, First Class, Same Day):** While smaller in overall volume, these premium options provide steady supplementary revenue and profit streams.

## 2. Discount Impact Analysis
* **Higher Discounts, Lower Returns:** Profit peaks when discount rates are low (0.0 to 0.05). As discount rates increase, overall profitability gradually fluctuates downward, indicating that steep discounts erode margins without proportional profit gains.

## 3. Delivery Performance Breakdown
* **Fulfillment Status:** The donut chart (totaling 62.65K orders) shows that the majority of our orders are shipped on time, in advance, or via standard delivery, with specific tracking for late deliveries, advance shipping, shipping on time, and shipping canceled.

---

## 💡 Shipping Key Takeaway
> "Standard Class is our primary driver for both sales volume and profit. Furthermore, while discounts attract initial interest, keeping discount rates minimal preserves our net profit margins. Maintaining reliable delivery standards for our top shipping modes will keep customer satisfaction high while protecting profitability."




## Dashboard 3: Customer & Geography Analysis

- Customer Segment Revenue
- Purchase Frequency
- Market Sales
- Regional Profitability

---
<img width="1105" height="651" alt="image" src="https://github.com/user-attachments/assets/ae9f3009-f0b4-4fff-9f6f-11da4dc5cde4" />
# Dashboard 3: Customer & Geography Analysis

## 🌍 Customer & Geography Analysis Overview

### 1. Sales by Customer Segment (Bar Chart)
* **Consumer Leadership:** The **Consumer** segment is our primary revenue driver (approx. $19M in total sales), followed by **Corporate** ($11M) and **Home Office** (approx. $6.5M).

### 2. Order Volume by Market (Bar Chart)
* **Top Order Markets:** **Europe** leads in order volume (approx. 18.5K orders), closely followed by **Pacific Asia** (approx. 17.5K) and **LATAM** (approx. 17K), while **USCA** (approx. 8.5K) and **Africa** (approx. 4K) follow behind.

### 3. Total Sales by Market (Bar Chart)
* **Top Revenue Markets:** **Europe** and **LATAM** lead in total sales revenue (approx. $10.8M and approx. $10.3M respectively), followed by **Pacific Asia** ($8.3M), **USCA** ($5.1M), and **Africa** (approx. $2.3M).

### 4. Top Country Profitability (Bar Chart)
* **Top Profit Drivers:** **Estados Unidos** generates the highest net profit by a significant margin (approx. $0.54M), followed by **Francia** ($0.33M) and **México** (approx. $0.3M).
* **High-Margin Regions:** **Alemania** ($0.2M) and **Brasil** (approx. $0.19M) round out the top 5 most profitable country markets.

---

## 💡 Geography Key Takeaway
> "The Consumer segment forms our core customer base across all global operations. Europe and LATAM drive the highest overall market sales and order volume, while key countries such as the United States (Estados Unidos), France (Francia), and Mexico (México) generate the largest net profits. Strategic expansion and marketing efforts should continue to prioritize high-margin country markets to maximize profitability."

---

# 9. Key Findings and Business Insights

* **Supporting visualizations:** Dashboard 3 successfully outlines customer segments, market-level sales and orders, and top country profitability.
* **Calculations:** Total revenue contributions are distributed across three distinct customer segments and five international markets.
* **Business interpretation:** Regional demand is heavily concentrated in Europe and LATAM, while profitability is anchored strongly by the US and key European/Latin American countries.
* **Study limitations:** Analysis is constrained by regional aggregation levels and currency standardization across diverse global markets.

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

