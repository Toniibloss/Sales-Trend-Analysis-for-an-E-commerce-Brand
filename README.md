
# Sales Trend Analysis & Forecasting for an E-commerce Brand

## Overview
This project analyzes and visualizes over 500,000 e-commerce transactions to uncover business insights and forecast future sales trends.  
It covers data cleaning, exploratory data analysis (EDA), and time series forecasting using ARIMA and Prophet models.

The goal is to help business stakeholders make data-driven decisions around inventory, pricing, and marketing strategies.

---

## Objectives
- Clean and preprocess raw transaction data.
- Analyze sales performance across products, countries, and time.
- Identify top-performing items and key revenue-generating markets.
- Build forecasting models to project future sales.
- Generate actionable insights for business improvement.

---

## Dataset
**Records:** 541,909  
**Columns:**
| Column | Description |
|---------|-------------|
| InvoiceNo | Unique invoice number |
| StockCode | Product identifier |
| Description | Product name |
| Quantity | Number of items purchased |
| InvoiceDate | Date and time of purchase |
| UnitPrice | Price per unit |
| CustomerID | Unique customer identifier |
| Country | Customer’s country |

---

## Data Preparation
- Removed missing `CustomerID` values.
- Converted `InvoiceDate` to datetime format.
- Filtered canceled transactions (negative quantities).
- Created `TotalPrice = Quantity × UnitPrice`.
- Aggregated sales by day and month.

---

## Exploratory Data Analysis
- **Revenue Trends:** Visualized daily and monthly fluctuations.
- **Top Products:** Identified best-selling products by revenue.
- **Regional Insights:** Determined top-performing countries.
- **Customer Patterns:** Studied purchasing frequency and volume.

**Key Insights:**
- UK contributed ~80% of total revenue.  
- Strong sales peaks during November–December (holiday season).  
- Top 5 SKUs made up over 30% of total revenue.

---

## Forecasting
Implemented two forecasting models:
1. **ARIMA (SARIMAX)** – statistical time series forecasting.
2. **Prophet** – seasonal and trend-based forecasting.

Predicted the next 6 months of total monthly revenue to anticipate growth and plan business operations accordingly.

---

## Tools and Technologies
- **Python**
- **Pandas**, **NumPy** – data processing
- **Matplotlib**, **Seaborn** – visualization
- **Statsmodels**, **Prophet** – forecasting
- **Jupyter Notebook** – analysis and presentation

---

## Project Structure
