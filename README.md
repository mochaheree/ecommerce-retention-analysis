# 📊 Customer Segmentation & Retention Strategy for E-commerce

## 🧠 Project Overview

This project analyzes an e-commerce customer dataset to understand customer behavior, retention patterns, and revenue distribution. The objective is to generate actionable business insights and propose strategic recommendations to improve customer retention and sustainable revenue growth.

An end-to-end analytics workflow was performed:
- Data Cleaning & Processing
- Feature Engineering
- RFM Segmentation
- Revenue & Retention Analysis
- Interactive Dashboard (Google Looker Studio)

---

## 📥 Dataset Description

The dataset contains transactional and customer-level information, including:

- Customer ID  
- Purchase Date  
- Product Category  
- Product Price  
- Quantity  
- Total Purchase Amount  
- Payment Method  
- Customer Age  
- Gender  
- Returns  
- Churn  

Total Records: **250,000 transactions**  
Total Customers: **49,661 customers**

---

## 🛠 Data Processing & Feature Engineering

Key steps performed:

- Handled missing values in `Returns`
- Converted `Purchase Date` to datetime
- Aggregated transaction-level data into customer-level dataset
- Created retention metrics:
  - Frequency
  - Monetary (Total Spend)
  - Recency
  - Tenure
  - Repeat Flag
  - VIP Flag (Top 20% spenders)

### Customer-Level Metrics Created

- `frequency` → total number of transactions  
- `monetary` → total customer spending  
- `avg_order_value` → average spending per transaction  
- `recency` → days since last purchase  
- `tenure_days` → customer lifetime duration  
- `is_repeat` → customer with more than 1 transaction  
- `is_vip` → top 20% customers based on total spend  

---

## 📊 RFM Segmentation

Customers were segmented using the RFM framework:

- **Recency (R)** → How recently the customer purchased  
- **Frequency (F)** → How often the customer purchased  
- **Monetary (M)** → How much the customer spent  

Each metric was scored using quintile-based segmentation.

This allows identification of:
- High-value loyal customers
- At-risk customers
- Low-engagement segments

---

## 📈 Key Business Insights

### 🔹 Retention Strength
- **96.67% of customers make repeat purchases**
- Repeat customers generate **~99.33% of total revenue**

This indicates strong retention but high dependency on repeat behavior.

---

### 🔹 Revenue Distribution
- Top 20% of customers contribute **~35% of total revenue**
- Revenue is relatively evenly distributed
- Growth opportunity lies in improving purchase frequency across the broader customer base

---

### 🔹 VIP Behavior
- VIP customers have:
  - Higher frequency
  - Lower recency (more recently active)
- However, non-VIP customers still contribute the majority of revenue

---

## 🚀 Strategic Recommendations

### 1️⃣ Loyalty Points Program
Implement a points-based system to increase purchase frequency without heavily relying on discounts.

**Success Metrics:**
- Increase in average monthly transactions
- Improvement in repeat rate
- Stable or increasing revenue per customer

---

### 2️⃣ Bundling Strategy
Offer product bundles to increase Average Order Value (AOV) while protecting margins.

---

### 3️⃣ Retention Monitoring
Use dashboard tracking to monitor:
- Repeat Rate
- Recency Trend
- Revenue Share by Segment
- VIP vs Non-VIP Performance

---

## 📊 Interactive Dashboard

An interactive dashboard was built using **Google Looker Studio** to visualize:

- Executive KPIs
- VIP vs Non-VIP segmentation
- Frequency distribution
- Retention metrics
- Revenue distribution

🔗 **Live Dashboard Link:**  
https://lookerstudio.google.com/reporting/97c0102a-1a5e-4f89-86af-f30770e97837

Screenshots available in the `/images` folder.

---

## 🧰 Tools Used

- Python (Pandas, NumPy)
- Google Colab
- Google Looker Studio
- GitHub

---

## 📌 Conclusion

This project demonstrates an end-to-end product analytics workflow, from raw transactional data to actionable strategic insights and interactive dashboard reporting.

The analysis highlights that while retention is strong, sustainable growth can be achieved by increasing customer purchase frequency through loyalty programs and value-driven bundling strategies.

---
