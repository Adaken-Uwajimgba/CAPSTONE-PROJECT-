## CAPSTONE-PROJECT
# PROJECT TITLE:SALES ANALYSIS

## OUTLINES
---
[SYNOPSIS](#synopsis)

[OVERVIEW](#overview)

[DATA DESCRIPTION](#data-description)

[APPROACH](#approach)

[EXPLORATORY DATA ANALYSIS](#exploratory-data-analysis)

[DATA ANALYSIS](#data-analysis)


### SYNOPSIS
---
The aim of this Data Analysis is to evaluate the Sales Performance of a Retail store over a Specified Period of Time. The Dataset encompasses a detailed view of customer Orders, Product,Region and the Sales/Revenue generated. The Sales Data provided will be used to Identify Monthly Sales Key Trends, uncovering Key Insights Such as Regional Performance,Top-Selling Products e.t.c


### OVERVIEW
---
#### Problem Outline
This Project is charged to conduct a comprehensive Sales Analysis to identify  factors contributing to it's current performance so as to make informed Decisions concerning the next moves to make that will be beneficial to the Retail store.

#### Goals
1) To Uncover Critical Insights such as identifying the Top-selling Products, the top-selling Regions
2) To understand the underlying trends and how they impact on Sales
3) To Predict future trends based on Customer Preference and Sales pattern

### DATA DESCRIPTION
---
#### Data Sources
The Data source used for this Analysis is the Data Sales.csv files and this is an open source Data that can be freely downloaded from any open source Platform such as [Kaggle](https://www.kaggle.com/datasets),[FRED](https://appsource.microsoft.com/en-us/product/office365/wa200003692?tab=overview) e.t.c

#### Data Characteristics
- OrderID: A distinct identifier for each order.
- CustomerId: A distinct identifier for each customer placing an order.
- Product: The particular item purchased in each transaction.
- Region: The geographical location (i.e North, South, East, West) where the order was placed.
- OrderDate: The date when the order was made.
- Quantity: The number of units purchased for each product in an order.
- UnitPrice: The price per unit of the product.
- Total Sales: The total sales value for the order: calculated as Quantity * UnitPrice


### APPROACH
---
#### Tools Used
1) [Microsoft Excel(xlxs)](https://www.microsoft.com/en-us/microsoft-365/excel)
   - Data Cleaning
   - Pivot Tables
   - Analysis
   - Data Visualization.
2) Structured Query Language([SQL](https://www.microsoft.com/en-us/sql-server/sql-server-2022))
   - Quering Data
3) [Power BI](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads)
   - Data Cleaning,
   - Data Visualization
   - For Reporting

#### Data Cleaning And Preparation
In the Initial Part of the Data cleaning and preparations, we implemented the following actions:-
- i) Data loading and Inspection
- ii) Removal of Duplicates
- iii) Data cleaning and Formatting


### EXPLORATORY DATA ANALYSIS
---
EDA consists of the exploring of this Data to give Answers to some questions such as;
- Retrieve the total Sales for each Product Category
- Find the number of sales transactions in each region
- Find the Highest-selling Product by total Sales value
- Calculate total Revenue per Product
- Calculate Monthly Sales totals for the Current Year
- Find the Top 5 Customers by total Purchase amount
- Calculate the Percentage of Total Sales contributed by each Region
- Identify Products with no Sales in the Last Quarter

### DATA ANALYSIS
---
This is where we include some Basic lines of code/Queries or even some of the DAX expressions used during the Analysis;
```SQL
SELECT product,
SUM(Total_revenue) AS TOTAL_Revenue
from
[dbo].[LITA PROJECT_1-SALES Analysis]
GROUP BY product
```
```SQL
SELECT TOP 1 Product,
SUM(Total_Revenue)AS Total_Revenue
from [dbo].[LITA PROJECT_1-SALES Analysis]
Group by Product
ORDER BY Total_Revenue DESC
```
#### Using SQL For Data Analysis
Below are the uploaded screenshots of each query which we ran while exploring the Data.
First we create our Database called 
```SQL
CREATE DATABASE LITA PROJECT1_SALES
```
- Query 1;Retrieve the total Sales for each Product Category
 ![Screenshot (20)](https://github.com/user-attachments/assets/1341cac3-fc96-4021-ac3d-fcc1a2b99c1e)

- Query 2;Find the Number of Sales transactions in each Region
![Screenshot (21)](https://github.com/user-attachments/assets/4f151216-c3a3-4e33-8c60-179450163654)

- Query 3;Find the highest selling Product by Total sales value
![Screenshot (22)](https://github.com/user-attachments/assets/7f714999-cff3-4c47-a38d-717a05b96133)

- Query 4;Calculate total Revenue per Product
![Screenshot (23)](https://github.com/user-attachments/assets/e85e269f-dc2d-4c1b-977b-95d1c5451d6f)

- Query 5;Calculate Monthly sales totals for the current year
![Screenshot (24)](https://github.com/user-attachments/assets/c711d666-1e70-4d02-9f20-3b3774091f9b)

- Query 6;Find the Top 5 Customers by Total Purchase Amount
![Screenshot (25)](https://github.com/user-attachments/assets/11fa45c6-7e88-4bbb-8e00-b1c09fbd4c2b)

- Query 7;Calculate the Percentage(%) of Total Sales contributed by each Region
![Screenshot (26)](https://github.com/user-attachments/assets/c32308ad-4fa1-4cb7-8ad7-cb01a9868445)

- Query 8;Identify products with no sales in the Last Quarter
![Screenshot (27)](https://github.com/user-attachments/assets/7f7363d7-23e7-4f38-a838-ddfa18704ffb)




