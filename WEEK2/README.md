#🛒 Warehouse and Retail Sales Performance - initial EDA

## Assignment Goal
The objective of this assignment was to understand the dataset

## Data Source
**Source:** Kaggle
**Dataset Name:** Warehouse and Retail Sales
**Original Size:** 307645 rows

## ✨Insights from Initial Analysis
- using the head() function, I noticed that the first five items have the same month and same year and their retail sales are almost the same value
- using the tail() function, I noticed that the last item code has an odd name
- we have 8 columns, 307645 rows in the dataset, we have three columns that have missing values which are (supplier, item type and retail sales)
- we have 3 different data types which are (int, floats and object data type)
- The year column has the highest mean which is meant to be a date data type column while the warehouse sales column has an unusually low minimum
### Column Names ###
 0   YEAR              307645 non-null  int64  
 1   MONTH             307645 non-null  int64  
 2   SUPPLIER          307478 non-null  object 
 3   ITEM CODE         307645 non-null  object 
 4   ITEM DESCRIPTION  307645 non-null  object 
 5   ITEM TYPE         307644 non-null  object 
 6   RETAIL SALES      307642 non-null  float64
 - what is the item type with the highest total sales? Liquor has the highest total sales, it also had the highest volue of sales
 7   RETAIL TRANSFERS  307645 non-null  float64
 8   WAREHOUSE SALES   307645 non-null  float64 
