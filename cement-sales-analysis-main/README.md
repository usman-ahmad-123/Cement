Cement Sales Analysis & ETL Pipeline

""Python Version" (https://img.shields.io/badge/Python-3.11%2B-blue)" (https://www.python.org/)
""License: MIT" (https://img.shields.io/badge/License-MIT-yellow.svg)" (https://opensource.org/licenses/MIT)

Project Overview

This project analyzes monthly cement sales data from 2010 to 2022 to identify sales trends, seasonal patterns, operational performance, and key economic drivers. The project also develops an ETL (Extract, Transform, Load) pipeline, calculates business KPIs, performs statistical and regression analysis, and forecasts cement sales for the next 12 months using a Time Series Forecasting model (Prophet).

The project demonstrates practical skills in Data Analytics, Data Engineering, SQL, Statistical Analysis, Machine Learning, Time Series Forecasting, and Business Intelligence, making it suitable for showcasing capabilities for Data Analyst and Data Scientist internship opportunities.

---

Project Structure

.
├── 📊 dashboard/
│   └── dashboard.pbix
├── 💾 data/
│   ├── processed/
│   │   ├── cement_factory.db
│   │   └── cleaned_cement_data.csv
│   ├── query_results/
│   │   ├── gdp_correlation.csv
│   │   ├── kpi_efficiency.csv
│   │   ├── low_efficiency.csv
│   │   ├── production_gap.csv
│   │   └── yearly_summary.csv
│   └── raw/
│       └── raw_cement_data.csv
├── 📓 notebooks/
│   ├── 01_analysis_and_forecasting.ipynb
│   └── 02_sql_query_examples.ipynb
├── 🔍 sql_queries/
│   ├── gdp_correlation.sql
│   ├── kpi_efficiency.sql
│   ├── low_efficiency.sql
│   ├── production_gap.sql
│   └── yearly_summary.sql
├── 🛠️ src/
│   ├── __init__.py
│   ├── data_cleaner.py
│   └── pipeline.py
├── .gitignore
├── 📝 README.md
└── 📦 requirements.txt

Directory Description

- 📊 "dashboard/" — Contains the Power BI dashboard used for interactive data visualization and business reporting.
- 💾 "data/" — Stores datasets throughout different stages of the data pipeline:
  - "raw/" — Original, unmodified source data.
  - "processed/" — Cleaned and transformed datasets in CSV and SQLite formats.
  - "query_results/" — Analytical datasets generated from SQL queries.
- 📓 "notebooks/" — Contains Jupyter Notebooks for exploratory data analysis, forecasting, statistical analysis, and SQL demonstrations.
- 🔍 "sql_queries/" — Contains modular SQL scripts for KPI calculations, efficiency analysis, production gaps, GDP relationships, and yearly summaries.
- 🛠️ "src/" — Contains the core Python source code for data cleaning and ETL pipeline execution.
- 📦 "requirements.txt" — Lists the Python libraries and dependencies required to run the project.

---

Dataset

- Source: "Kaggle – Cement Sales Demand" (https://www.kaggle.com/datasets/kishorkhengare/cement-sales-demand)
- Time Period: 2010–2022
- Frequency: Monthly
- Key Variables: Production, Sales, Demand, GDP, Population, Interest Rate, and other economic indicators
- Raw Data Location: "data/raw/raw_cement_data.csv"

---

Methodology & Workflow

1. Data Ingestion & ETL Pipeline

Developed a Python-based ETL pipeline using Pandas to:

- Ingest raw cement sales data.
- Clean and preprocess the dataset.
- Handle missing values and inconsistencies.
- Transform the data into an analysis-ready format.
- Load the processed data into a SQLite database.

The resulting database is stored at:

"data/processed/cement_factory.db"

2. Exploratory Data Analysis

Performed comprehensive EDA using Pandas, Matplotlib, and Seaborn to identify:

- Long-term sales trends.
- Monthly and seasonal patterns.
- Production and demand behavior.
- Year-over-year changes.
- Relationships between sales and economic indicators.

3. KPI Analysis

Designed SQL queries to calculate and monitor key operational KPIs, including:

- Production Efficiency
- Demand Fulfillment
- Production Gap
- Yearly Sales Performance
- Low-Efficiency Periods

These metrics provide insights into production performance and the organization's ability to satisfy market demand.

4. Economic & Cost Driver Analysis

Applied Ridge Regression using Scikit-learn to analyze the relationship between cement sales and macroeconomic variables such as:

- GDP
- Interest Rate
- Population
- Other relevant economic indicators

This analysis helps identify the factors most strongly associated with changes in cement sales.

5. Sales Forecasting

Implemented Prophet, a time-series forecasting model, to predict cement sales for the next 12 months.

The forecasting process considers historical trends and recurring seasonal patterns to generate future sales estimates.

6. Business Intelligence & Visualization

Developed an interactive Power BI dashboard to present:

- Sales trends
- Production performance
- Demand fulfillment
- KPI performance
- Economic indicators
- Forecasted sales

The dashboard enables users to explore the data interactively and derive actionable business insights.

---

Key Findings & Business Insights

- Sales demonstrated a consistent long-term growth trend, accompanied by clear seasonal fluctuations.
- Seasonal demand patterns were evident, with sales generally reaching higher levels during the middle of the year.
- Production Efficiency and Demand Fulfillment remained above 95%, indicating strong operational performance and effective demand management.
- GDP emerged as one of the strongest economic factors associated with cement sales, highlighting the relationship between economic activity and construction-material demand.
- The forecasting model projected approximately 5–8% sales growth for the following year, suggesting continued positive demand under the modeled conditions.

---

Technology Stack

Category| Technologies
Programming| Python 3.11+
Data Manipulation| Pandas, NumPy
Data Visualization| Matplotlib, Seaborn
Database| SQLite
Query Language| SQL
Machine Learning| Scikit-learn, Ridge Regression
Forecasting| Prophet
Business Intelligence| Power BI
Development Environment| Jupyter Notebook, VS Code

---

Project Highlights

This project demonstrates an end-to-end analytics workflow:

Raw Data → Data Cleaning → ETL Pipeline → SQLite Database → SQL Analysis → Statistical/ML Analysis → Forecasting → Power BI Dashboard

It combines technical data-processing capabilities with business-oriented analysis to transform raw cement-industry data into actionable insights.
