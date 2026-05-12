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
    
<img width="950" height="461" alt="image" src="https://github.com/user-attachments/assets/96510b66-e8b6-4a90-bf1a-5f1d38932c69" />

<img width="990" height="537" alt="image" src="https://github.com/user-attachments/assets/a82fb950-5e1c-494c-b08d-e7d5885cab77" />

## 💼 Business Recommendations
    1. Promote card payments via in-app incentives or loyalty rewards for card-paying riders
    2. Ensure working card terminals in all taxis to eliminate cash-only fallback situations
    3. Display upfront fare estimates in card-enabled apps to attract higher-spending passengers
    4. Track payment-type KPIs monthly to measure the impact of any policy changes on driver revenue

## 📁 Project Structure
    ├── Untitled1.ipynb       # Main analysis notebook
    ├── README.md             # Project documentation
    
## 🚀 Getting Started
        # Clone the repository
    git clone https://github.com/your-username/taxi-revenue-analysis.git
    cd taxi-revenue-analysis
    
    # Install dependencies
    import pandas as pd 
    import matplotlib.pyplot as plt
    import seaborn as sns 
    import numpy as np
    import scipy.stats as st
    from scipy import stats as st
    import statsmodels.api as sm
    import warnings 
    warnings.filterwarnings('ignore')
    
    # Launch the notebook
    jupyter notebook Untitled1.ipynb

## 📌 Conclusion
Statistical evidence confirms that credit card payments are associated with significantly higher fares in NYC yellow taxi trips. Encouraging card adoption is a low-friction, high-impact strategy for boosting driver revenue without changing the service experience.
