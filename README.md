# IKEA Data Analysis Project | SQL Server, Python & Power BI

<img width="986" height="622" alt="image" src="https://github.com/user-attachments/assets/582d8e8f-adc9-4746-a01b-91c8197279a4" />
<img width="987" height="620" alt="image" src="https://github.com/user-attachments/assets/47bea829-8726-4a69-a92c-a30f55bef24e" />
<img width="987" height="621" alt="image" src="https://github.com/user-attachments/assets/ae9c4536-5c30-447e-a8ca-d49b5c36d7f8" />



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

Core Concepts Implemented

1. Data Cleaning and Validation

I processed the raw transactional dataset using SQL Server, addressing data quality issues such as inconsistent date formats, invalid values, duplicate records, and missing customer identifiers.

I used SQL conversion functions and window functions to standardize data types, identify duplicate transactions, and validate the cleaned dataset.

2. RFM Analysis

I implemented Recency, Frequency, and Monetary (RFM) analysis to evaluate customer purchasing behavior.

Recency: How recently a customer made a purchase.

Frequency: How often a customer purchased.

Monetary: How much a customer spent.

I calculated these metrics for individual customers and assigned scores on a 1–5 scale to support customer evaluation and segmentation.

3. Customer Segmentation

Using the RFM scores, I grouped customers into six business-oriented segments:

Champions

Loyal

At Risk

New

Needs Attention

Lost

This segmentation helps distinguish high-value customers from customers who may require additional engagement or retention efforts.

4. Churn Analysis

I implemented a rule-based churn indicator using a 90-day inactivity threshold.

This approach identifies customers who have not purchased recently, allowing the business to investigate potential retention opportunities.

The metric represents inactivity-based churn under the project's chosen definition, rather than confirmed customer attrition.

5. Business Intelligence and Data Visualization

I prepared an analysis-ready dataset combining transactional information with customer segmentation results.

Using Power BI and DAX, I developed interactive visualizations to monitor business performance, compare customer segments, and analyze trends over time.

Project Workflow

Step 1: Business Requirements and Planning

I defined the business problem, analytical objectives, key performance indicators, and business questions before beginning the technical implementation.

This helped align the data preparation and visualization stages with the intended business outcomes.

Step 2: Data Cleaning and Exploration Using SQL Server

I imported the raw transaction data into SQL Server and performed data preparation and validation.

My work included:

Standardizing inconsistent date formats.

Converting columns to appropriate data types.

Identifying and removing duplicate records.

Handling invalid transaction values.

Investigating missing customer identifiers.

Validating record counts throughout the cleaning process.

The original project analysis reports the removal of 32,907 exact duplicate rows. I retained row-count validation as part of the data quality workflow.

Step 3: Customer Analytics Using Python

I used Python and Pandas to calculate customer-level Recency, Frequency, and Monetary metrics.

I then scored customers across the three RFM dimensions, assigned them to six customer segments, and created a churn indicator based on 90 days of inactivity.

The resulting customer-level analysis provided the foundation for the dashboard's segmentation and retention metrics.

Step 4: Dashboard Development Using Power BI

I integrated the customer segmentation results with the cleaned transactional data to prepare a dataset for reporting.

I developed a three-page Power BI report containing headline KPIs, revenue trends, customer segmentation analysis, and churn-related visualizations.

I also incorporated interactive filters and navigation features to make the report easier to explore.

Dashboard Structure

Page 1: Home

The home page introduces the project and provides navigation to the main report pages.

It also includes a glossary explaining key concepts such as Recency, Frequency, Monetary value, and churn.

Page 2: Business Overview

This page provides a high-level view of business performance through key metrics, including:

Total customers

Total revenue

Customer churn percentage

Average customer value

It also includes customer and revenue comparisons, segment-level breakdowns, and monthly, quarterly, and yearly trends.

Interactive filters allow users to explore results by date, country, customer segment, and churn status.

Page 3: RFM Analysis

This page focuses on customer segmentation and customer value.

It includes:

Customer count by segment

Revenue contribution by segment

Average RFM scores

Average customer value across segments

Churn trends over time

These visualizations help identify high-value customer groups and segments that may need targeted retention strategies.
