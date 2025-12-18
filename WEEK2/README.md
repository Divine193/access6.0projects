#🛒 Warehouse and Retail Sales Dataset

## Assignment for week 2 Session 3
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
 - 0   YEAR              307645 non-null  int64  
 - 1   MONTH             307645 non-null  int64  
 - 2   SUPPLIER          307478 non-null  object 
 - 3   ITEM CODE         307645 non-null  object 
 - 4   ITEM DESCRIPTION  307645 non-null  object 
 - 5   ITEM TYPE         307644 non-null  object 
 - 6   RETAIL SALES      307642 non-null  float64
 - 7   RETAIL TRANSFERS  307645 non-null  float64
 - 8   WAREHOUSE SALES   307645 non-null  float64
- what is the item type with the highest total sales? Liquor has the highest total sales, it also had the highest volume of sales

# Assignment for Week 2 Session 4

## Assignment Objective
- Clean the dataset and prepare it for Exploratory Data Analysis

## Data Cleaning Deliverables
### Handling Missing Values
- I filled the missing item in the ITEM TYPE column with 'WINE' which is the correct item that should be there according the item description column
- I filled the missing values under RETAIL SALES column with the mode
- I filled the missing values under the SUPPLIER column with the word 'UNKNOWN'
### Checking For Duplicates
- There were no duplicate rows in this dataset
### Feature Engineering
- I created two new columns- DATE column and a TOTAL SALES COLUMN
### Saving The Dataset
- I saved my new and cleaned dataset as Cleaned_Sales_Data.csv 
