🧩 Customer Segmentation and Lifetime Value Modelling in Retail
📘 Project Overview

This project analyses five years of retail transaction data (2020–2025) to segment customers and estimate their Customer Lifetime Value (CLV) using interpretable, business-oriented analytics. The objective is to identify high-value customer groups, forecast their future revenue potential, and generate actionable recommendations for retention, upselling, and marketing prioritisation.

The full project was implemented in Python (Google Colab) and documented in a comprehensive report available in the repository.

📊 Dataset Overview
Column	Description
Order ID	Unique identifier for each order
Amount	Total sale amount
Profit	Profit earned from each order
Quantity	Number of items sold
Category	Product category (e.g., Furniture, Electronics)
Sub-Category	Detailed product type
PaymentMode	Payment method used
Order Date	Date of transaction
CustomerName	Name of customer
State / City	Delivery location
Year-Month	Month and year of transaction

Data Period: March 2020 – March 2025
Records: 1,194 | Customers: 802 | Categories: 3 | Sub-Categories: 12

🧠 Methodology
1. Exploratory Data Analysis (EDA)
- Analysed total customers and revenue trends
- Identified top 10 high-value customers
- Visualised distribution of revenue and profit margin vs total spend
- Highlighted skewed revenue concentration among a small elite group

2. Feature Engineering
- Derived RFM (Recency, Frequency, Monetary) metrics
- Calculated TotalProfit, Average Order Value (AOV), and Profit Margin
- Standardised metrics for modelling

3. Customer Segmentation
- Applied RFM quantile scoring (Champions, Loyal, Potential Loyalists, At Risk, Lost)
- Performed K-Means clustering for deeper behavioural patterns
- Visualised clusters via PCA for interpretability

4. CLV Modelling
- Fitted BG/NBD model for expected repeat purchases (180-day horizon)
- Integrated Gamma-Gamma model (where applicable) for order value estimation
- Aggregated CLV results by segment for actionable business insights

5. Insights & Recommendations
- Prioritised Champions and Loyal Customers for retention investment
- Identified Potential Loyalists as scalable growth opportunities
- Recommended low-cost automation for reactivating at-risk segments

📈 Key Results
Segment	Customers	Avg CLV ($)	Total CLV ($)	Avg Expected Purchases
Loyal Customers	266	4.13	1,098.78	0.0008
Potential Loyalists	288	3.11	896.99	0.0006
Champions	130	5.80	753.59	0.0011
At Risk	104	2.05	213.17	0.0004
Lost	14	1.69	23.70	0.0003

Key Findings:
- Most customers are single-purchase buyers, limiting short-term CLV.
- Loyal Customers and Champions drive the largest revenue and CLV contribution.
- Potential Loyalists are the largest cohort and the best opportunity for scalable growth.
- High spend ≠ high profit margin, indicating opportunity for margin optimisation.

📊 Visualisations (Included in Report)

Total Revenue vs Customer Count

Top 10 Customers by Spend

Revenue Distribution Histogram

Profit Margin vs Total Spend Scatterplot

Customer Segments by RFM Score

K-Means Cluster Visualisation (PCA)

CLV Distribution by Segment (Boxplot)

💡 Business Insights

The top 20% of customers account for a disproportionate share of total revenue.

Retention-focused marketing for Loyal and Champion segments yields the highest ROI.

Automation and targeted incentives can convert Potential Loyalists into repeat buyers.

CLV-based budgeting allows dynamic reallocation of marketing spend toward high-value customers.

🧰 Tech Stack

Languages & Libraries: Python, Pandas, NumPy, Scikit-learn, Lifetimes, Matplotlib, Seaborn
Environment: Google Colab
Report & Versioning: Google Docs → PDF, GitHub

🚀 Future Work

Automate the ETL and CLV refresh pipeline (e.g., using Airflow/dbt)

Extend analysis to churn prediction and campaign attribution

Integrate marketing and behavioural data for multi-channel CLV modelling

Deploy CLV updates to a BI dashboard (Tableau/Looker) for real-time tracking
