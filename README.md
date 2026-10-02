# Sales Data Analytics

## Sales Performance, Data Quality & Profitability Analysis

An end-to-end sales analytics project using Python and Power BI to clean sales transaction data, validate data quality, identify outliers, and analyze order value, cost, and profitability.

## Project Overview

The project works with sales transaction data containing information about:

* Country
* Order value
* Cost
* Date
* Category
* Customer
* Sales manager
* Sales representative
* Device type
* Order ID

The analysis focuses on transforming raw sales data into a reliable dataset for business reporting and profitability analysis.

## Dataset

* **Original records:** 1,001
* **Final records:** 1,000
* **Original columns:** 10
* **Final analytical columns:** 18

## Data Cleaning

The Python workflow includes:

* Checking missing values
* Detecting and removing duplicate records
* Standardizing column names
* Cleaning text fields
* Standardizing categorical values
* Converting financial fields to numeric format
* Converting dates to a consistent datetime format
* Handling missing order values
* Handling missing cost values
* Filling missing device types
* Validating business rules

## Outlier Detection

The project uses the **Interquartile Range (IQR)** method to identify potential outliers in:

* Order value
* Cost
* Cost-to-order-value ratio

The analysis identified **18 outlier rows**.

Outliers are flagged for investigation rather than automatically removed.

## Business Rule Validation

A business rule was used to identify records where:

**Cost > Order Value**

The validation found no records where cost exceeded order value.

## Profitability Analysis

The project calculates:

### Gross Margin

```text
Gross Margin = Order Value - Cost
```

### Gross Margin Percentage

```text
Gross Margin % = (Gross Margin / Order Value) × 100
```

These metrics support profitability analysis at the transaction level.

## Power BI Dashboard

The cleaned sales dataset was used to create a Power BI dashboard for sales and profitability reporting.

The dashboard can be used to analyze sales performance across dimensions such as:

* Country
* Category
* Sales manager
* Sales representative
* Device type
* Time
* Order value
* Cost
* Gross margin

## Tools & Technologies

* Python
* Pandas
* NumPy
* Power BI
* Data Cleaning
* Exploratory Data Analysis
* Outlier Detection
* Business Rule Validation
* Profitability Analysis
* Data Visualization
* Business Intelligence

## Project Workflow

**Raw Sales Data → Data Quality Checks → Cleaning → Standardization → Outlier Detection → Business Validation → Profitability Analysis → Power BI Dashboard**

## Repository Contents

| File                   | Description                                |
| ---------------------- | ------------------------------------------ |
| `SALES_DATA.ipynb`     | Python data cleaning and analysis notebook |
| `sales_dashboard.pbix` | Power BI sales dashboard                   |

> The original Excel source dataset is not included unless permission is available to publish it publicly.

## Skills Demonstrated

* Python Data Analysis
* Pandas
* NumPy
* Data Cleaning
* Data Validation
* Outlier Detection
* Feature Engineering
* Profitability Analysis
* Power BI
* Business Intelligence
* Data-Driven Analysis
