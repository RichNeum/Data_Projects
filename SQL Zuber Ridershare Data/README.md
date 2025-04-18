# 📦 Zuber Database Analysis (SQL Project)

## 📊 Project Overview

This Business Intelligence project focuses on analyzing taxi ride data to uncover patterns in passenger preferences and the impact of external factors on rides. The primary objective is to examine the effect of weather, specifically rainy Saturdays, on the duration of rides from the Loop to O'Hare International Airport. 

The project uses **SQL** to query and manipulate large datasets, providing insights on ride counts, taxi company performance, and the impact of weather on ride durations. The goal is to understand trends and provide actionable recommendations for taxi companies and city planners.

---

## 📁 Table of Contents

- [Project Goals](#-project-goals)  
- [Key Assumptions](#-key-assumptions)  
- [Data Cleaning & Preparation](#-data-cleaning--preparation)  
- [Findings](#-findings)  
- [Tech Stack](#-tech-stack)  
- [Author](#-author)

---

## 🎯 Project Goals

- Investigate the effect of weather conditions on taxi ride duration between the Loop and O'Hare.
- Analyze taxi ride data to identify trends in company performance and passenger preferences.
- Compare ride data across different taxi companies and assess the impact of weather on rides.
- Explore the relationship between ride duration and weather patterns, specifically rainy Saturdays.

---

## 🔍 Key Assumptions

- There isn't a direct connection between the `trips` table and the `weather_records` table in the database.
- Each table uses unique primary keys: `neighborhood_id` for neighborhoods, `cab_id` for cabs, `trip_id` for trips, and `record_id` for weather records.
- Weather conditions are categorized by hour in the `weather_records` table.
- Taxi ride data is analyzed for specific time frames, focusing on high-traffic periods like weekends.

---

## 🧹 Data Cleaning & Preparation

- Filtered and joined the relevant tables: `trips`, `cabs`, `neighborhoods`, and `weather_records`.
- Removed duplicates and handled missing values in the dataset.
- Cleaned up ride data for consistency in company names and ride durations.
- Standardized weather conditions and timestamps to ensure accurate comparisons across data sources.

---

## 🔎 Findings

- **Top Taxi Companies**: "Flash Cab" had the highest number of taxi rides for Nov. 15th-16th, 2017, with 19,558 trips. "Blue Diamond" had the highest number of taxi rides for Nov. 1st-7th, 2017, with 6,764 trips.
- **Company Comparison**: The combined ride count of "Flash Cab" and "Taxi Affiliation Services" is significantly lower than the total number of rides from other companies, indicating a high volume of rides from smaller companies.
- **Neighborhood IDs**: The `neighborhood_id` for O'Hare is 63, and for the Loop, it's 50.
- **Saturday Rides**: A SQL query was used to retrieve all rides that started in the Loop on a Saturday and ended at O'Hare, including weather conditions and ride durations.
- **Weather Analysis**: Weather conditions were categorized by the hour, with weather records linked to each ride to analyze the impact of weather on ride duration.

---

## 🧰 Tech Stack

- **SQL** – Data querying and manipulation  
- **PostgreSQL** – Database management system  
- **Microsoft Excel** – Data cleaning and initial analysis 
- **Data Visualization** – future implementation (Power BI or Tableau for reporting)

---

## 👤 Author

**Richard Neumann**  
Business Intelligence & Data Analyst  
📍 New York City  
🎯 Focused on solving complex business problems with data and analytics, especially in tech, retail, and government.

---

## 📫 Contact

Want to collaborate or have questions about the project?  
Feel free to connect via [LinkedIn](https://www.linkedin.com/in/richard-neumann) or check out more on GitHub!

