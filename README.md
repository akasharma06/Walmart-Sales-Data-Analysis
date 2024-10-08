# **Walmart Sales Data Analysis**

**Project Overview**

This project aims to explore Walmart's sales data to identify top-performing branches and products, analyze sales trends across different product categories, and understand customer behaviour. The goal is to derive insights that can be used to improve and optimize sales strategies.

**Project Objectives**

The primary objective of this project is to gain insights into the sales data of Walmart stores, focusing on the factors that influence sales performance across different branches and product lines.

**Dataset Description**

| **Column Name**             | **Description**                               | **Data Type**       |
|-----------------------------|-----------------------------------------------|---------------------|
| `invoice_id`                | Invoice ID for the sales transaction          | VARCHAR(30)         |
| `branch`                    | Branch where the sale occurred                | VARCHAR(5)          |
| `city`                      | Location of the branch                        | VARCHAR(30)         |
| `customer_type`             | Type of customer making the purchase          | VARCHAR(30)         |
| `gender`                    | Gender of the customer                        | VARCHAR(10)         |
| `product_line`              | Product line of the sold item                 | VARCHAR(100)        |
| `unit_price`                | Price per unit of the product                 | DECIMAL(10, 2)      |
| `quantity`                  | Number of units sold                          | INT                 |
| `VAT`                       | Value-added tax on the purchase               | DECIMAL(6, 4)       |
| `total`                     | Total cost of the purchase                    | DECIMAL(12, 5)      |
| `date`                      | Date of the purchase                          | DATE                |
| `time`                      | Time of the purchase                          | TIMESTAMP           |
| `payment_method`            | Payment method used                           | VARCHAR(15)         |
| `cogs`                      | Cost of goods sold                            | DECIMAL(10, 2)      |
| `gross_margin_percentage`   | Gross margin percentage                       | DECIMAL(11, 9)      |
| `gross_income`              | Gross income from the sale                    | DECIMAL(12, 4)      |
| `rating`                    | Customer rating                               | DECIMAL(2, 1)       |

**Analysis Approach**

**Data Preparation and Enhancement:**
- Inspect the data for NULL or missing values and apply appropriate data cleaning techniques.
- Ensure data integrity by handling missing values, duplicates, and inconsistencies.
- Create new columns to generate additional insights from the existing data:
  - `time_of_day`: Categorize sales into Morning, Afternoon, and Evening to analyze peak sales times.
  - `day_name`: Extract the day of the week for each transaction to determine the busiest days.
  - `month_name`: Track sales and profitability trends by month.

**Exploratory Data Analysis (EDA):**
- Perform detailed analysis to address the project's objectives and answer key business questions.

**Key Business Questions**

- **Generic Questions:**
  - How many unique cities are represented in the data?
  - In which city is each branch located?

- **Product Analysis:**
  - How many unique product lines are present?
  - What is the most common payment method?
  - Which are the top 5 most selling product line?
  - What is the total revenue by month?
  - Which product line generates the largest revenue?
  - What is the contribution of cities in revenue?
  - What is the average tax by product line?
  - Which branch sold more products than the average product?
  - Which is the most common product line by gender?
  - What is the average rating of each product line? 
 
- **Sales Analysis:**
  - Total number of sales made per time of the day on each weekday
  - Which customer type contributes the most revenue?
  - Which city has the largest tax percentage?

- **Customer Analysis:**
  - How many unique customer types are in the dataset?
  - How many sales were made by each customer type?
  - Which customer type had the highest average rating?
  - What does each customer type generate in total revenue?
  - Which gender has the highest average unit price?
  - How many sales were made in each city by the 'member' customer type?
  - What is the total gross income for each customer type and city?
  - Which customer type and city combination has the highest total tax amount?
  - Find the average unit price and quantity for each customer type. Which customer type has the highest average unit price and quantity?
  - Identify the customer type that has generated the highest gross margin percentage.
  - Find the total tax amount for each city and identify the customer type that contributed the most tax in each city.
  - What is the total revenue for the highest-grossing customer type in each city?
  - Which city has the highest total gross income from the 'normal' customer type, and what is that total?
