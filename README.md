# 🧹 Online Retail II Data Wrangling Case Study: From Messy Transactions to Data Gold

## Project Structure

```
online-retail-ii-wrangling-1/
│
├── datasets/
│ ├── online_retail_ii_2009-2010.csv.zstd # Raw dataset (2009–2010)
│ ├── online_retail_ii_2010-2011.csv.zstd # Raw dataset (2010–2011)
│ └── online-retail-ii-cleaned.csv.zstd # Cleaned dataset (wrangling results)
│
├── notebooks/
│ └── code.ipynb # Main data wrangling notebook
│
├── environment.yml # Environment dependencies (conda)
├── README.md # Project documentation
```

## Overview

This project is a data wrangling case study on the **Online Retail II** dataset. The goal is to transform raw transaction data into a clean, structured, and reusable analytical dataset for various data-driven projects.

The initial dataset contained various data quality issues such as missing values, duplication, canceled transactions, and extreme values ​​in numeric variables. Therefore, a series of data wrangling processes were performed to improve the quality and consistency of the dataset before it was used in further analysis.

## Dataset

The dataset used is **Online Retail II** from the UCI Machine Learning Repository.

[https://archive.ics.uci.edu/dataset/502/online+retail+ii](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

This dataset contains online retail transactions from a UK-based company from 2009–2011, with over 1 million transactions.

## Project Objectives

This project aims to:

* Identify data quality issues in retail transaction datasets
* Implement data wrangling steps (discovering, structuring, cleaning, enriching, validating)
* Produce a clean and reusable analytical dataset for various data-driven projects

## What is Data Wrangling

Data wrangling is the process of cleaning, structuring, and enriching raw data to create a clean, consistent dataset ready for analysis, visualization, and machine learning.

Reference:
[https://www.ibm.com/think/topics/data-wrangling](https://www.ibm.com/think/topics/data-wrangling)

## Tools & Libraries

* Python
* Pandas
*Seaborn
* Matplotlib

## Data Wrangling Workflow

### Discovering

* Dataset overview
* Missing values ​​analysis
* Duplicate detection
* Unique value exploration
* Invoice anomaly detection
* Outlier visualization

### Structuring

* Rename columns
* Type conversion
* Memory optimization

### Cleaning

* Remove duplicates
* Fill in missing description
* Handle missing CustomerID
* Add guest indicators

### Enriching

* Time-based feature engineering
* Business flags (cancellation, adjustment, negative values)
* TotalPrice calculation

### Validating

* Recheck missing values
* Outlier detection (IQR)
* Final dataset Verification

## Final Results

Final dataset:

* 1,033,036 transactions
* 23 variables
* No missing values
* Consistent data structure
* Complete business and temporal features

The dataset is saved in the following format:

```bash
online-retail-ii-cleaned.csv.zstd
```

## Data Dictionary (Cleaned Dataset)

| Column | Description |
| --------------------- | ------------------------------------- |
| InvoiceID | Transaction ID |
| StockCode | Product Code |
| Description | Product Name |
| Quantity | Number of products |
| InvoiceDate | Transaction Date |
| Price | Price per unit |
| CustomerID | Customer ID |
| Country | Customer Country |
| IsGuest | Anonymous Customer Indicator |
| Hour–MonthName | Temporal Feature |
| IsNegQty / IsNegPrice | Negative value indicator |
| IsCanceled | Cancellation indicator |
| IsAdjusted | Adjustment indicator |
| TotalPrice | Transaction value |
| IsQuantityOutlier | Outlier Quantity |
| IsPriceOutlier | Outlier Price |

# Further Development

This wrangled dataset can be used for:

| Area | Project Ideas |
| ------------------- | --------------------------------- |
| Customer Analytics | RFM Segmentation |
| Predictive Modeling | Sales Forecasting |
| Predictive Modeling | Regression Modeling |
| Customer Value | Customer Lifetime Value |
| Recommendation | Product Recommendation |
| Market Basket | Association Rules |
| Anomaly Detection | Fraud Detection |
| BI | Interactive Dashboard |
| Geospatial | Country Analysis |

## Key Insight

The wrangled dataset serves as:

* Analytical dataset
* Gold data layer
* Foundation dataset for various data science projects