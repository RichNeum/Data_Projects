# 🍽️ Zomato Customer Segmentation & Behavioral Analysis (Power BI Project)

## 📊 Project Overview

This Business Intelligence project leverages Zomato user data to uncover key patterns in customer behavior, enabling data-driven recommendations to optimize customer retention, increase engagement, and boost revenue.

Utilizing **Power BI**, the project explores user demographics, behavioral KPIs, and RFM segmentation to deliver actionable insights through interactive dashboards.

---

## 📁 Table of Contents

- [Project Goals](#project-goals)
- [Key Assumptions](#key-assumptions)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Dashboards](#dashboards)
  - [Demographics Dashboard](#1-demographics-dashboard)
  - [Customer KPI Dashboard](#2-customer-kpi-dashboard)
  - [RFM Analysis Dashboard](#3-rfm-analysis-dashboard)
- [Key Insights](#key-insights)
- [Strategic Opportunities](#strategic-opportunities)
- [Recommendations](#recommendations)
- [Tech Stack](#tech-stack)
- [Author](#author)

---

## 🎯 Project Goals

- Analyze customer data to identify meaningful behavioral and demographic patterns.
- Segment users using RFM (Recency, Frequency, Monetary) analysis.
- Uncover key metrics related to user activity, engagement, and loyalty.
- Deliver strategic business recommendations to improve retention and increase revenue.

---

## 🔍 Key Assumptions

- Assumption1: There were two outliers in the "currency" column of the orders table which were formatted in USD instead of INR. USD amounts were converted to INR at a rate of $1 USD: 83 INR which is approximately the exchange rate in the timeframe the data was presented. A new INR-converted sales column was created to ensure consistency across all financial metrics.
- Assumption 2: For demographic data all users were accounted for from the "users" table. In any metrics or KPI calculated only active users from the "orders" table were included (those with at least one order). 
- Assumption 3: For RFM Metrics, scores were determined by meeting certain criteria based on average values gained from KPI's, they are as follows:
"Recency Score" (Days since last order) <= 7: 5, <= 14: 4, <= 30: 3, <= 60: 2, all others: 1.
"Frequency Score" (Total amount of orders placed by user) >= 8: 5, >= 6: 4, >= 4: 3, >= 2: 2, all others: 1.
"Monetary Score" (Total amount of money spent) >= $12,000: 5, >= $8,000: 4, >= $4,000: 3, >= $2,000: 2, all others: 1. 
"RFM Score" = (Recency Score + Frequency Score + Monetary Score) 
"RFM Score" categories fall into >= 12: "VIP", >= 10: "Loyal Customers", >= 7: "Dormant Potentials", >= 4: "Occasional Browser", all others: "At Risk" 
  

---

## 🧹 Data Cleaning & Preparation

- Removed null or missing values in key fields.
- Standardized date and currency formats.
- Transformed categorical values for consistency (e.g., gender, location).
- Engineered RFM features:
  - **Recency**: Days since last purchase.
  - **Frequency**: Total number of orders.
  - **Monetary**: Total spending.

---

## 📊 Dashboards

### 1. Demographics Dashboard

Highlights:
- Gender distribution
- Age group breakdown
- total sales by Occupation breakdown 
- Family size distribution
- 

**Use case**: Identify high-value demographics for targeted marketing campaigns.

---

### 2. Customer KPI Dashboard

Tracks key behavioral metrics:
- Average Order Value (AOV)
- Retention Rate
- Lifetime Value (LTV)
- Time Between Purchases
- Day and Monthly activity trends

**Use case**: Monitor user health and purchasing habits over time.

---

### 3. RFM Analysis Dashboard

Visualizes segmentation based on:
- **Recency** (R)
- **Frequency** (F)
- **Monetary** (M)

Segments users into personas:
- VIP
- Loyal Customers
- Occasional Browsers
- At Risk
  

**Use case**: Tailor retention strategies and promotions for each segment.

---

## 🔎 Key Insights

- **Loyal Users**: Clustered around specific regions and age groups (25-34).
- **Gender Trends**: Males showed higher frequency of orders; females had higher AOV.
- **Dormant Users**: High-value customers with declining engagement in recent months.
- **High LTV**: Concentrated among users in RFM category "loyal customers" with frequent and recent purchases.

---

## 🚀 Strategic Opportunities

- **Retention Campaigns**: Target “At Risk” and “Occasional Browsers” segments with win-back offers.
- **Loyalty Programs**: Incentivize repeat purchases among mid-tier customers.
- **Personalized Promotions**: Use demographic data to send targeted deals.
- **Optimize AOV**: Bundle offerings or upsell during checkout to boost transaction value.

---

## ✅ Recommendations

- Develop re-engagement campaigns for inactive high-spending users.
- Launch targeted referral programs focused on top-performing segments.
- Use segmentation to tailor email marketing and push notifications.
- Monitor RFM scores monthly to proactively manage churn risk.

---

## 🧰 Tech Stack

- **Power BI** – Data modeling, dashboard development, and visualization.
- **Microsoft Excel** – Initial data cleaning and exploration.
- **DAX** – Custom metrics, KPIs, and logic for interactive visuals.

---

## 👤 Author

**[Richard Neumann]**  
Business Intelligence & Data Analyst  
📍 New York City  
🎯 Passionate about using data to drive strategic decisions in tech, healthcare, and government.

---

## 📫 Contact

Want to collaborate or have questions about the project?  
Feel free to connect via [linkedin] (www.linkedin.com/in/richard-neumann) or GitHub!


