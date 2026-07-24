# 🚲 Cyclistic Bike-Share Analysis Case Study

## 📌 Executive Summary
This case study is part of the **Google Data Analytics Professional Certificate**. The primary objective is to analyze historical trip data from **Cyclistic**, a bike-share company in Chicago, to understand how **annual members (`member`)** and **casual riders (`casual`)** use bikes differently. 

The ultimate business goal is to provide data-driven recommendations for the marketing team to design targeted strategies to convert casual riders into annual members.

* 📊 **Interactive Dashboard:** [View Tableau Public Dashboard](https://public.tableau.com/app/profile/razaz.omer4799/vizzes)

---

## 🛠️ Tools & Technologies Used
* **Google BigQuery (SQL):** Data merging (over 6.6M rows across 12 months), data cleaning, feature extraction, and exploratory analysis.
* **Tableau Public:** Data visualization and interactive dashboard design.
* **Markdown:** Project documentation and report structuring.

---

## 🧹 Data Cleaning & Processing (SQL Steps)
1. **Data Union:** Combined 12 individual CSV datasets into a single unified table using `UNION ALL`.
2. **Feature Engineering:**
   * Calculated ride duration in minutes (`ride_length_minutes`) using `TIMESTAMP_DIFF`.
   * Extracted the day of the week (`day_of_week`) and month (`month`).
3. **Data Filtering:** Removed anomalous records (rides shorter than 1 minute or longer than 24 hours).

---

## 📊 Key Analytical Insights

| Analysis Dimension | Casual Riders (`casual`) | Annual Members (`member`) |
| :--- | :--- | :--- |
| **Total Trips Share** | **37%** (~2.27M trips) | **63%** (~4.01M trips) |
| **Weekly Peak Usage** | **Weekends** (Saturday & Sunday) | **Weekdays** (Tuesday - Thursday) |
| **Seasonal Trends** | Peaks sharply during Summer; drops significantly in Winter | Steady activity year-round with moderate Summer increase |
| **Bike Type Preference** | High preference for **Electric Bikes** | Strong preference for **Electric Bikes**, followed by Classic |

---

## 💡 Data-Driven Marketing Recommendations

1. **Weekend-Specific Memberships:** Introduce a flexible "Weekend Pass / Membership" targeting casual riders who predominantly use the service on Saturdays and Sundays.
2. **Seasonal Marketing Campaigns:** Focus promotional conversion offers during late Spring and early Summer (May – July) when casual user activity is at its peak.
3. **Electric Bike Incentives:** Offer exclusive discounts or free extra minutes on electric bikes upon signing up for an annual membership.

---
*Created by Razaz Omer*
