Amazon Sales Data Analysis with Microsoft Excel
Project Overview
This project analyzes an Amazon product dataset using Microsoft Excel. The objective was to clean raw data, identify data quality issues, calculate key performance indicators, answer business questions, and build an interactive dashboard to present the results.
The project demonstrates practical Excel skills commonly used in data analysis, including data cleaning, Pivot Tables, Pivot Charts, dashboard design and business reporting.
Project Objectives
Clean and prepare the dataset for analysis
Identify and handle missing values
Remove duplicate records
Transform text data into usable fields
Convert raw text into structured data
Calculate key perfomance indicators
Analyse product categories
Create an interactive dashboard
Present Business insights based on the analysis
Dataset
*SOURCE* https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset
The dataset contains information about Amazon products, including:
-Product ID
-Product Name
-Product Category
-Selling Price
-Original Price
-Discount Percentage
-Customer Rating
-Product Description
-Review Information

Data Cleaning Process

Several data cleaning steps were performes before the analysis:
1.Duplicate Check
-Checked the dataset for duplicate records.
-No duplicate rows remained after validation
2.Missing Values
Missing values were identified using the "COUNTBLANK()" function.
Results:
-Rating: 1 missing value
-Rating Count: 2missing values
-All other colums contained no missing values.
To ensure data quality, the three incomplete records wetre removd before the analysis.
3.Data Transformatio0n
A new column called "main category" was created by extracting the first category from the original "category" column.
Formula used:
=LEFT([@category],FIND("|",[@category])-1)
4.Price Conversion
The currency symbol was removed from the price colums and both price fields were converted into numeric values for calculations.

Key Performance Indicators
The dasboard includes the following KPIs:
-Total Products
-Average Rating 
-Average Selling Price
-Average Discount

Business Questions
The analysis answers the following questions:
Which main category contains the highest number of products?
Which main category has thE HIGHEST AVERAGE CUSTOMER RATING?
Which main category has the highest average discount?
Which main category has the highest average selling price?

Key Insights
"ELECTRONICS" contains the highest number of products(509), making it the largest category in the dataset.
"OFFICE PRODUCTS" has the highest average customer rating(4.31) , indicating the highest customer satisfaction among the analysed categories.
"HOME IMPROVEMENT" offers the highest average discount(57.50%), sugesting a morew aggresive pricing strategy.
"ELECTRONICS" has the highest average selling price(6079.48), making it the most expensive category on average.

Summary
Overall, Electronics dominates the dataset in both product count and average selling price, while, Home Improvement stands out for its significat discounts. Office Products accived the highest average customer ratings.

DASHBOARD
The dashboard was created using:
-Pivot Tables
-Pivot Charts
-KPI Cards
-Excel Tables
-Interactive dashboard using Exel Slicers
Dashboard Previw
![Dashboard](dashboard.png)





