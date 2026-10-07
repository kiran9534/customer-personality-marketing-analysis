# Customer Personality & Marketing Campaign Analysis

## Overview

This project looks at customer purchasing behavior and marketing campaign response for a consumer/e-commerce business.

The main goal was to move from a raw customer dataset to a cleaner dataset, understand how customers behave, compare people who responded to campaigns with those who did not, and create customer segments that could support more targeted marketing.

## Business questions

- Who are the higher-value customers?
- How does income relate to spending?
- Which product categories contribute most to spending?
- Which campaigns have the strongest response?
- Do campaign responders purchase more?
- Do customer characteristics differ between responders and non-responders?
- Can customers be grouped into meaningful segments based on their behavior?

## Dataset

The project uses a 2,240-record customer dataset containing demographic information, product spending, purchase channels, campaign responses, and customer dates.

The cleaned dataset contains additional fields created during analysis, including:
- Age
- Total Spending
- Total Purchases
- Total Campaigns Accepted
- Children
- Parental Status
- Customer Tenure
- Campaign Responder

## Tools

- Python
- Pandas and NumPy
- Matplotlib / Seaborn / Plotly
- Jupyter Notebook
- SQL / MySQL
- Power BI
- Excel

## What I did

1. Inspected the dataset and checked data types, missing values, duplicates, and unusual records.
2. Converted the customer date field into a proper date format.
3. Filled missing income values using the median.
4. Flagged unusually high income values for analysis.
5. Created calculated fields for age, total spending, total purchases, campaign acceptance, children, parental status, and customer tenure.
6. Compared campaign responders with non-responders.
7. Built charts to understand product spending, purchase channels, and campaign response.
8. Prepared the cleaned dataset for further SQL and Power BI analysis.
9. Used PCA and K-Means clustering to create four customer segments based on spending and purchase behavior.

## Key findings

- Campaign 4 was the strongest of the five campaigns, with 167 customer acceptances.
- Customers who responded to at least one campaign spent about ₹1,097 on average, compared with about ₹478 for non-responders.
- Responders also made about 16.7 purchases on average, compared with about 11.5 for non-responders.
- The analysis was used to support a four-segment customer grouping for targeted marketing.

These figures are based on the project data and analysis included in this repository.

## Files

- `notebooks/Marketing_campaign.ipynb` — Python analysis and data preparation
- `data/customer_personality_cleaned.csv` — cleaned analysis dataset
- `data/marketing_project.xlsx` — Excel working file
- `customer-personality-analysis.pbix` — Power BI dashboard
- `requirements.txt` — Python packages used for the notebook

## Reproducing the Python analysis

Install the packages in `requirements.txt`, open the notebook, and run the cells using the included dataset as the input.

The public notebook copy intentionally does not contain database passwords or other credentials. If a database connection is needed, credentials should be stored locally using environment variables.

## Portfolio takeaway

This project demonstrates the full analytics workflow I want to use as a Data Analyst: cleaning data, exploring customer behavior, answering business questions, segmenting customers, and communicating the results through dashboards.
