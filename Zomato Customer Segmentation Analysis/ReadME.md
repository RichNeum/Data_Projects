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
## 🔍 Key Insights

- 22% of Zomato users are classified as dormant, having never placed an order, indicating a substantial inactive user base.
- The user demographic is predominantly younger, with the average age being 25 years, 70% identifying as single, and 53% as students.
- 48% of users report no income, signifying a price-sensitive cohort with potentially low disposable income.
- The majority (68%) reside in households with 3–6 members, which suggests opportunities for family-centric marketing strategies.
- Housewives, although a smaller segment, exhibit higher average spend per capita than other groups, warranting targeted high-value offers.
- The platform experiences 99.6% of orders on weekdays, with a pronounced peak on Fridays; weekends show significantly lower transaction volumes.
- A notable drop in activity is observed between July and September, likely attributed to the academic calendar and student vacations.
- Cuisine preferences are dominated by Indian, Chinese, and hybrid Indian/Chinese offerings, indicating a preference for these cuisines.
- Major Quick Service Restaurants (QSRs) such as Domino’s and KFC show strong performance metrics where brand-specific data is available.

## 💡 Strategic Opportunities

- Implement **re-engagement campaigns** to target dormant users, utilizing personalized incentives to drive reactivation.
- Develop **targeted student programs**, leveraging the high concentration of students within the user base to maximize user acquisition and retention.
- Introduce **budget-friendly meal options** to cater to the price-sensitive segment, including singles and low-income earners.
- Promote **family-oriented meal bundles** and group-based incentives to leverage the large household segment (3–6 members).
- Execute **segmentation-based marketing** focused on user occupation (e.g., self-employed, homemakers) to increase conversion rates.
- Enhance **weekday monetization** by optimizing promotional offers during peak weekdays (Friday), and address **weekend underperformance** by diversifying weekend-specific offers.
- Launch **seasonal promotions** to counter the summer lull and optimize engagement during low-traffic periods (July–September).
- Expand offerings in the **Indian/Chinese fusion cuisine** category, and implement **cuisine-specific marketing** to drive niche engagement.

## ✅ Recommended Actions

- **User Re-engagement**: Deploy personalized push notifications, first-order discounts, and reactivation campaigns for dormant users.
- **Student-Centric Campaigns**: Roll out tailored meal plans, loyalty programs, and exclusive student discounts to address the high proportion of student users.
- **Cost-Efficient Bundles**: Design and market affordable meal bundles that appeal to singles and lower-income segments, with volume-based discounts.
- **Family-Oriented Meal Bundles**: Develop combo packages and group-order incentives, highlighting value for larger households.
- **Behavioral Segmentation**: Leverage user occupation and spending patterns to deliver hyper-targeted promotions and customized marketing content.
- **Weekday Promotions**: Optimize the Friday peak by offering exclusive weekday-only deals, loyalty rewards, and limited-time discounts.
- **Weekend Incentives**: Introduce curated weekend-specific offers, such as weekend-only discounts or exclusive meal kits, to boost weekend sales.
- **Seasonal Campaigns**: Develop summer-themed offerings and reward continuous engagement to mitigate seasonal declines in usage.
- **Cuisine-Focused Marketing**: Implement weekly promotional campaigns focused on popular cuisines like “Top Indian Picks” or “Fusion Feast,” driving awareness and engagement.

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

## 🔗 View the Interactive Dashboard

## 👉 [View on Power BI Website](https://app.powerbi.com/groups/me/reports/a8a50495-dd51-4271-ac55-6fe857b3a3c9/9daf7eb0c18c6c28680e?experience=power-bi)
---

## 📫 Contact

Want to collaborate or have questions about the project?  
Feel free to connect via [linkedin] (www.linkedin.com/in/richard-neumann) or GitHub!


