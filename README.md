# Maximizing-Revenue-Taxi-Cab-Drivers
Statistics Project On Hypothesis Testing

## 📌 Overview
  #### This project investigates whether payment method (credit card vs. cash) has a statistically significant impact on fare amounts for NYC Yellow Taxi trips.      #### Using January 2020 trip data, an A/B test was conducted to determine if encouraging card payments could meaningfully boost driver revenue.

## 🧠 Problem Statement
    In the fast-paced taxi booking sector, maximizing revenue is essential for long-term driver success. This study focuses on the relationship between payment   type and fare amount to answer:
    
    Can customers be nudged toward payment methods that generate higher revenue for drivers — without negatively impacting their experience?

## 🎯 Objective
    • Run an A/B test comparing average fares for card vs. cash payments
    • Use descriptive statistics and hypothesis testing to extract actionable insights
    • Provide data-driven recommendations for revenue optimization
  
<img width="803" height="389" alt="image" src="https://github.com/user-attachments/assets/d2fca68c-a556-485b-a819-1d829ce5f6b1" />

## 🛠️ Tech Stack
    Python — core analysis
    Pandas — data manipulation
    Matplotlib / Seaborn — visualization
    SciPy / Statsmodels — statistical testing

## 🧹 Data Cleaning Steps
    1. Parsed pickup/dropoff timestamps and derived trip duration in minutes
    2. Selected 5 relevant columns for analysis
    3. Dropped ~1% null rows in passenger_count and payment_type
    4. Filtered to payment types 1 (Card) and 2 (Cash) only
    5. Kept passenger counts between 1 and 5
    6. Removed rows with zero or negative fares, distances, and durations
    7. Dropped ~3.3M duplicate records
    8. Applied 1.5×IQR outlier removal on fare_amount, trip_distance, and duration
    
<img width="920" height="324" alt="image" src="https://github.com/user-attachments/assets/4393eaa4-fd3c-459a-a9d2-f912a78620d5" />

