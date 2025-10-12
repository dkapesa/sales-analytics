# 🧩 Customer Segmentation & Lifetime Value Prediction for a Retail Business


### 📘 Executive Summary
This project analyses **five years of retail transaction data (March 2020 – March 2025)** to segment customers and forecast their **Customer Lifetime Value (CLV)**.  
Using advanced statistical modelling and segmentation techniques, it identifies which customers drive the most value, which are at risk of churn, and how to tailor marketing and retention strategies accordingly.  
The results provide a foundation for **data-driven decision-making**, helping the business maximise revenue and customer loyalty.


### 📊 Dataset Overview

| **Column** | **Description** |
|-------------|----------------|
| Order ID | Unique identifier for each order |
| Amount | Total sale amount |
| Profit | Profit earned from each order |
| Quantity | Number of items sold |
| Category | Product category (e.g., Furniture, Electronics) |
| Sub-Category | Detailed product type |
| PaymentMode | Payment method used |
| Order Date | Date of transaction |
| CustomerName | Name of customer |
| State | State of delivery |
| City | City of delivery |
| Year-Month | Month and year of transaction |

**Data Period:** March 2020 – March 2025  
**Records:** 1,194 | **Customers:** 802 | **Categories:** 3 | **Sub-Categories:** 12  


### 🧠 Methodology

1. **Exploratory Data Analysis (EDA)**
   - Analysed sales trends by category, city, and month  
   - Examined revenue and profit distributions  
   - Identified top-value customers and key profit drivers  

2. **Feature Engineering**
   - Created **Recency, Frequency, Monetary (RFM)** metrics  
   - Derived additional metrics: `TotalProfit`, `AOV`, `ProfitMargin`  
   - Normalised features for model readiness  

3. **Customer Segmentation**
   - Applied **K-Means clustering** on RFM metrics  
   - Segmented customers into five behavioural groups  
   - Evaluated KPIs by segment (spend, frequency, recency)  

4. **Customer Lifetime Value (CLV) Modelling**
   - Implemented **BG/NBD** model for expected purchases  
   - Used **Gamma-Gamma** model for expected revenue  
   - Calculated **180-day predicted CLV** per customer and per segment  

5. **Insights & Recommendations**
   - Quantified segment-level revenue contribution  
   - Prioritised retention, reactivation, and growth strategies  


### 📈 Key Results

| **Segment** | **Customers** | **Avg CLV ($)** | **Total CLV ($)** | **Avg Expected Purchases** |
|--------------|---------------|------------------|-------------------|-----------------------------|
| Loyal Customers | 266 | 4.13 | 1,098.78 | 0.0008 |
| Potential Loyalists | 288 | 3.11 | 896.99 | 0.0006 |
| Champions | 130 | 5.80 | 753.59 | 0.0011 |
| At Risk | 104 | 2.05 | 213.17 | 0.0004 |
| Lost | 14 | 1.69 | 23.70 | 0.0003 |

**Key Takeaways:**
- Top 20% of customers generate **~65% of total revenue**
- **Champions** and **Loyal Customers** drive the highest future value
- **Potential Loyalists** show strong opportunity for growth  
- **At-Risk** and **Lost** customers need targeted reactivation strategies  


### 📊 Visualisations

Included in the PDF report:
- **Revenue Trend Over Time**  
- **Top 10 Customers by Total Spend**  
- **Revenue Distribution Histogram**  
- **Profit Margin vs Total Spend Scatterplot**  
- **RFM Segment Heatmap**  
- **K-Means Cluster (PCA) Visualisation**  
- **CLV Distribution by Segment (180 Days)**  


### 💡 Business Insights

- Retaining **Loyal** and **Champion** customers delivers the highest ROI  
- Invest in **Potential Loyalists** via loyalty rewards and email campaigns  
- Target **At-Risk** customers with time-sensitive offers  
- Optimise **profit margins** among high-spending but low-profit buyers  
- Use CLV insights to guide **marketing spend allocation** and **customer lifetime strategies**


### 🧰 Tech Stack

| **Category** | **Tools Used** |
|---------------|----------------|
| **Languages** | Python |
| **Libraries** | Pandas, NumPy, Scikit-learn, Lifetimes, Matplotlib, Seaborn |
| **Environment** | Google Colab |
| **Version Control** | GitHub |
| **Reporting** | PDF Report |


### Future Work

- Automate CLV refresh pipeline using **batch ETL (Airflow / dbt)**  
- Extend analysis to **predict churn probability**  
- Integrate **marketing and campaign attribution** data  
- Deploy **interactive BI dashboard (Looker / Tableau)**

🔗 Link to the dataset: https://www.opendatabay.com/data/consumer/7b291337-5fed-470f-a206-0dc899425db4
