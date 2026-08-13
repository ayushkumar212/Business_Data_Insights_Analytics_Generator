# AI Data Insights Generator

## Project Overview

AI Data Insights Generator is a data analytics project built to transform raw business sales data into meaningful business insights, risk analysis, recommendations, and an interactive-style dashboard.

The project uses the Sample Superstore dataset and follows a complete analytics workflow from data exploration and cleaning to business insights, reporting, and dashboard visualization.

## Objectives

- Explore and understand the business dataset.
- Clean and prepare the data for analysis.
- Analyze sales, profit, margins, returns, categories, products, and yearly performance.
- Identify important business and product-level risks.
- Generate actionable business recommendations.
- Create an executive-level final business report.
- Build a dashboard containing key performance indicators and visualizations.

## Project Workflow

The project is organized into six Jupyter notebooks:

1. `01_Data_Exploration.ipynb`
   - Initial dataset exploration
   - Data structure and column inspection
   - Basic descriptive analysis

2. `02_Data_Cleaning.ipynb`
   - Data cleaning and preparation
   - Creation of analysis-ready data

3. `03_Exploratory_Data_Analysis.ipynb`
   - Sales and profit analysis
   - Category and sub-category analysis
   - Product-level analysis
   - Yearly and business performance analysis

4. `04_Insight_Generation.ipynb`
   - Business insight generation
   - Risk identification
   - Product risk scoring
   - Business recommendations
   - JSON business insights output

5. `05_Final_Report.ipynb`
   - Executive summary
   - Key business risks
   - Critical product risks
   - Business recommendations
   - Product recommendations
   - Final business report generation

6. `06_Dashboard.ipynb`
   - Dashboard KPIs
   - Business risk visualizations
   - Product risk visualizations
   - Sales and profit analysis
   - Category profitability
   - Monthly sales and profit trends

## Dataset

The project uses the Sample Superstore dataset.

Main dataset:

`SampleSuperstore.csv`

The cleaned dataset is stored in:

`data/SampleSuperstore_Cleaned.csv`

The final analysis dataset contains 5,901 records and 22 columns.

Important fields include:

- Order information
- Customer information
- Category and sub-category
- Product information
- Sales
- Quantity
- Profit
- Payment mode
- Returned status
- Shipping days

## Key Business Results

The generated analysis identified:

- Total Sales: **$1,565,804.32**
- Total Profit: **$175,262.11**
- Profit Margin: **11.19%**
- Return Rate: **4.86%**
- Critical Business Risks: **3**
- Warning Business Risks: **1**

### Major Business Risks

The analysis identified profitability concerns in areas including:

- Binders
- Machines
- Tables
- Paper
- Art

The analysis also identified broader category-level concerns involving Office Supplies, Furniture, and Technology.

### Critical Product Risks

High-risk products included:

- Ibico EPK-21 Electric Binding System
- GBC Ibimaster 500 Manual ProClick Binding System
- Fellowes PB500 Electric Punch Plastic Comb Binding Machine with Manual Bind
- Ibico Hi-Tech Manual Binding System

These products showed significant profitability concerns and require further review of pricing, discounts, costs, and profitability.

## Generated Reports

The project generates the following reports in the `reports` directory:

- `business_insights.json`
- `final_business_report.json`
- `Final_Business_Report.md`

These files contain the generated business insights, executive summary, risks, and recommendations.

## Dashboard

The dashboard contains:

- Total Sales KPI
- Total Profit KPI
- Profit Margin KPI
- Return Rate KPI
- Critical Risk KPI
- Warning Risk KPI
- Top Business Risks by Profit Change
- Top Product Risks by Risk Score
- Sales vs Profit by Category
- Profit Margin by Category
- Monthly Sales & Profit Trend

## Project Structure

```text
AI_Data_Insights_Generator/
│
├── 01_Data_Exploration.ipynb
├── 02_Data_Cleaning.ipynb
├── 03_Exploratory_Data_Analysis.ipynb
├── 04_Insight_Generation.ipynb
├── 05_Final_Report.ipynb
├── 06_Dashboard.ipynb
│
├── data/
│   └── SampleSuperstore_Cleaned.csv
│
├── reports/
│   ├── business_insights.json
│   ├── final_business_report.json
│   └── Final_Business_Report.md
│
├── charts/
├── screenshots/
├── src/
├── notebooks/
├── venv/
│
├── SampleSuperstore.csv
├── README.md
└── .gitignore