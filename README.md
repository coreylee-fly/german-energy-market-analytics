# German Energy Market Analytics & Forecasting

## Project Status

This project is currently in the initial development stage.

The initial project structure has been created. The next steps are data collection, data cleaning, exploratory data analysis, SQL modeling, dashboard development, and machine learning forecasting.

## Project Overview

This project analyzes the German electricity market using public energy market data and weather data.

The goal is to build an end-to-end data analytics and machine learning project that demonstrates:

- Python data processing
- SQL-based analysis
- Exploratory data analysis
- Power BI dashboard development
- Time-series feature engineering
- Machine learning forecasting
- Professional project organization with Git and GitHub

## Main Questions

This project will investigate:

1. How does German electricity generation vary by hour, weekday, month, and season?
2. What is the relationship between renewable energy generation and electricity prices?
3. How do solar and wind generation patterns differ over time?
4. How does electricity demand change during different time periods?
5. Can electricity demand or electricity price be forecast using historical energy and weather data?
6. Which features are most important for forecasting?

## Planned Data Sources

Planned data sources include:

- SMARD electricity market data
  - electricity generation
  - electricity consumption/load
  - renewable generation
  - day-ahead electricity price
  - power plant generation data

- Historical weather data
  - temperature
  - wind speed
  - solar radiation
  - cloud cover
  - precipitation

Large raw data files may not be uploaded to GitHub. Instead, the repository will document how to download and reproduce the data.

## Planned Workflow

### 1. Data Collection

- Download SMARD market data
- Download power plant generation data
- Download historical weather data
- Store raw files in `data/raw/`

### 2. Data Cleaning

- Parse datetime columns
- Standardize column names
- Handle missing values
- Convert units if necessary
- Align datasets to hourly timestamps

### 3. Data Integration

- Merge generation, consumption, price, and weather data
- Create hourly analysis dataset
- Create daily aggregated dataset
- Save processed files in `data/processed/`

### 4. SQL Analysis

- Create database schema
- Import processed data into SQL tables
- Write analytical SQL queries
- Create SQL views for dashboard usage

### 5. Exploratory Data Analysis

Planned analysis topics:

- Total electricity generation over time
- Renewable vs conventional generation
- Electricity consumption patterns
- Electricity price trends
- Weekday and weekend differences
- Seasonal patterns
- Relationship between renewable generation and electricity price

### 6. Feature Engineering

Planned features:

- Hour of day
- Day of week
- Month
- Weekend indicator
- Holiday indicator
- Lag features
- Rolling averages
- Weather features
- Renewable generation share

### 7. Machine Learning Forecasting

Planned target variables:

- Electricity demand
- Electricity price

Planned models:

- Baseline model
- Linear Regression
- Random Forest
- XGBoost or LightGBM

Planned metrics:

- MAE
- RMSE
- MAPE
- R² score

### 8. Power BI Dashboard

Planned dashboard pages:

1. Market Overview
2. Renewable Energy Analysis
3. Electricity Price Analysis
4. Forecasting Results

## Project Structure

```text
german-energy-market-analytics/
├── app/
├── dashboard/
├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
├── models/
├── notebooks/
├── reports/
├── sql/
├── src/
│   └── energy_market/
├── tests/
├── .gitignore
├── LICENSE
├── Makefile
├── pyproject.toml
├── README.md
└── requirements.txt