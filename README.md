# 🏏 IPL Data Analysis using Apache Spark on Databricks

## 📌 **Project Overview**
This project focuses on analyzing **Indian Premier League (IPL)** cricket match data using **Apache Spark** on **Databricks**, leveraging **Python**, **SQL**, and **Matplotlib** for **ETL**, **data exploration**, and **visualization**.  
The goal is to **extract meaningful insights** from raw IPL datasets, such as:

- Team performance  
- Player statistics  
- Match outcomes  
- Venue analysis  

---

## 🛠️ **Tools & Technologies Used**

- **Apache Spark**: Distributed data processing engine for ETL and analytics  
- **Databricks**: Cloud-based platform for big data analytics and collaborative notebooks  
- **Python (PySpark)**: For writing Spark jobs and data manipulation  
- **SQL**: For querying structured data within Spark  
- **Matplotlib**: For creating visualizations  
- **Pandas**: For local data manipulation and plotting  

---

## 📂 **Dataset Description**

The project uses IPL datasets typically containing:

- `matches.csv`: Match-level data including teams, venue, toss, winner, etc.  
- `deliveries.csv`: Ball-by-ball data including batsman, bowler, runs, wickets, etc.  

These datasets are publicly available on platforms like **Kaggle**.

---

## 🔄 **ETL Process**

### 1. 📥 **Data Ingestion**
- Loaded CSV files into Databricks using Spark DataFrames  
- Verified schema and performed initial data inspection  

### 2. 🧹 **Data Cleaning**
- Handled missing values and inconsistent entries  
- Standardized team names and player names  
- Removed duplicate records  

### 3. 🔄 **Data Transformation**
- Joined `matches` and `deliveries` datasets for enriched analysis  
- Created derived columns like total runs, wickets per match, strike rate, economy rate, etc.  
- Aggregated data for team-wise and player-wise performance  

---

## 📊 **Analysis Performed**

### 🏆 **Match & Team Analysis**
- Total matches played per season  
- Most successful teams by win count  
- Toss decision impact on match outcome  

### 👨‍🏫 **Player Performance**
- Top run scorers and wicket takers  
- Best strike rate and economy rate  
- Player of the match frequency  

### 🏟️ **Venue Insights**
- Most matches played at each venue  
- Venue-wise win percentage  

### 📈 **Season Trends**
- Runs scored per season  
- Wickets taken per season  
- Average match duration and scores  

---

## 📉 Visualizations
Created using Matplotlib and Pandas:

-📊 Bar charts for top players and teams
-🥧 Pie charts for toss decisions
-📈 Line graphs for season-wise trends
-🔥 Heatmaps for venue performance

## ✅ Conclusion
This project demonstrates how big data tools like Apache Spark can be used to perform scalable and insightful sports analytics.
It combines ETL, SQL querying, and visualization to uncover patterns in IPL cricket data.
