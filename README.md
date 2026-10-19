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

This project analyzes player performance during the ICC Men's T20 World Cup 2024 using Microsoft Power BI. The dashboard provides interactive insights into batting, bowling, and all-round performance to help identify top-performing players across different roles.

It also features a data-driven **Dream Team XI**, selecting players based on performance metrics such as batting average, strike rate, wickets, economy rate, and overall impact.

## Business Problem

Cricket tournaments generate large amounts of player performance data, making it difficult to compare players across different roles using raw statistics alone.

The objective of this project is to transform player statistics into meaningful, interactive visualizations that help answer questions such as:

- Who are the top-performing batsmen and bowlers?
- Which openers and middle-order batsmen demonstrate strong batting performance?
- Which all-rounders provide a balanced contribution with bat and ball?
- Which bowlers combine wicket-taking ability with economical bowling?
- How can a Dream Team XI be selected using performance-based criteria?

## Dataset

- **Tournament:** ICC Men's T20 World Cup 2024
- **Source:** Kaggle.com
- **Format:** Microsoft Excel
- **Data fields:** Player Name, Role, Team, Runs, Wickets, Batting Average, Strike Rate, and Economy Rate, along with other relevant performance attributes available in the dataset.

The dataset was imported into Power BI Desktop for cleaning, transformation, modeling, and visualization.

*Note: Add the original dataset link and exact row count here if available.*

## Tools & Technologies

- **Power BI Desktop:** Dashboard development and data visualization
- **Microsoft Excel:** Dataset source and initial data storage
- **Power Query (M):** Data cleaning and transformation
- **DAX:** Measures, calculated metrics, and KPIs
- **Data Modeling:** Relationships between relevant tables
- **Kaggle:** Dataset source

## Project Structure

The following is a suggested repository structure. Adjust the filenames to match the files actually uploaded to your GitHub repository.

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
│   └── dashboard_screenshot.png
│
└── README.md
```

## Data Cleaning & Preparation

Data preparation was performed using Power Query Editor in Power BI.

The main steps included:

1. **Data Import:** Imported the Excel dataset into Power BI Desktop.
2. **Promoted Headers:** Used the first row as column headers where required.
3. **Data Type Correction:** Assigned appropriate data types to numerical and text columns.
4. **Column Renaming:** Renamed columns for better readability.
5. **Column Removal:** Removed unnecessary columns that were not relevant to the analysis.
6. **Missing Value Handling:** Investigated missing values and removed incomplete records or corrected them after verification against ESPNcricinfo, where appropriate.
7. **Data Validation:** Checked the consistency and accuracy of the cleaned records.
8. **Data Loading:** Applied the transformations using **Close & Apply**.

## Exploratory Data Analysis (EDA)

The exploratory analysis focused on comparing player performance across batting, bowling, and all-rounder categories.

Key areas of analysis included:

- **Batting Performance:** Total runs, batting averages, and strike rates.
- **Opening Batsmen:** Comparison of run-scoring performance and strike rates.
- **Middle-Order Batsmen:** Analysis of batting consistency, boundaries, and strike rates.
- **All-Rounders:** Evaluation of combined batting and bowling contributions.
- **Bowling Performance:** Wickets taken, bowling averages, and economy rates.
- **Team Performance:** Comparison of player contributions across participating teams.

These analyses were used to build interactive report pages and support the selection of players for the Dream Team XI.

## Research Questions & Key Findings

### Research Questions

1. Who scored the most runs during the tournament?
2. Which players performed best as openers?
3. Which middle-order batsmen demonstrated strong performance across the selected metrics?
4. Which all-rounders made the most valuable combined contributions?
5. Which bowlers took the most wickets while maintaining economical bowling figures?
6. Which players should be considered for a data-driven Dream Team XI?

### Key Findings

The dashboard enables users to identify and compare top-performing players across the selected categories.

- Batting performance can be compared using runs, average, and strike rate.
- Bowling performance can be evaluated using wickets, bowling average, and economy rate.
- All-rounder contributions can be compared using the selected impact metric.
- The Dream Team page presents a role-based selection of 11 players using the project's chosen performance criteria.

*Add specific player names, statistics, and rankings from your actual dashboard to make this section more informative.*

## Dashboard

The Power BI report contains six analytical pages.

### 🏠 Page 1 – Overview Dashboard

- Tournament summary KPIs, including total matches, runs, wickets, and average strike rate.
- Dynamic indicators for top run scorer, best bowler, Player of the Match, and best economy rate, where supported by the dataset.
- Overview of team and player performance.

### 🏏 Page 2 – Openers Analysis

- Comparison of the top 5–6 openers using runs and strike rates.
- Filters for country, player role, and venue where available.
- Identification of high-performing opening batsmen.

### 🎯 Page 3 – Middle-Order Performance

- Analysis of batting average, boundaries, and strike rate.
- Comparison of middle-order players across teams.
- Evaluation of batting consistency and scoring contribution.

### 💪 Page 4 – All-Rounders Analysis

- Comparison of batting and bowling contributions.
- Impact Score used to support player evaluation.
- Scatter plot illustrating the relationship between run contribution and wicket impact.

### 🎳 Page 5 – Bowlers Dashboard

- Identification of leading wicket-takers.
- Comparison of bowling averages and economy rates.
- Analysis of wickets per match and economy variation, where supported by the data.

### 🧢 Page 6 – Dream Team XI

A dedicated page presenting a proposed XI based on the project's performance criteria.

The selection approach described for this project includes:

- 3 openers evaluated using batting average and strike rate.
- 3 middle-order batsmen evaluated using consistency and boundary ratio.
- 2 all-rounders evaluated using Impact Score.
- 3 bowlers evaluated using wicket-taking ability and economy rate.

The page also includes player cards, role-based color coding, and summary indicators for team runs, wickets, and impact score.

### Dashboard Design & Interactivity

- Cricket-inspired green, yellow, and blue color palette.
- KPI cards, bar charts, scatter plots, and player cards.
- Interactive slicers, cross-filtering, drill-through, and hover tooltips where configured.
- Role-based organization for easier player comparisons.

## How to Run This Project

1. Download or clone this GitHub repository.
2. Download the Excel dataset from the repository's dataset folder, if included.
3. Install Microsoft Power BI Desktop.
4. Open the `.pbix` dashboard file in Power BI Desktop.
5. If prompted, update the data source path to point to the downloaded Excel file.
6. Refresh the dataset to load the data.
7. Navigate through the report pages and use the available filters and interactive visuals.

*Ensure the PBIX file and dataset are included in the repository, or provide links to their actual locations.*

## Final Recommendations

Based on the analytical capabilities of this dashboard, the following recommendations can support further player-performance evaluation:

- **Compare players within their roles:** Evaluate openers, middle-order batsmen, all-rounders, and bowlers using role-appropriate metrics.
- **Balance batting performance:** Consider both scoring volume and strike rate when comparing batsmen.
- **Evaluate bowling effectiveness:** Review wickets alongside economy rate and bowling average instead of relying on a single metric.
- **Assess all-round contributions:** Consider both batting and bowling performance when evaluating all-rounders.
- **Use transparent selection criteria:** Apply consistent, role-specific criteria when selecting a Dream Team XI.
- **Validate the Impact Score:** Test alternative weightings for runs and wickets to understand how the selection changes.
- **Improve future analysis:** Incorporate match-level context, opposition strength, and consistency metrics if the required data is available.

These are analytical recommendations rather than verified tournament-specific conclusions. They should be refined using the actual dashboard findings.

## Author & Contact

**Kartik Verma**

- **LinkedIn:** [Add your LinkedIn profile URL](https://www.linkedin.com/)
- **GitHub:** [KartikVerma8](https://github.com/KartikVerma8)

Feel free to explore the project and share feedback or suggestions for improvement.
