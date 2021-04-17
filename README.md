# Amazon_Vine_Analysis
## Overview of Project
### Purpose:  Analyze Amazon reviews written by members of the paid Amazon Vine program.
### Background:
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Specifically, this project completes the following tasks and provides stakeholders with actionable insights.

- Use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 
- use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset

## Resources
Software:  PySpark, RDS(AWS), pgAdmin, 
Amazon Review datasets, challenge_schema.sql, Amason_Reviews_ETL_starter_code.ipynb

## Analysis
### Deliverable 1:

First, I created an AWS RDS database with tables in pgAdmin, choosing the "home improvement" dataset from the Amazon Review datasets. The dataset was extracted and transfered into four seperate Dataframes that matched a table schema in pre-coded in pgAdmin. The transformed data was loaded into the appropriate tables and checked by queries to confirm successful upload.

Tables created: 
![Customer_Table](https://github.com/Quinneth/Amazon_Vine_Analysis/blob/main/Customer_Table.png)
![Products_Table](https://github.com/Quinneth/Amazon_Vine_Analysis/blob/main/Products_Table.png)
![Vine_Table](https://github.com/Quinneth/Amazon_Vine_Analysis/blob/main/Vine_Table.png)<br>

### Deliverable 2:


## Results
- Total reviews of helpful votes:  39095  
- Total of Paid reviews = 26573
- Total of unpaid reviews 12522
- Total 5-star reviews:  18371 
- Total 5-star paid reviews: 13199
- Total 5-star unpaid reviews: 5172
- Total Percentage of 5-star reviews:  46.99%
- Percentage of 5-star Vine reviews:  49.67%
- Percentage of 5-star non-vine reviews: 41.30%
## Summay

The similarity of the Vine program percentage compared to the non-Vine program percentage indicates minimal bias. Further analysis should be conducted by involving more sample data to see if this assumption persists.
