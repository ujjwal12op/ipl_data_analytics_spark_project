## 🏏 IPL Data Analysis using Apache Spark on Databricks 
📌 Project Overview
This project focuses on analyzing Indian Premier League (IPL) cricket match data using Apache Spark on Databricks, leveraging PySpark, SQL, and Matplotlib for scalable ETL, data exploration, and insightful visualizations.
Goals:

## Team performance trends
Player statistics
Match outcomes
Venue-based analysis


## 🛠️ Tools & Technologies Used

Apache Spark: Distributed data processing for large-scale ETL and analytics
Databricks: Unified cloud platform for big data analytics and collaborative notebooks
PySpark (Python): For data manipulation and transformation
SQL: For structured querying within Spark
Matplotlib & Seaborn: For data visualization
Pandas: For local data manipulation and plotting


## 📂 Dataset Description
Publicly available IPL datasets (e.g., from Kaggle):

matches.csv: Match-level data (teams, venue, toss, winner, etc.)
deliveries.csv: Ball-by-ball data (batsman, bowler, runs, wickets, extras, etc.)


## 🔄 ETL Process
1. 📥 Data Ingestion

Loaded CSV files into Spark DataFrames using defined schemas
Verified schema integrity and performed initial inspection

2. 🧹 Data Cleaning

Removed duplicates and handled missing values
Standardized team and player names
Filtered out invalid deliveries (e.g., wides, no-balls for specific analyses)

3. 🔄 Data Transformation

Joined match and delivery datasets for enriched analytics
Created derived columns: total runs, wickets, strike rate, economy rate, etc.
Applied window functions for running totals and rankings
Added conditional flags (e.g., high-impact deliveries, veteran players)


📊 Key Analyses Performed
🏆 Match & Team Analysis

Total matches played per season
Most successful teams by win count
Toss decision impact on match outcome
Categorized win margins: High, Medium, Low

👨‍🏫 Player Performance

Top run scorers and wicket takers
Best strike rate and economy rate
Veteran player identification (age ≥ 35)
Years since debut calculation
Player performance in winning matches

🏟️ Venue Insights

Average and highest scores by venue
Most matches played per venue
Venue-wise team performance

📈 Season Trends

Runs scored per season
Wickets taken per season
Average match duration and scores


## 📉 Visualizations
Created using Matplotlib and Seaborn:

📊 Bar charts: Top players and teams
🥧 Pie charts: Toss decisions
📈 Line graphs: Season-wise trends
🔥 Heatmaps: Venue performance
📉 Player performance in wins (Top 10 scorers)


## ✅ Conclusion
This project demonstrates how big data tools like Apache Spark can be used to perform scalable and insightful sports analytics. It combines ETL, SQL querying, and visualization to uncover hidden patterns in IPL cricket data, making it a strong portfolio project for data engineering and analytics roles.
