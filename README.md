🏏 IPL Data Analysis using Apache Spark on Databricks
📌 Project Overview
This project focuses on analyzing Indian Premier League (IPL) cricket match data using Apache Spark on Databricks, leveraging Python, SQL, and Matplotlib for ETL, data exploration, and visualization. The goal is to extract meaningful insights from raw IPL datasets, such as team performance, player statistics, match outcomes, and venue analysis.

🛠️ Tools & Technologies Used

Apache Spark: Distributed data processing engine for ETL and analytics.
Databricks: Cloud-based platform for big data analytics and collaborative notebooks.
Python (PySpark): For writing Spark jobs and data manipulation.
SQL: For querying structured data within Spark.
Matplotlib: For creating visualizations.
Pandas: For local data manipulation and plotting.


📂 Dataset Description
The project uses IPL datasets typically containing:

matches.csv: Match-level data including teams, venue, toss, winner, etc.
deliveries.csv: Ball-by-ball data including batsman, bowler, runs, wickets, etc.

These datasets are publicly available on platforms like Kaggle.

🔄 ETL Process
1. Data Ingestion

Loaded CSV files into Databricks using Spark DataFrames.
Verified schema and performed initial data inspection.

2. Data Cleaning

Handled missing values and inconsistent entries.
Standardized team names and player names.
Removed duplicate records.

3. Data Transformation

Joined matches and deliveries datasets for enriched analysis.
Created derived columns like total runs, wickets per match, strike rate, economy rate, etc.
Aggregated data for team-wise and player-wise performance.


📊 Analysis Performed
🏆 Match & Team Analysis

Total matches played per season.
Most successful teams by win count.
Toss decision impact on match outcome.

👨‍🏫 Player Performance

Top run scorers and wicket takers.
Best strike rate and economy rate.
Player of the match frequency.

🏟️ Venue Insights

Most matches played at each venue.
Venue-wise win percentage.

📈 Season Trends

Runs scored per season.
Wickets taken per season.
Average match duration and scores.


🧠 SQL Queries Used


Extracting top 5 batsmen by total runs:
SQLSELECT batsman, SUM(batsman_runs) AS total_runsFROM deliveriesGROUP BY batsmanORDER BY total_runs DESCLIMIT 5;Show more lines


Team win count:
SQLSELECT winner, COUNT(*) AS winsFROM matchesGROUP BY winnerORDER BY wins DESC;Show more lines


Toss vs Match Winner:
SQLSELECT toss_winner, winner, COUNT(*) AS match_countFROM matchesGROUP BY toss_winner, winner;Show more lines



📉 Visualizations
Created using Matplotlib and Pandas:

Bar charts for top players and teams.
Pie charts for toss decisions.
Line graphs for season-wise trends.
Heatmaps for venue performance.


📌 Key Insights

Toss decisions often influence match outcomes.
Certain venues favor specific teams.
Consistent players like Virat Kohli and MS Dhoni show up in top stats.
Some seasons had significantly higher scoring matches.


📁 Folder Structure
ipl-data-analysis/
│
├── data/
│   ├── matches.csv
│   └── deliveries.csv
│
├── notebooks/
│   └── IPL_Analysis_Notebook.ipynb
│
├── visuals/
│   └── top_players.png
│   └── team_wins.png
│
├── README.md
└── requirements.txt


✅ Conclusion
This project demonstrates how big data tools like Apache Spark can be used to perform scalable and insightful sports analytics. It combines ETL, SQL querying, and visualization to uncover patterns in IPL cricket data.
