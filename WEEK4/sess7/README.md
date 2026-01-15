# 💾 SESSION 7 & 8 - INTRO TO FEATURE ENGINEERING AND MODEL THINKING

Week 4 Session 7 focuses on feature engineering, Preprocessing and Model Thinking - Preparing datasets for future machine learning 

## 📌 Session Coverage

### 🔹 Feature Engineering
- Creating new features from existing data
- Date-based and aggregation features
- Feature selection (keeping relevant features, dropping unnecessary ones)
- Understanding the impact of features on model performance

### 🔹 Encoding & Scaling
- Identifying categorical and numerical features

- When and why to encode categorical variables

- When and why to scale numerical features

- Common techniques:

    - One-hot encoding
    - Standard scaling
    - Min-max scaling
      
- Importance of preprocessing before modeling

### 🔹 Introduction to Model Thinking

- Understanding supervised vs unsupervised learning

- Identifying types of target variables:

    - Regression
    - Binary classification
    - Multiclass classification
    - Matching datasets to problem types

- Thinking about models conceptually before training

### 🔹 Pipelines (Conceptual)

- Organizing preprocessing steps in a structured workflow
- Avoiding common mistakes
- Preparing for future model training

## Mini Project

### 📌 Project Structure

This mini project has two parts:

  Part 1: Practice on the dataset you've been working on

  Part 2: Apply skills to a brand-new dataset

🔹 Part 1 — Feature Engineering & Model Thinking (Practice)

 Dataset

🏪 Warehouse and Retail Sales – Montgomery County

You have already:

Cleaned the dataset

Handled missing values

Parsed dates

Performed EDA and visualization

This part focuses on the next stage of the data science workflow.

🎯 Tasks (Part 1)

Feature Engineering

Create at least 3 new meaningful features

Examples:

Date-based features (day, month, year)

Aggregated features (e.g. total sales per category)

 Encoding Decisions

Identify which columns need encoding

State the type of encoding you would use and why (No need to implement the code)

Scaling Decisions

Identify which numerical features may need scaling.

Model Thinking

Identify a suitable target variable

State the problem type and explain your reasoning in 3–5 sentences

## 📌 Project Solution

### Part 1:
- Feature Engineering was already performed on the data set during data cleaning

Columns that need encoding:

- Item Type column should be encoded using One Hot Encoding because it is a nominal categorical variable

Other categorical Variables has too many unique columns that One Hot Encoder will create man columns so it is better to use more advanced encoding methods or drop the columns.

Scaing Decisions:

Numerical Features that need Scaling:

  - Retail Transfers
  - Warehouse Sales
  - Total Sales(Engineered Columns)

Model Thinking

1. Problem Type:
This project aims to address a Regression problem. Regression is a type of supervised machine learning task where the goal is to predict a continuous numerical output value based on input features.

2. Target Variable:
The primary target variable for our prediction model is RETAIL SALES. This column represents the continuous numerical value of sales generated through retail channels for each item in the dataset.

3. Reasoning for Choosing Regression:
Our objective is to forecast or estimate the exact RETAIL SALES amount for individual items. Since RETAIL SALES is a continuous numerical variable (it can take on any value within a range, not just a few discrete categories), a regression approach is the most appropriate methodology. We are not merely classifying an item into a category (e.g., 'high sales' or 'low sales'), but rather attempting to predict the specific dollar amount it will generate in retail sales.

  - Impact on Feature Selection and Data Preparation:
  Choosing RETAIL SALES as the target variable has direct implications for our feature set and data preprocessing steps:
  
  - Target Variable Isolation: The RETAIL SALES column will be separated from the feature set (X) to serve as the ground truth (y) for  
  model training and evaluation.
  
  - Data Leakage Prevention:
  
     - The TOTAL SALES column must be excluded from the feature set. TOTAL SALES is often a sum of different sales components (including
         RETAIL SALES and WAREHOUSE SALES), and its inclusion would introduce severe data leakage, leading to an artificially inflated model performance that would not generalize to unseen data.
  
   -  Feature Transformation:
  
      Categorical features (SUPPLIER, ITEM DESCRIPTION, ITEM TYPE) will undergo appropriate encoding (e.g., One-Hot Encoding) to convert them into a numerical format suitable for regression models.
      Numerical features (YEAR, RETAIL TRANSFERS, WAREHOUSE SALES) will be scaled (e.g., using StandardScaler or MinMaxScaler) to ensure consistent ranges and improve model convergence and performance.
      Other Columns like Item Code and Date should be dropped because they are not directly useful in predicting the target variable.

## Part 2

### Project Overview 
 This is a mini project designed to test our knowledge on data cleaning, EDA, and feature engineering 
The dataset was the popular housing dataset from kaggle 

### Key Insights 
It was discovered that houses far from the coast were cheaper than houses near the ocean and on the islands.
Houses on the island had the smallest dara points but the highest average price, this shows that houses tend to be more costly than houses on the Inland.
It was also discovered that the median income and median house value were strongly positively correlated; this shows that the higher your income, the more luxury bome you will be able to afford.
I created a new column which i called Bedroom per room which shows the bedroom to room ratio; the lower the ratio, the bigger the house, i.e, many other rooms for work and fun.
The bedroom per room column was strongly negatively correlated with median income after taking away some inconsistent values gotten from feature creation; this simply means the higher your income, the bigger the house you will buy, because you would want to have rooms for other things like home office, home gym etc.
I created a second column which i called rooms per household, i.e, shows how much people can be accommodated in a room. This column was strongly negatively correlated with bedroom to room ratio, this makes sense in the real world because the bigger your house, the more people you would be able to accommodate.
