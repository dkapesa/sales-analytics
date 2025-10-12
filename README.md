🧩 Customer Segmentation & Lifetime Value Prediction for a Retail Business
📘 Project Overview

This project analyses five years of retail transaction data (2020–2025) to segment customers and forecast their Customer Lifetime Value (CLV).
The goal is to help the business optimise marketing, retention, and profitability by identifying:

Which customers generate the most value 💰

Which are most likely to churn ⚠️

How to target each segment efficiently 🎯

The project was implemented in Python (Google Colab) and includes a detailed PDF report with all findings and visuals.

📊 Dataset Overview
Feature	Description
Order ID	Unique identifier for each order
Amount	Total sale amount
Profit	Profit earned from each order
Quantity	Number of items sold
Category	Product category (e.g., Furniture, Electronics)
Sub-Category	Detailed product type
PaymentMode	Payment method used
Order Date	Date of transaction
CustomerName	Name of the customer
State / City	Delivery location
Year-Month	Month and year of transaction

📅 Data Period: March 2020 – March 2025
🧾 Records: 1,194  👥 Customers: 802  🛍 Categories: 3  📦 Sub-Categories: 12

🧠 Methodology
🔍 1. Exploratory Data Analysis (EDA)

Analysed sales trends by category, time, and location

Identified top-value customers and their profit margins

Visualised revenue concentration and customer distribution

⚙️ 2. Feature Engineering

Constructed RFM (Recency, Frequency, Monetary) metrics

Created derived features: TotalProfit, Average Order Value (AOV), Profit Margin

Standardised features for clustering and modelling

🧩 3. Customer Segmentation

Applied RFM quantile scoring → grouped customers into:

🥇 Champions

💎 Loyal Customers

🌱 Potential Loyalists

⚠️ At Risk

🕳 Lost

Performed K-Means clustering for behavioural segmentation

Used PCA for 2D visualisation of clusters

💵 4. CLV Modelling

Implemented BG/NBD model for predicting repeat purchases

Used Gamma-Gamma model to estimate average order value

Computed expected CLV (180-day horizon) per customer and segment

💬 5. Insights & Recommendations

Identified high-ROI segments (Champions & Loyal)

Flagged at-risk and lost customers for reactivation campaigns

Suggested marketing and retention strategies by segment

📈 Key Results
Segment	# Customers	Avg CLV ($)	Total CLV ($)	Avg Expected Purchases
🥇 Loyal Customers	266	4.13	1,098.78	0.0008
🌱 Potential Loyalists	288	3.11	896.99	0.0006
💎 Champions	130	5.80	753.59	0.0011
⚠️ At Risk	104	2.05	213.17	0.0004
🕳 Lost	14	1.69	23.70	0.0003

Key Findings

🧩 Loyal and Champion segments dominate both revenue and future value.

🌱 Potential Loyalists represent scalable growth potential.

💰 High-spending customers don’t always yield the highest profit margins, signalling optimisation opportunities.

⚡️ The top 20 % of customers drive roughly 65 % of all revenue.

📊 Example Visualisations

📈 Revenue Trend Over Time

🔥 Top 10 Customers by Total Spend

🧮 Revenue Distribution Histogram

💹 Profit Margin vs Total Spend Scatterplot

🎯 RFM Segment Heatmap

🌀 K-Means Cluster Visualisation (PCA)

💰 CLV Distribution by Segment

All visuals are available in the included PDF report.

💡 Business Insights

✅ Retention-first strategy: Investing in Loyal and Champion customers delivers the highest ROI.
🌱 Growth potential: Nurture Potential Loyalists via email campaigns and loyalty programmes.
⚠️ Reactivation focus: Use targeted offers for At-Risk customers.
📊 Profitability leverage: Optimise discounts for customers with low margin but high spend.
🔁 CLV-based budgeting enables smarter marketing spend allocation.

🧰 Tech Stack
Category	Tools Used
Languages	Python
Libraries	Pandas, NumPy, Scikit-learn, Lifetimes, Matplotlib, Seaborn
Environment	Google Colab
Version Control	GitHub
Reporting	PDF Report (in repository)
🚀 Future Work

🧩 Automate ETL and CLV refresh pipeline (e.g., Airflow, dbt)

🧠 Extend analysis to churn prediction and campaign attribution

📈 Integrate marketing and behavioural data for multi-channel CLV models

🖥 Deploy results to a BI dashboard (Tableau / Looker) for live tracking
