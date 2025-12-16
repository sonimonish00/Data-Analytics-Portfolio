# 🛒 Retail Analytics Pipeline: End-to-End (The "Hero" Project)

## 📖 Executive Summary

This project is a Full-Stack Data Analytics solution designed for the Retail/E-Commerce sector. It simulates a real-world scenario where a company needs to track competitor pricing (External Data) and analyze internal customer retention (Internal Data).

The pipeline automates data extraction via **Web Scraping**, stores clean data in a **PostgreSQL Data Warehouse**, predicts customer churn using **Machine Learning**, and visualizes actionable insights via a **Tableau Dashboard**.

---

## 💼 Business Problem & Objectives

Retailers face two major threats: **Price Wars** and **Customer Churn**.

1.  **Objective 1 (Market Intelligence):** Scrape competitor pricing data to identify where our products are overpriced or underpriced.
2.  **Objective 2 (Customer Retention):** Analyze historical sales data to predict which customers are likely to stop buying (churn) in the next 30 days.

## 📂 Repository Structure

```text
01_Ecomm_Retail_E2E/
├── README.md                <-- Prescriptive Analytics (Recommendation) & Project-specific docs
├── requirements.txt         <-- Libraries: selenium, pandas, sqlalchemy, scikit-learn
│
├── data/
│   ├── raw/                 <-- Scraped JSON/CSVs (e.g., amazon_prices.csv)
│   └── processed/           <-- Cleaned CSVs ready for SQL import
│
├── scripts/                 <-- The Automation Engines (Data Engineering)
│   ├── 01_scraper_bot.py    <-- Selenium/BS4 script
│   └── 02_cleaning_etl.py   <-- Pandas script to clean & push to SQL
│
├── sql/                        <-- Diagnostic Analytics (Database Logic)
│   ├── schema_setup.sql        <-- CREATE TABLE code (Star Schema design)
│   └── analytical_queries.sql  <-- Complex queries used for analysis
│
├── models/                      <-- Predictive Analytics (ML Models)
│   ├── churn_prediction.ipynb   <-- Notebook for Customer Churn (Logistic Regression)
│   └── sales_forecasting.ipynb  <-- Notebook for Time Series
│
└── dashboards/                         <-- Descriptive Analytics
    ├── Retail_Executive_Dashboard.twb  <-- Tableau Workbook
    └── images/                         <-- Screenshots of dashboard for the README
```

---

## 🛠️ Tech Stack

| Component        | Tool / Library          | Usage                                                           |
| ---------------- | ----------------------- | --------------------------------------------------------------- |
| Data Extraction  | Selenium, BeautifulSoup | Automated scraping of dynamic e-commerce pages.                 |
| Data Processing  | Pandas, NumPy           | Cleaning, transformation, and handling missing values.          |
| Database         | PostgreSQL, SQLAlchemy  | Relational storage using Star Schema design.                    |
| Machine Learning | Scikit-Learn            | Logistic Regression for binary classification (Churn/No-Churn). |
| Visualization    | Tableau                 | Interactive dashboard for stakeholders.                         |

## 📂 Database Schema (SQL)

The project uses a **Star Schema** optimized for analytics:

- **Fact Table:** fact_sales (Transactions, Revenue, Dates)
- **Dimension Tables:**

  - dim_customers (Demographics, Membership Tier)
  - dim_products (Category, SKU, Competitor Price)
  - dim_time (Month, Quarter, Seasonality)

## 📊 Key Insights & Deliverables

_(To be updated as project progresses)_

- **Competitor Analysis:** Real-time comparison of our SKU prices vs. major market competitors.
- **Churn Risk:** A generated list of "High Risk" customers enabling the marketing team to target them with retention offers.
- **Sales Forecasting:** Trend analysis identifying seasonal spikes in specific product categories.

---

## ⚙️ Setup & Installation

0. Prerequisites : Ensure you have Python 3.9+ and PostgreSQL installed locally.

### 1️⃣ Install Python Libraries

```bash
pip install -r requirements.txt
```

### 2️⃣ Database Setup

Create a database named retail_db in PostgreSQL. Then, run the schema script:

```bash
psql -U postgres -d retail_db -f sql/schema.sql
```

### 3️⃣ Running the Pipeline

#### Step 1: Scrape fresh data

```bash
python scripts/01_scraper.py
```

#### Step 2: Clean and Load to SQL

```bash
python scripts/02_etl_cleaning.py
```

#### Step 3: Run Analysis Open models/churn_prediction.ipynb in Jupyter Lab.

---

## 📌 Future Improvements

    Dockerization: Containerize the scraper to run on a cloud server.

    Airflow: Orchestrate the scraping job to run daily automatically.

    Deep Learning: Experiment with LSTM models for more accurate time-series forecasting.
