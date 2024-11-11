## CAPSTONE-PROJECT
# PROJECT TITLE:SALES ANALYSIS

## OUTLINES
---
[SYNOPSIS](#synopsis)

[OVERVIEW](#overview)

[DATA DESCRIPTION](#data-description)

[TOOLS USED](#tools-used)

[DATA CLEANING AND PREPARATION](#data-cleaning-and-preparation)

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
---
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

### TOOLS USED
---
1) Microsoft Excel(xlxs)
   - Data Cleaning
   - Pivot Tables
   - Analysis
   - Data Visualization.
2) Structured Query Language(SQL)
   - Quering Data
3) Power BI
   - Data Cleaning,
   - Data Visualization
   - For Reporting
4) GitHub
   - Portfolio Building

### DATA CLEANING AND PREPARATION
---
In the Preliminary Stage of the Data cleaning and preparations, we implemented the following actions:-
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
