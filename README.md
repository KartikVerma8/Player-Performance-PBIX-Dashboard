# Player-Performance-PBIX-Dashboard

## 📌 Table of Contents

- [Overview](#overview)
- [Business Problem](#business-problem)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Project Structure](#project-structure)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Research Questions & Key Findings](#research-questions--key-findings)
- [Dashboard](#dashboard)
- [How to Run This Project](#how-to-run-this-project)
- [Final Recommendations](#final-recommendations)
- [Author & Contact](#author--contact)

---

## Overview

This project analyzes player performance during the ICC Men's T20 World Cup 2024 using Microsoft Power BI. It provides interactive insights into batting, bowling, and all-round performance to identify top-performing players across different roles.

The dashboard also features a data-driven Dream Team XI, selecting players based on performance metrics such as batting average, strike rate, wickets, economy rate, and overall impact.

## Business Problem

Cricket tournaments generate extensive player statistics, making it challenging to compare players across different roles using raw data alone.

This project transforms player statistics into interactive visualizations to answer questions such as:

- Who are the top-performing batsmen and bowlers?
- Which openers and middle-order batsmen perform best across selected metrics?
- Which all-rounders contribute effectively with both bat and ball?
- Which bowlers combine wicket-taking ability with economical bowling?
- How can a Dream Team XI be selected using performance-based criteria?

## Dataset

- **Tournament:** ICC Men's T20 World Cup 2024
- **Source:** Kaggle
- **Format:** Microsoft Excel
- **Attributes:** Player Name, Team, Role, Runs, Wickets, Batting Average, Strike Rate, Economy Rate, and other available performance metrics.

The dataset was imported into Power BI Desktop for data cleaning, transformation, modeling, and visualization.

*Note: Add the original Kaggle dataset URL and exact dataset details when available.*

## Tools & Technologies

- **Power BI Desktop:** Dashboard development and visualization
- **Microsoft Excel:** Dataset source
- **Power Query (M):** Data cleaning and transformation
- **DAX:** Measures, calculations, and KPIs
- **Data Modeling:** Relationships between relevant tables
- **Kaggle:** Dataset source

## Project Structure

```text
Player-Performance-PBIX-Dashboard/
│
├── Dataset/
│   └── T20_World_Cup_2024.xlsx
│
├── Dashboard/
│   └── Player_Performance_Dashboard.pbix
│
├── Images/
│   ├── powerhouse-openers.png
│   ├── pressure-absorbers.png
│   ├── power-surge.png
│   ├── all-rounders.png
│   └── fast-bowlers.png
│
└── README.md
```

*The filenames above are suggested names. Ensure they match the files uploaded to your repository.*

## Data Cleaning & Preparation

Data preparation was performed using Power Query Editor in Power BI.

1. **Data Import:** Imported the Excel dataset into Power BI Desktop.
2. **Promoted Headers:** Used the first row as column headers where required.
3. **Data Type Correction:** Assigned appropriate data types to columns.
4. **Column Renaming:** Renamed columns for better readability.
5. **Column Removal:** Removed unnecessary columns that were not relevant to the analysis.
6. **Missing Value Handling:** Investigated missing values and removed incomplete records or corrected them after verification against ESPNcricinfo, where appropriate.
7. **Data Validation:** Checked the consistency and accuracy of the cleaned records.
8. **Data Loading:** Applied the transformations using **Close & Apply**.

## Exploratory Data Analysis (EDA)

The exploratory analysis focused on comparing player performance across different batting and bowling roles.

- **Batting Performance:** Runs, batting averages, strike rates, and boundary percentages.
- **Openers:** Comparison of leading openers by runs, average, and strike rate.
- **Middle-Order Batsmen:** Evaluation of batting consistency and scoring contribution.
- **All-Rounders:** Comparison of batting and bowling contributions using an impact metric.
- **Bowlers:** Analysis of wickets, bowling averages, strike rates, and economy rates.
- **Player Comparison:** Interactive comparison of players using tables, trend charts, and scatter plots.

## Research Questions & Key Findings

### Research Questions

1. Who scored the most runs during the tournament?
2. Which openers performed best in terms of runs and strike rate?
3. Which middle-order batsmen demonstrated strong batting performance?
4. Which all-rounders made valuable contributions with bat and ball?
5. Which bowlers combined wicket-taking ability with economical bowling?
6. Which players should be considered for a data-driven Dream Team XI?

### Key Findings

The dashboard provides interactive views to identify and compare players across the selected categories.

- Batting performance can be compared using runs, average, strike rate, and boundary percentage.
- Bowling performance can be assessed using wickets, economy rate, and bowling average.
- All-rounders can be evaluated using their combined batting and bowling contributions.
- The player comparison visuals help highlight differences between selected players.
- The Dream Team page presents an XI based on the project's defined selection criteria.

*Add specific player names and numerical findings from the dashboard to make this section more informative.*

## Dashboard

The Power BI report includes specialized pages for player performance analysis. The screenshots below show the corresponding dashboard views.

### 🏏 1. Powerhouse / Openers

Analyzes the leading opening batsmen using runs, batting average, strike rate, and boundary percentage.

- Compares the highest run-scoring openers.
- Displays batting metrics in a player comparison table.
- Uses visual comparisons to explore batting average and strike rate.
- Supports interactive player selection.

[https://github.com/KartikVerma8/Player-Performance-PBIX-Dashboard/blob/b8848ea419fc9a6f418f47df830d2adfe7e9c0f9/Power-House](https://github.com/KartikVerma8/Player-Performance-PBIX-Dashboard/blob/479469508eb3fd456b89ffc00a961facf959d06b/Power-House.png)

### 🎯 2. Pressure Absorbers

Focuses on middle-order and pressure-handling batting performance using the selected batting metrics.

- Compares runs, batting average, strike rate, and boundary percentage.
- Highlights differences in player scoring performance.
- Includes comparative visuals for batting average and strike rate.

[![Pressure Absorbers Dashboard](Images/pressure-absorbers.png)](https://github.com/KartikVerma8/Player-Performance-PBIX-Dashboard/blob/51552c14442e712cda475947838f447ba2a22532/Pressure-Absorber.png)

### 💥 3. The Power Surge

Analyzes powerful batting contributions using batting average, strike rate, and related player performance metrics.

- Compares runs and batting performance across selected players.
- Displays strike rate and batting average comparisons.
- Supports player-level analysis through interactive visuals.

[![The Power Surge Dashboard](Images/power-surge.png)](https://github.com/KartikVerma8/Player-Performance-PBIX-Dashboard/blob/f1bcd4c2a146be00c76c2b876a81d69b73cfe282/Power%20Surge.png)

### 💪 4. All-Rounders

Evaluates players who contribute with both bat and ball.

- Compares runs, batting average, strike rate, wickets, and economy rate.
- Presents bowling statistics alongside batting metrics.
- Uses a scatter plot to compare bowling strike rate and economy rate.
- Supports evaluation of balanced all-round performance.

[![All-Rounders Dashboard](Images/all-rounders.png)](https://github.com/KartikVerma8/Player-Performance-PBIX-Dashboard/blob/93c82a9c39849f2f320f8a44db2679f06c4e4e5d/All%20rounders.png)

### 🎳 5. Fast Bowlers

Analyzes fast-bowling performance using wickets, economy rate, bowling strike rate, and bowling average.

- Highlights leading wicket-takers.
- Compares economy rates and bowling averages.
- Displays bowling performance trends.
- Uses a scatter plot to compare bowling strike rate and economy rate.

[Fast Bowlers.png](https://github.com/KartikVerma8/Player-Performance-PBIX-Dashboard/blob/bfbfd7aed40e922fca34253f72e2719489b1ebbf/Fast%20Bowlers.png)

### 🎨 Dashboard Design & Interactivity

- Cricket-inspired green, yellow, blue, and dark-themed design.
- KPI visuals, player tables, trend charts, and scatter plots.
- Interactive player selection and report navigation.
- Group Stage and Super 8 filters.
- Cross-filtering and tooltips where configured.

## How to Run This Project

1. Clone or download this GitHub repository.
2. Download the Excel dataset from the repository's `Dataset` folder, if included.
3. Install Microsoft Power BI Desktop.
4. Open the `.pbix` file from the `Dashboard` folder.
5. If prompted, update the data source path to the downloaded Excel dataset.
6. Refresh the data and verify that all report visuals load correctly.
7. Navigate through the dashboard pages and use the available filters.

## Final Recommendations

Based on the analytical capabilities of this dashboard, the following recommendations can support player-performance evaluation:

- **Compare players by role:** Use role-appropriate metrics rather than applying the same criteria to every player.
- **Evaluate batting effectiveness:** Consider runs, batting average, and strike rate together.
- **Assess bowling performance:** Evaluate wickets alongside economy rate and bowling average.
- **Measure all-round contributions:** Consider both batting and bowling performance.
- **Use transparent selection criteria:** Apply consistent metrics when selecting a Dream Team XI.
- **Validate the Impact Score:** Test alternative weightings for runs and wickets to understand how player rankings change.
- **Expand future analysis:** Include opposition strength, match conditions, and consistency metrics if the required data is available.

These are general analytical recommendations and should be refined using verified results from the dashboard.

## Author & Contact

**Kartik Verma**

- **GitHub:** [KartikVerma8](https://github.com/KartikVerma8)
- **LinkedIn:** Add your LinkedIn profile URL

