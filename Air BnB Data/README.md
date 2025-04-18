# 🗽 Airbnb Manhattan Vacation Rentals Analysis (Excel Project)

## 📊 Project Overview

This Business Intelligence project analyzes Airbnb vacation rental data in **Manhattan, NYC**, using **Excel**. The objective is to identify pricing trends, optimize host strategies, and improve booking efficiency. The analysis includes location-based pricing, availability patterns, and host performance, with interactive dashboards built for strategic insights.

---

## 📁 Table of Contents

- [Project Goals](#-project-goals)  
- [Data Source](#-data-source)  
- [Key Assumptions](#-key-assumptions)  
- [Data Cleaning](#-data-cleaning)  
- [Neighborhood Analysis](#-neighborhood-analysis)  
- [Property Size Analysis](#-property-size-analysis)  
- [Revenue Analysis](#-revenue-analysis)  
- [Additional Analysis](#-additional-analysis)  
- [Data Visualization](#-data-visualization)  
- [Findings & Recommendations](#-findings--recommendations)  
- [Tech Stack](#-tech-stack)  
- [Author](#-author)  
- [Contact](#-contact)

---

## 🎯 Project Goals

- Analyze price variations across Manhattan neighborhoods.  
- Examine availability and occupancy rates to identify underutilized listings.  
- Understand host behavior and listing performance.  
- Provide recommendations to increase visibility, occupancy, and revenue.

---

## 🌐 Data Source

- **Dataset**: Airbnb Manhattan Vacation Rentals  
- **Columns Include**:  
  - `id`, `name`, `host_id`, `neighbourhood_group`, `neighbourhood`  
  - `room_type`, `price`, `minimum_nights`, `number_of_reviews`  
  - `reviews_per_month`, `availability_365`, `calculated_host_listings_count`

---

## 🔍 Key Assumptions

- Only properties with a **minimum night requirement** of 7 days or less were considered.  
- Properties with **no reviews in the last 12 months** were considered inactive.  
- Reviews reflect rental frequency; used `number_of_reviews_ltm` to measure a listing's attractiveness.  
- **Super luxury listings** (price > $1,321.21) and **extremely low-priced listings** (< $85.28) were filtered out as outliers.  
- **Building staff** refers to listings with **doormen**.

---

## 🧹 Data Cleaning

- Removed duplicates and null values.  
- Filtered out listings with `price = 0` and `minimum_nights > 365`.  
- Converted key fields to numerical types.  
- Applied functions like `PROPER`, `TRIM`, `IF`, `ISNUMBER`, `FIND`, `ROUND`, `SUMIF`, `VLOOKUP`, `CHOOSE`, and `WEEKDAY` for data tidying.

---

## 🏙️ Neighborhood Analysis

- **Top 10 neighborhoods** based on profitability and rental demand:
  1. Lower East Side  
  2. Hell's Kitchen  
  3. Harlem  
  4. Midtown  
  5. Upper West Side  
  6. Chelsea  
  7. East Village  
  8. East Harlem  
  9. West Village  
  10. Upper East Side  

---

## 🏘️ Property Size Analysis

- **Most popular property size**:
  - **1-bedroom** listings dominate all neighborhoods except **Midtown**, which favors **studio** properties.
  - The listings which matched the criteria for most popular properties in the top 10 neighborhoods generated a grand total of **$5,474,281.00**, with the 10 highest earning listings generating      between **$13,500** to **$29,940.00** in the prvious 12 months.
---

## 💰 Revenue Analysis

- **Estimated annual revenue** for the top properties: **$69,957**  
- Focus investments on **1-bedroom properties** in the top 10 neighborhoods (excluding Midtown, where studios perform best).

---

## 📊 Additional Analysis

- **Occupancy Rates**: Fridays had the highest occupancy rate at **86.4%**.  
- **Instant Bookings**: Listings with **instant booking** had a significantly higher occupancy rate, averaging **52%**.  
- **Superhosts**: Can charge higher prices (**$334** on average) with statistically significant occupancy.  
- **Doormen**: Buildings with doormen received statistically significant higher review ratings (**+0.05 stars**).  
- **Price by Review Ratings**: Listings with higher review ratings can charge higher prices, with a clear correlation.

---

## 📊 Data Visualization

- Created visualizations to highlight:
  - **Price by neighborhood and room type**  
  - **Occupancy trends by day of the week**  
  - **Revenue potential** for top-performing listings  
  - **Price vs. review ratings** correlation

---

## 📌 Findings & Recommendations

### Key Insights:
- **Top neighborhoods for vacation rentals**: Lower East Side, Hell's Kitchen, Harlem, Midtown, Upper West Side, Chelsea, East Village, East Harlem, West Village, and Upper East Side.
- **Most popular property size**: 1-bedroom (except Midtown, which prefers studios).
- **Estimated annual revenue**: Based on top listings, estimated at **$69,957** per year.

### Strategic Opportunities:
- **Focus on 1-bedroom properties** in the top 10 neighborhoods for highest profitability, except in Midtown, where studios perform best.
- **Encourage instant bookings** to capitalize on higher occupancy rates.
- **Target superhosts** for premium pricing and higher revenue potential.
- **Consider investing in buildings with doormen**, as they tend to get better reviews and higher occupancy rates.

---

## 🧰 Tech Stack

- **Microsoft Excel**  
  - Pivot Tables  
  - Slicers & Timelines  
  - Conditional Formatting  
  - Interactive Charts  
  - Power Query for preprocessing

---

## 👤 Author

**Richard Neumann**  
Business Intelligence & Data Analyst  
📍 New York City  


---

## 📫 Contact

💼 [LinkedIn](https://www.linkedin.com/in/richard-neumann)  


