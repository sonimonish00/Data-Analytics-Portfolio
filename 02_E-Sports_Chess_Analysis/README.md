# ♟️ Chess : Descriptive & Diagnostic Analytics

![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=flat&logo=powerbi) ![Excel](https://img.shields.io/badge/Excel-Power%20Query-217346?style=flat&logo=microsoft-excel) ![Status](https://img.shields.io/badge/Status-Complete-success?style=flat)

## 📖 Executive Summary

**Goal:** Answer _"What happened in 20,000+ games?"_ and _"Why do specific players win?"_

This project bridges **Descriptive Analytics** (summarizing historical match data) and **Diagnostic Analytics** (investigating the root causes of victory). Using a dataset of online chess games, I built an interactive Business Intelligence (BI) solution to help players optimize their opening repertoire.

While Descriptive analytics tells us _that_ White wins more often, Diagnostic analytics helps us understand _which specific opening moves_ drive that advantage.

---

## 💼 Business Problem & Objectives

In competitive strategy (E-Sports/Chess), the margin for error is slim. Players need to know:

1.  **Descriptive (The Landscape):** What are the most popular openings? What is the average game length?
2.  **Diagnostic (The Strategy):** _Why_ does the "Sicilian Defense" yield higher win rates for Black? Is it due to early traps (short games) or positional grinding (long games)?

---

## 📂 Repository Structure

```text
02_E-Sports_Chess_Analysis/
├── README.md
├── data/                    <-- Diagnostic Analytics (Power Query)
│   ├── raw_games.csv        <-- Kaggle dataset
│   └── processed_excel.xlsx <-- The Excel file with Power Query steps
│
└── dashboards/                      <-- Descriptive Analytics
    ├── Chess_Opening_Strategy.pbix  <-- Power BI File
    └── images/                      <-- Screenshots of dashboard
```

## 🛠️ Tools & Technologies Used

This project relies on Low-Code/No-Code BI tools to handle data transformation and interactive storytelling.

| Component            | Tool / Feature                     | Usage                                                                                     |
| :------------------- | :--------------------------------- | :---------------------------------------------------------------------------------------- |
| **ETL & Cleaning**   | **Excel (Power Query)**            | Cleaning raw notation (PGN), filtering nulls, and standardizing opening names.            |
| **Descriptive Viz**  | **Power BI (Core Visuals)**        | Histograms for game length distribution, Donut charts for Win/Loss ratios.                |
| **Diagnostic Logic** | **Power BI (DAX & Drill-through)** | Creating "Drill-through" filters to isolate specific openings and analyze win-conditions. |
| **Modeling**         | **Star Schema**                    | Modeled the data into Fact (Games) and Dimensions (Players, Openings, Time Control).      |

---

## 🔎 The Analysis: Hybrid Approach

This project demonstrates two distinct analytical layers:

### 1️⃣ Phase 1: Descriptive Analytics ("What Happened?")

_Focus: Aggregation & Central Tendency_

- **Metrics:** Total Games Played, Average Rating, Game Length Distribution.
- **Visuals:**
  - **Frequency Distribution:** Which openings are played most often? (Pareto Analysis).
  - **Time Series:** How game popularity shifts over time (if time data exists).
- **Insight:** "The King's Pawn Game is the most frequent opening, accounting for 63% of matches."

### 2️⃣ Phase 2: Diagnostic Analytics ("Why did it Happen?")

_Focus: Root Cause & Segmentation_

- **Technique: Drill-Down Analysis:**
  - Users can click on a high-level opening (e.g., "Sicilian Defense") and _drill down_ into specific variations (e.g., "Najdorf Variation").
- **Technique: Correlation:**
  - Analyzing the relationship between **Opening Choice** and **Win Probability**.
  - Investigating if "First Move Advantage" (White) holds true across all skill levels.
- **Insight:** "While White usually has an advantage, the 'Scandinavian Defense' reverses this trend in lower-rated games due to frequent opponent blunders."

---

## 📊 Dashboard Preview & Logic

### Power BI Features Implemented

- **Slicers:** Filter by Player Rating (Beginner vs. Grandmaster).
- **Decomposition Tree (Diagnostic):** breaks down the "Win Rate" metric by First Move -> Second Move -> Outcome.
- **Tooltips:** Hovering over a move shows the average rating of players who use it.

---

## 🚀 How to Run This Project

### 1. Prerequisites

You need **Microsoft Power BI Desktop** installed (Free).

### 2. View the Dashboard

1.  Navigate to the `dashboards/` folder.
2.  Double-click `Chess_Opening_Strategy.pbix`.
3.  Interact with the report:
    - _Click_ on a bar chart to filter the rest of the page.
    - _Right-click_ on an opening name to "Drill Through" to the deep-dive page.

### 3. Check the Data Transformation

1.  Open `data/processed_excel.xlsx`.
2.  Go to the **Data** tab -> **Queries & Connections** to see the Power Query steps applied to the raw data.

---

## 🗝️ Key Concepts Demonstrated

- **Descriptive:** Measures of Central Tendency (Mean Rating), Frequency Distributions.
- **Diagnostic:** Root Cause Analysis, Drill-Downs, Comparative Analysis (White vs. Black win rates).
- **Data Modeling:** Fact/Dimension relationships in Power BI.

---

### 📫 Contact & Feedback

- **GitHub:** [sonimonish00](https://github.com/sonimonish00)
