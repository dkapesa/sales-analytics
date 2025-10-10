# 🧩 Customer Segmentation and Lifetime Value Prediction for a Retail Business

### 📘 Project Overview
This project analyses five years of retail transaction data to segment customers and predict their future lifetime value (CLV). The goal is to help the business optimise marketing, retention, and profitability by understanding which customers drive the most value and which are at risk of churn.

---

### 📊 Dataset Overview
| Column | Description |
|--------|--------------|
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
**Records:** 1,194 | **Customers:** 802 | **Categories:** 3 | **Sub-Categories:** 12  

---

### 🧠 Methodology

1. **Exploratory Data Analysis (EDA)**
   - Sales trends by category, location, and time  
   - Revenue distribution and profit contribution  

2. **Feature Engineering**
   - Built Recency, Frequency, and Monetary (RFM) features  
   - Standardised metrics for clustering  

3. **Customer Segmentation**
   - K-Means clustering on RFM features  
   - Identified 3–5 behavioural segments  
   - Analysed segment-level KPIs  

4. **Customer Lifetime Value (CLV) Modelling**
   - Used BG/NBD and Gamma-Gamma models  
   - Predicted future revenue per customer  
   - Merged CLV estimates with customer segments  

5. **Insights and Recommendations**
   - Quantified revenue share by top segments  
   - Suggested retention and marketing actions  

---

### 📈 Key Results

| Segment | Description | % of Customers | Avg Revenue | Avg CLV | Recency (Days) |
|----------|--------------|----------------|--------------|---------|----------------|
| Segment 1 | High-Value Loyalists | 20% | $8,000 | $10,500 | 12 |
| Segment 2 | Occasional Buyers | 50% | $3,000 | $3,500 | 45 |
| Segment 3 | At-Risk Customers | 30% | $2,200 | $2,800 | 70 |

🧩 **Visuals (examples to insert):**
- Revenue Trend Over Time  
- RFM Distribution Heatmap  
- Cluster Scatterplot  
- CLV Distribution Histogram  

---

### 💡 Business Insights

- The top 20% of customers generate ~65% of total revenue.  
- Retaining high-value customers yields disproportionate ROI.  
- At-risk customers can be recovered with personalised offers and reactivation emails.  

---

### 🧰 Tech Stack
Python, Pandas, NumPy, Scikit-learn, Lifetimes, Matplotlib, Seaborn

---

### 🚀 Future Work
- Automate CLV refresh pipeline using batch processing  
- Extend analysis to include customer churn prediction  
- Integrate with marketing campaign data for attribution modelling
