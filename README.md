# IKEA Data Analysis Project | SQL Server, Python & Power BI

## Disclaimer

**IKEA Gifting** is a fictional business concept created for this educational data analytics project. This project is not affiliated with, endorsed by, or representative of the actual IKEA corporation. All financial figures, customer metrics, and business insights are calculated from a publicly available, anonymized transactional dataset and do not represent IKEA's actual business performance. IKEA-inspired branding is used solely for dashboard design and visualization purposes.

---

## Project Overview

I developed this end-to-end data analytics project to simulate a real-world business intelligence engagement for a fictional UK-based gifting and home décor e-commerce business, **IKEA Gifting**.

The primary objective was to transform raw transactional data into actionable business insights by integrating SQL Server, Python, and Power BI into a unified analytics workflow.

I used SQL Server for data cleaning and validation, Python for customer analytics and segmentation, and Power BI to build an interactive dashboard that helps business stakeholders understand customer behavior, revenue distribution, and customer retention.

The project demonstrates how I applied data analytics techniques to solve business problems, from defining requirements and preparing raw data to developing customer segments and presenting insights through interactive visualizations.

## Business Problem

The business needed a structured way to identify its most valuable customers, understand purchasing behavior, and recognize customers at risk of churning.

Without a clear view of customer value and retention patterns, the business could struggle to prioritize marketing campaigns and develop effective customer retention strategies.

I addressed this problem by developing an analytics workflow centered on customer segmentation, revenue analysis, and churn identification.

## Business Questions

Through this project, I explored the following questions:

- Who are the most valuable customers, and how much revenue do they contribute?
- Which customers have become inactive and may be at risk of churning?
- How do revenue, customer value, and retention change over time?
- How do customer segments and purchasing patterns vary across geographic markets?
- What retention strategies could be recommended for different customer segments?

## Key Findings

Based on the project's analytical results:

- **Customer value concentration:** The Champions segment represents approximately 22% of customers while contributing nearly 68% of total revenue.
- **Customer churn:** The calculated churn rate is approximately 50.86%, using a 90-day inactivity threshold.
- **Customer segmentation:** Average customer value varies considerably across segments, highlighting differences in purchasing behavior and revenue contribution.
- **Seasonal revenue patterns:** Revenue shows noticeable spikes during the fourth quarter, suggesting seasonal purchasing trends within the gifting category.

These findings can help the business prioritize high-value customers, investigate declining engagement, and plan targeted retention campaigns.

*Note: These figures are derived from the analytical results of this project and should be validated against the final cleaned dataset and dashboard.*

## Dataset

**Dataset:** Online Retail II  
**Source:** UCI Machine Learning Repository  
**Original contributor:** Daqing Chen  
**Coverage:** December 2009 – December 2011  
**Dataset size:** Approximately 1.07 million transaction records  
**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

The dataset contains anonymized transactional records from a UK-based, non-store online retailer selling giftware for various occasions.

I selected this dataset to work with realistic data quality challenges and demonstrate how transactional data can be transformed into meaningful customer and business insights.

## Tools and Technologies

| Technology | Application |
|---|---|
| SQL Server | Data import, cleaning, deduplication, validation, and exploratory analysis |
| SQL Server Management Studio (SSMS) | Writing and executing SQL queries |
| Python | Customer analytics, RFM scoring, segmentation, and churn identification |
| Pandas | Data manipulation and analytical transformations |
| Jupyter Notebook | Developing and documenting the Python analysis |
| Power BI Desktop | Creating interactive business intelligence dashboards |
| DAX | Developing measures for revenue, customer counts, churn, and customer value |

## Core Concepts Implemented

### 1. Data Cleaning and Validation
I processed the raw transactional dataset using SQL Server, addressing data quality issues such as inconsistent date formats, invalid values, duplicate records, and missing customer identifiers.

I used SQL conversion functions and window functions to standardize data types, identify duplicate transactions, and validate the cleaned dataset.

### 2. RFM Analysis
I implemented **Recency, Frequency, and Monetary (RFM) analysis** to evaluate customer purchasing behavior.

- **Rec
