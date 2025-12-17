# 📊 End-to-End Data Analysis Portfolio

![Data Analysis Banner](https://img.shields.io/badge/Data%20Analysis-Portfolio-blue?style=for-the-badge&logo=github) ![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

Welcome to my data analytics portfolio! This repository houses a collection of end-to-end projects demonstrating my ability to solve real-world problems using data.

## 📂 Repository Structure & Industry Verticals

I have organized my projects according to standard **Economic Sectors (Verticals)** to demonstrate domain-specific analytics.

```text
Data-Analytics-Portfolio/
│
├── .gitignore                   <-- CRITICAL: Ignores virtual envs, .DS_Store, and large data files
├── README.md                    <-- The Main Portfolio Landing Page
│
│   # -----------------------------------------------------------------------
│   # PROJECT 1: RETAIL / E-COMMERCE (Vertical: Logistics, Trade & Services)
│   # Focus: Engineering + Full Stack Analytics (Python -> SQL -> Tableau)
│   # -----------------------------------------------------------------------
├── 01_Ecomm_Retail_E2E/
│   ├── README.md                <-- 𝗣𝗿𝗲𝘀𝗰𝗿𝗶𝗽𝘁𝗶𝘃𝗲 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀 (Recommendation) & Project-specific docs
│   ├── requirements.txt         <-- Libraries: selenium, pandas, sqlalchemy, scikit-learn
│   │
│   ├── data/
│   │   ├── raw/                 <-- Scraped JSON/CSVs (e.g., amazon_prices.csv)
│   │   └── processed/           <-- Cleaned CSVs ready for SQL import
│   │
│   ├── scripts/                 <-- The Automation Engines (Data Engineering)
│   │   ├── 01_scraper_bot.py    <-- Selenium/BS4 script
│   │   └── 02_cleaning_etl.py   <-- Pandas script to clean & push to SQL
│   │
│   ├── sql/                        <-- 𝗗𝗶𝗮𝗴𝗻𝗼𝘀𝘁𝗶𝗰 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀 (Database Logic)
│   │   ├── schema_setup.sql        <-- CREATE TABLE code (Star Schema design)
│   │   └── analytical_queries.sql  <-- Complex queries used for analysis
│   │
│   ├── models/                      <-- 𝗣𝗿𝗲𝗱𝗶𝗰𝘁𝗶𝘃𝗲 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀 (ML Models)
│   │   ├── churn_prediction.ipynb   <-- Notebook for Customer Churn (Logistic Regression)
│   │   └── sales_forecasting.ipynb  <-- Notebook for Time Series
│   │
│   └── dashboards/                         <-- 𝗗𝗲𝘀𝗰𝗿𝗶𝗽𝘁𝗶𝘃𝗲 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀
│       ├── Retail_Executive_Dashboard.twb  <-- Tableau Workbook
│       └── images/                         <-- Screenshots of dashboard for the README
│
│   # -----------------------------------------------------------------------
│   # PROJECT 2: E-SPORTS / STRATEGY (Vertical: Tech, Media & Strategy)
│   # Focus: Storytelling & Tool Mastery (Excel + Power BI)
│   # -----------------------------------------------------------------------
├── 02_E-Sports_Chess_Analysis/
│   ├── README.md
│   ├── data/                    <-- 𝗗𝗶𝗮𝗴𝗻𝗼𝘀𝘁𝗶𝗰 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀 (Power Query)
│   │   ├── raw_games.csv        <-- Kaggle dataset
│   │   └── processed_excel.xlsx <-- The Excel file with Power Query steps
│   │
│   └── dashboards/                      <-- 𝗗𝗲𝘀𝗰𝗿𝗶𝗽𝘁𝗶𝘃𝗲 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀
│       ├── Chess_Opening_Strategy.pbix  <-- Power BI File
│       └── images/                      <-- Screenshots of dashboard
│
│   # -----------------------------------------------------------------------
│   # PROJECT 3: BANKING (Vertical: BFSI)
│   # Focus: Statistical Rigor & Business Logic (Python + SQL + Tableau)
│   # -----------------------------------------------------------------------
├── 03_BFSI_Credit_Risk/
│   ├── README.md
│   ├── requirements.txt
│   ├── data/
│   │   └── loan_defaults.csv
│   │
│   ├── analysis/
│   │   ├── 01_EDA_and_cleaning.ipynb    <-- Diagnostic Analytics (Correlation matrix)
│   │   └── 02_risk_prediction_model.ipynb <-- 𝗣𝗿𝗲𝗱𝗶𝗰𝘁𝗶𝘃𝗲 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀 (Logistic Reg/Decision Tree)
│   │
│   └── strategy_report/
│       └── Credit_Risk_Strategy.pdf     <-- 𝗣𝗿𝗲𝘀𝗰𝗿𝗶𝗽𝘁𝗶𝘃𝗲 𝗔𝗻𝗮𝗹𝘆𝘁𝗶𝗰𝘀 (Recommendation)
```

---

### 🚀 Portfolio Highlights

| Project                                                  | Vertical/Domain                      | Type                        | Tech Stack                          | Key Business Insight                                                                                               |
| :------------------------------------------------------- | :----------------------------------- | :-------------------------- | :---------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| **[01. Retail E2E Pipeline](./01_Ecomm_Retail_E2E/)**    | 🛒 Logistics & Trade (Retail/E-Comm) | **Full Stack**              | Python (Selenium), SQL, Tableau     | Developed a competitor price tracker and churn prediction model to identify high-risk customer segments.           |
| **[02. Chess Analytics](./02_E-Sports_Chess_Analysis/)** | ♟️ Tech & Media (E-Sports/Strategy)  | **Descriptive/Diagnostic**  | Excel, Power BI                     | Analyzed opening repertoires to visualize win-rates; proved specific openings increase win probability by 15%.     |
| **[03. Credit Risk Model](./03_BFSI_Credit_Risk/)**      | 🏦 BFSI (Banking & Finance)          | **Predictive/Prescriptive** | Python (Scikit-Learn), SQL, Tableau | Built a Logistic Regression model to predict loan defaults; recommended a strategy to reduce risk exposure by 12%. |

---

### 📂 Project Details

#### 1. [The "Hero" Project: Retail Competitor & Sales Analytics](./01_Ecomm_Retail_E2E/)

- **The Goal:** Build a completely automated pipeline to track competitor pricing and analyze internal sales health.
- **The Workflow:**
  - **Extract:** Web scraped product data using `Selenium` & `BeautifulSoup`.
  - **Process:** Cleaned data with `Pandas` and stored in a **PostgreSQL** database.
  - **Analyze:** Performed Customer Churn modeling (Binary Classification) and Sales Forecasting.
  - **Visualize:** Connected Tableau to the SQL database for a live executive dashboard.

#### 2. [Chess Opening Analysis](./02_E-Sports_Chess_Analysis/)

- **The Goal:** Translate complex game data into a visual story for non-technical users.
- **The Workflow:** Used **Excel Power Query** for data transformation and **Power BI** for interactive filtering of chess opening effectiveness.

#### 3. [BFSI Loan Default Prediction](./03_BFSI_Credit_Risk/)

- **The Goal:** Reduce financial risk by predicting bad loans before they are approved.
- **The Workflow:** Used Python for **Diagnostic Analysis** (Correlation Matrices) to find root causes of default, and **Predictive Modeling** (Logistic Regression) to flag high-risk applicants.

---

### 📊 Industry Overview

Just for the overview am providing all the core sector/industries data analyst work on (Just for information) :

#### 🛠️ Technical Stack & Workflow

| Analytics Phase | Primary Tools                | Secondary Tools         |
| --------------- | ---------------------------- | ----------------------- |
| Descriptive     | SQL, PowerBI, Tableau        | Excel                   |
| Diagnostic      | Excel, SQL, PowerBI, Tableau | Python                  |
| Predictive      | Python (Matplotlib/Seaborn)  | SQL                     |
| Prescriptive    | Python                       | Excel, PowerBI, Tableau |

#### **Tools Specifics**

- **Python(TRANSFORMER - Cleaning & Modelling):** Pandas, NumPy, Scikit-Learn (ML), Matplotlib/Seaborn(DataViz).
- **SQL (FETCHER - Large Dataset):** PostgreSQL (Mostly), MySQL.
- **BI & Viz:** PowerBI (DAX, Power-Query), Tableau, Excel (AUDITOR - VBA/Pivot/Lookups).
- **Others:** Git, GitHub (Pages/Repo), VSCode, Jupyter, pgAdmin/Dbeaver (PostgreSQL).

  | #   | Vertical Name<br>[70% work is in 3 vertical & desc/diag]                      | Economic Sector Classification                      | Industries Included (ICI, GICS, ISIC)                                                                                                      | Analyst Focus Topic/proj/example                                                                                                                                                                                 |
  | --- | ----------------------------------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  | 1   | Energy, Resources & Utilities<br>[Dominant Analytics : Prescriptive]          | Primary (Mining)<br>Secondary (Power/Refining)      | • India Core: Coal, Crude Oil, Natural Gas, Refinery Products, Electricity.<br>• Global: Renewable Energy, Water Supply, Waste Management. | • Demand Forecasting & Load Balancing<br>• Predictive Maintenance (Asset Management)<br>• Production Optimization, EDA<br>• Environmental Impact Analysis                                                        |
  | 2   | Agriculture, Food & Staples<br>[Dominant Analytics : Descriptive]             | Primary (Farming)<br>Secondary (Processing)         | • India Core: Fertilizers.<br>• Global: Farming, Fishing, Forestry, Food & Beverage Processing (FMCG).                                     | • Yield Prediction & Crop Modeling<br>• Supply Chain Cold-Chain Integrity<br>• Commodity Price Trend Analysis<br>• Soil & Weather Pattern Correlation<br>• Inventory Spoilage Reduction                          |
  | 3   | Heavy Manufacturing (Industrial 4.0)<br>[Dominant Analytics : Diagnostic]     | Secondary (Production)                              | • India Core: Steel, Cement.<br>• Global: Automotive, Aerospace, Chemicals, Machinery, Textiles                                            | • Quality Control (Six Sigma/Defect Rates)<br>• OEE (Overall Equipment Effectiveness)<br>• Supply Chain & Vendor Risk Management<br>• Production Cycle Time Analysis<br>• Safety Incident Reporting              |
  | 4   | Construction & Real Estate<br>[Dominant Analytics : Descriptive]              | Secondary (Building)<br>Tertiary (Leasing/Sales)    | • Global: Infrastructure, Residential & Commercial Real Estate, PropTech, Smart Cities.                                                    | • Project Cost Overrun Estimation<br>• Market Valuation & Price Indices<br>• Rental Yield & ROI Analysis<br>• Geographic/Spatial (GIS) Analysis<br>• Occupancy & Vacancy Rate Tracking                           |
  | 5   | Logistics, Trade & Consumer Services<br>[Dominant Analytics : Predictive]     | Tertiary (Service & Distribution)                   | • Global: Retail, E-commerce, Wholesale, Transport (Rail/Air/Ship), Warehousing, Tourism.                                                  | • Route Optimization & Fleet Management<br>• Customer Segmentation & Churn Analysis<br>• Market Basket Analysis (Cross-selling)<br>• Delivery Time Performance Metrics<br>• Inventory Turnover & Demand Planning |
  | 6   | BFSI (Banking, Fin. Service & Insurance)<br>[Dominant Analytics : Predictive] | Tertiary (Service)<br>Quaternary (Analysis)         | • Global: Commercial Banks, Insurance, Fintech, Stock Markets, Wealth Management.                                                          | • Credit Risk Assessment & Scoring<br>• Fraud Detection Algorithms<br>• Customer Lifetime Value (CLV)<br>• Portfolio Performance Analysis<br>• Claims Processing Efficiency                                      |
  | 7   | Healthcare & Life Science<br>[Dominant Analytics : Diagnostic]                | Tertiary (Care)<br>Quaternary (R&D)                 | • Global: Hospitals, Pharmaceuticals, Biotech, Medical Devices, Public Health.                                                             | • Patient Readmission Prediction<br>• Clinical Trial Data Analysis<br>• Epidemiology & Disease Mapping<br>• Hospital Resource Utilization<br>• Drug Efficacy Modeling                                            |
  | 8   | Tech, Media & Strategy<br>[Dominant Analytics : Desc/Diagnostic]              | Quaternary (Knowledge)<br>Quinary (Decision Making) | • Global: IT Services, Telecom, Education, Media, Sports, Government Policy, NGOs.                                                         | • Sentiment Analysis (NLP)<br>• User Engagement & A/B Testing<br>• Policy Impact Assessment<br>• Educational Assessment Metrics<br>• Player/Team Performance Analytics                                           |

---

## 💻 How to Run These Projects

If you wish to run the code locally, follow the steps below:

### 1️⃣ Clone the repository

```bash
git clone https://github.com/sonimonish00/Data-Analytics-Portfolio.git
```

### 2️⃣ Navigate to the project folder

```bash
cd Data-Analytics-Portfolio/01_Ecomm_Retail_E2E
```

### 3️⃣ Install dependencies (for Python projects)

```bash
pip install -r requirements.txt
```

### 4️⃣ Open the Notebook/File

Launch Jupyter Lab, or open the .pbix / .sql files in their respective applications.

📫 Contact & Feedback

I am always open to feedback or collaboration opportunities!

    GitHub: [sonimonish00](https://github.com/sonimonish00)

    LinkedIn: [Monish Soni](https://www.linkedin.com/in/monishsoni/)

    Email: sonimonish00[at]gmail[dot]com

    Portfolio Website: [sonimonish00](https://sonimonish00.github.io/)
