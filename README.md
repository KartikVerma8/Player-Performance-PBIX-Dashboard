# Player-Performance-PBIX-Dashboard
📘 Objective

To analyze and visualize player performance metrics from the T20 World Cup 2024, and to identify the top-performing players across categories such as openers, middle-order batsmen, all-rounders, and bowlers.
Additionally, the project features a “Dream Team” — a data-driven selection of the best players based on their overall impact and consistency throughout the tournament.

⚙️ Tools & Technologies Used

Power BI Desktop

Microsoft Excel (Dataset Source – from Kaggle.com)

Power Query for Data Cleaning

DAX (Data Analysis Expressions) for Calculations

Data Modeling and Relationships

📊 Project Overview

This Power BI project provides an in-depth analysis of T20 World Cup 2024 player performance using an Excel dataset sourced from Kaggle.
It delivers interactive insights into batting, bowling, and all-round performance, helping users easily identify the top players and teams of the tournament.
The dashboard also includes a Dream Team page featuring the best XI players chosen based on data-driven criteria such as batting average, strike rate, wickets, and economy rate.

🧠 Step-by-Step Project Process
🔹 1. Data Collection

Downloaded the T20 World Cup 2024 player performance dataset from Kaggle.com in Excel format.

The dataset included attributes such as Player Name, Role, Team, Runs, Wickets, Average, Strike Rate, and Economy Rate.

🔹 2. Data Import into Power BI

Imported the dataset into Power BI Desktop using the Get Data → Excel option.

Verified all sheets and tables for proper structure and consistency.

🔹 3. Data Cleaning in Power Query

Performed thorough cleaning and transformation in Power Query Editor:

Promoted Headers to correctly define column names.

Changed Data Types (numbers, text, and dates).

Renamed Columns for better readability.

Removed Unnecessary Columns that didn’t contribute to analysis.

Handled Missing/Null Values — either removed incomplete rows or replaced them with correct data after cross-checking with Cricinfo.com.

Ensured data accuracy and consistency across all records.

After validation, clicked Close & Apply to load the cleaned data into Power BI.

🔹 4. Data Modeling

Created relationships between tables such as Player, Match, and Team based on unique identifiers.

Designed a Star Schema Model to ensure optimized querying and report performance.

Ensured referential integrity between datasets for seamless DAX calculations.

🔹 5. DAX Calculations

Developed custom measures and KPIs to support performance analysis and ranking:

Total Runs = SUM(Player[Runs])

Strike Rate = DIVIDE(SUM(Player[Runs]) * 100, SUM(Player[Balls Faced]))

Batting Average = DIVIDE(SUM(Player[Runs]), COUNT(Player[Innings]))

Wickets Taken = SUM(Player[Wickets])

Economy Rate = DIVIDE(SUM(Player[Runs Conceded]), SUM(Player[Overs Bowled]))

Impact Score = (Runs / 10) + (Wickets * 15) (used to select Dream Team players)

These measures powered the analytical insights and ranking systems throughout the report.

🔹 6. Report Building (Dashboard Creation)
🏠 Page 1 – Overview Dashboard

Tournament summary cards: total matches, total runs, total wickets, and average strike rate.

Dynamic KPIs: Top Run Scorer, Best Bowler, Player of the Match, and Best Economy Rate.

Overall team performance trends.

🏏 Page 2 – Openers Analysis

Bar charts and KPI visuals showing Top 5–6 Openers with highest runs and strike rates.

Filters by country, player role, and venue.

🎯 Page 3 – Middle Order Performance

Analysis of middle-order players based on average, boundaries, and strike rate.

Visual comparisons of players within teams.

💪 Page 4 – All-Rounders Analysis

Created an Impact Score combining batting and bowling metrics.

Visualized in a scatter plot showing player balance between run contribution and wicket impact.

🎳 Page 5 – Bowlers Dashboard

Highlighted top bowlers with most wickets, lowest economy, and best bowling averages.

Included visual trends for wickets per match and economy variation.

🧢 Page 6 – Dream Team (Top XI Players)

Designed a “Dream Team” page featuring the best 11 players from the T20 World Cup 2024.

Selection based purely on data-driven metrics:

Top 3 openers with the best average and strike rate.

3 middle-order batsmen with consistency and boundary ratio.

2 all-rounders with highest impact scores.

3 bowlers with best economy and wicket count.

Used KPI visuals, player cards, and role-based color coding to represent the Dream XI lineup.

Added a summary card showing Total Team Runs, Total Wickets, and Team Impact Score.

🎨 Dashboard Design

Used a cricket-themed color palette (green, yellow, blue).

Added logos, icons, and formatted titles for professional aesthetics.

Enabled cross-filtering, drill-through, and hover tooltips for interactivity.

💡 Key Insights & Outcomes

Identified Top Performers across roles (openers, middle order, all-rounders, bowlers).

Created a data-driven Dream Team XI showcasing the best players statistically.

Enabled comparative performance analysis for any player, team, or match.

Enhanced Power BI expertise in data modeling, DAX calculations, and report storytelling.

Produced a visually rich and insightful dashboard suitable for analytical decision-making in sports data.
