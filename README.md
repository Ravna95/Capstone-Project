
<img width="733" height="384" alt="image" src="https://github.com/user-attachments/assets/4cdca9e1-8699-4472-8b6d-2739840ff161" />

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

## Objective 5: Predictive Analytics (Linear Regression for Profit Prediction)

### 1. Objective & Methodology
To answer how operational factors and financial metrics influence profitability, implemented a **Multiple Linear Regression** model.
* **Dependent Variable ($Y$):** `Order Profit Per Order` (Net profit per transaction)
* **Independent Variables ($X$):**
  * **Categorical Features (One-Hot Encoded):** Shipping Method, Customer Segment, Order Country, and Product Category.
  * **Continuous Numerical Features:** Total Sales, Order Item Discount Rate, Order Item Quantity, and Product Price.

---

### 2. Model Performance & Output
* **R-squared ($R^2$ Score):** `0.0206` (or ~2.1%) 
* **Root Mean Squared Error (RMSE):** `$100.34`

---

### 3. Explanation of Results & Observations
* **What the $R^2$ Score Means:** 
  The model achieved an $R^2$ score of roughly 2.1%. This indicates that while operational factors (like shipping mode or customer segment) provide high-level context, transaction-level financial metrics (such as exact sales amounts and discount rates) are required to capture the full picture of order profitability.
* **The Role of Financial Drivers:** 
  By combining categorical attributes with numerical transaction drivers, the model successfully accounts for variance driven by revenue and discounting behavior.
* **Business Takeaway:** 
  For DataCo to maintain strong profit margins, management cannot rely solely on broad categories (like customer type or shipping method). Instead, they must actively control transaction-level levers—specifically **discount rates** and **sales pricing strategies**—to prevent margin erosion and avoid unprofitable shipments.
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

<img width="1083" height="667" alt="image" src="https://github.com/user-attachments/assets/45624eec-2b01-4489-8f61-a8309901a9e4" />


## 📈 Executive Summary & Key Metrics

* **Total Sales:** $36.78M (Gross revenue generated across the dataset)
* **Total Orders:** 65.75K (Distinct customer orders processed, averaging ~$560 per order)
* **Total Profit:** $3.97M (Net benefit/profit after costs)
* **Profit Margin:** ~12% (Stable and healthy operational return)

---

## 📅 Visualizations & Dashboard Components

### 1. Headline KPI Cards (Top Section)
* Four summary cards providing an instant view of **Total Sales**, **Total Orders (Distinct Count)**, **Total Profit**, and **Profit Margin**.

### 2. Sales Trends (Line Chart)
* **Seasonal Peak:** Sales reach their annual high in **January (~$3.46M)** due to post-holiday demand.
* **Stable Period:** Monthly sales remain steady between **$3.1M and $3.2M** from March through October.
* **Year-End Dip:** Noticeable decrease in November and December (~$2.6M–$2.7M), highlighting potential end-of-year fulfillment or stock constraints.

### 3. Category Performance (Bar Chart)
* **Top Revenue Drivers:** **Fishing ($6.93M)**, **Cleats ($4.43M)**, and **Camping & Hiking ($4.12M)** dominate product sales.
* **Low Performers:** Minor product categories (Books, Golf Bags, Toys, CDs) generate under $15K each, contributing minimally to total revenue.

---

## 💡 Key Takeaway & Strategic Recommendations
> *"Our supply chain is highly profitable and driven primarily by sports and outdoor equipment. To maximize future growth, operations should prioritize inventory availability for top categories (like Fishing and Cleats) to prevent stockouts during peak seasons, while reviewing low-demand catalog items to optimize warehouse space and working capital."*



## Dashboard 2: Shipping Performance

- Profit by Shipping Mode
- Shipping Cost Efficiency
- Discount Analysis
- Delivery Performance

<img width="977" height="631" alt="image" src="https://github.com/user-attachments/assets/839bb71e-ea7a-4d85-97af-ee7cc331fd2a" />
## 🚚 Shipping Performance Overview

### 1. Profit & Sales by Shipping Mode
* **Standard Class Dominance:** Standard Class handles the vast majority of our total sales volume (~$20M+) and generates the highest net profit (~$2.5M).
* **Express & Priority (Second Class, First Class, Same Day):** While smaller in overall volume, these premium options provide steady supplementary revenue and profit streams.

### 2. Discount Impact Analysis
* **Higher Discounts, Lower Returns:** Profit peaks when discount rates are low (0.0 to 0.05). As discount rates increase, overall profitability gradually declines, indicating that steep discounts erode margins without proportional profit gains.

### 3. Delivery Performance Breakdown
* **Fulfillment Status:** The donut chart shows that the vast majority of our orders are shipped on time, in advance, or via standard delivery, with only a small percentage experiencing late delivery risk or cancellations.

---

### 💡 Shipping Key Takeaway
> *"Standard Class is our primary driver for both sales volume and profit. Furthermore, while discounts attract initial interest, keeping discount rates minimal preserves our net profit margins. Maintaining reliable delivery standards for our top shipping modes will keep customer satisfaction high while protecting profitability.




## Dashboard 3: Customer & Geography Analysis

- Customer Segment Revenue
- Purchase Frequency
- Market Sales
- Regional Profitability

---
<img width="983" height="604" alt="image" src="https://github.com/user-attachments/assets/06b7f7c4-de06-4d0c-8718-1d5d781c5778" />

---

## 🌍 Customer & Geography Analysis Overview

### 1. Customer Segment Revenue
* **Consumer Leadership:** The **Consumer** segment is our primary revenue driver (~$19M+ in total sales), followed by **Corporate** (~$11M) and **Home Office** (~$6M).

### 2. Market Sales & Order Volume
* **Top Geographic Markets:** **Europe** and **LATAM** lead in both total sales volume (~$10M+ each) and overall order count (~18K+ orders each).
* **Pacific Asia & USCA:** **Pacific Asia** demonstrates strong revenue (~$8M) and high order activity, while **USCA** and **Africa** represent steady growth opportunities.

### 3. Country Profitability Breakdown
* **Top Profit Drivers:** The **United States (Estados Unidos)** generates the highest net profit by a significant margin (~$0.54M), followed by **France (Francia)** (~$0.33M) and **Mexico (México)** (~$0.30M).
* **High-Margin Regions:** **Germany (Alemania)** and **Brazil (Brasil)** round out the top 5 most profitable country markets.

---

### 💡 Geography Key Takeaway
> *"The Consumer segment forms our core customer base across all global operations. Europe and LATAM drive the highest overall market volume, while key countries such as the United States, France, and Mexico generate the largest net profits. Strategic expansion and marketing efforts should continue to prioritize high-margin country markets to maximize profitability."*


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

# Key Findings & Business Insights

## Objective 1: Shipping Mode Analysis

### Visualizations
- Horizontal Bar Chart: Average Profit Margin (%) by Shipping Mode
- Bar Chart: Total Profit ($) by Shipping Tier

### Key Finding
**Standard Class is the dominant profitability driver.**

| Shipping Mode | Average Profit Margin |
|--------------|---------------------|
| Standard Class | ~16.2% |
| Second Class | ~14.8% |
| First Class | ~11.5% |
| Same Day | ~8.2% |

Fast shipping options generate lower profitability because higher fulfillment costs reduce unit profit.

---

## Objective 2: Discount Impact Analysis

### Visualizations
- Line Chart: Profit Margin (%) across Discount Rates (0%–25%)
- Grouped Bar Chart: Profit Margin by Discount Level and Shipping Tier

### Key Finding
**Promotional discounts are a major cause of margin erosion.**

When discounts exceed **15%** on **First Class** or **Same Day** shipments, average net profit per order becomes negative.

**Business Insight:** Deep discounts combined with expensive shipping methods significantly reduce profitability.

---

## Objective 3: Product Category Analysis

### Visualizations
- Bar Chart: Top 10 Most vs. Least Profitable Categories
- Stacked Bar Chart: Department Sales vs. Department Profit

### Key Finding
**Profitability varies significantly across product categories.**

Heavy-item categories such as:
- Fishing
- Cleats

show substantially lower profit margins when shipped via Same Day delivery compared with lightweight products.

**Business Insight:** Shipping strategy should be optimized according to product characteristics.

---

## Objective 4: Customer Segment Analysis

### Visualizations
- Donut Chart: Profit Contribution (%) by Customer Segment
- Clustered Bar Chart: Average Order Spend by Segment

### Key Finding
**Customer segments exhibit minimal profitability differences.**

| Segment | Average Profit Margin |
|----------|----------------------|
| Consumer | ~13.5% |
| Corporate | ~14.1% |
| Home Office | ~13.8% |

Profitability is influenced more by operational decisions such as shipping mode and discount strategy than customer type.

---

## Objective 5: Temporal & Seasonal Analysis

### Visualizations
- Line Chart: Monthly Sales Revenue vs Net Profit
- KPI Cards:
  - Total Revenue
  - Total Profit
  - Overall Margin %

### Key Finding
**Profit margins remain relatively stable throughout the year.**

- Overall net margin remains around **14%**
- Minor declines occur during year-end promotional periods
- No major seasonal profitability fluctuations observed

---

# Overall Takeaway

The primary cause of lower order profitability is:

✅ Expensive fast-shipping options (Same Day and First Class)

✅ Excessive promotional discounts

These factors have a significantly greater impact on profitability than customer segment or geographic location.

---

# Additional Observation

## Payment Type Analysis

A supplementary analysis shows minor profitability differences across payment methods.

- Debit Card and Bank Transfer transactions tend to generate slightly higher net margins.
- Cash payments produce relatively lower margins due to additional processing and operational costs.

### Recommendation
Prioritize:
1. Standard Class Shipping
2. Controlled Discount Policies (<15%)
3. Shipping Method Optimization by Product Category
4. Cost-Efficient Payment Methods

These strategies can improve overall profitability while maintaining customer satisfaction.

