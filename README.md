Walmart Sales Data Analysis
Project Overview
This project aims to explore Walmart's sales data to identify top-performing branches and products, analyze sales trends across different product categories, and understand customer behavior. The goal is to derive insights that can be used to improve and optimize sales strategies.

Project Objectives
The primary objective of this project is to gain insights into the sales data of Walmart stores, focusing on the factors that influence sales performance across different branches and product lines.

Dataset Description
Column Name	Description	Data Type
invoice_id	Invoice ID for the sales transaction	VARCHAR(30)
branch	Branch where the sale occurred	VARCHAR(5)
city	Location of the branch	VARCHAR(30)
customer_type	Type of customer making the purchase	VARCHAR(30)
gender	Gender of the customer	VARCHAR(10)
product_line	Product line of the sold item	VARCHAR(100)
unit_price	Price per unit of the product	DECIMAL(10, 2)
quantity	Number of units sold	INT
VAT	Value-added tax on the purchase	FLOAT(6, 4)
total	Total cost of the purchase	DECIMAL(10, 2)
date	Date of the purchase	DATE
time	Time of the purchase	TIMESTAMP
payment_method	Payment method used	DECIMAL(10, 2)
cogs	Cost of goods sold	DECIMAL(10, 2)
gross_margin_percentage	Gross margin percentage	FLOAT(11, 9)
gross_income	Gross income from the sale	DECIMAL(10, 2)
rating	Customer rating	FLOAT(2, 1)
Analysis Approach
Data Preparation and Enhancement:

Inspect the data for NULL or missing values and apply appropriate data cleaning techniques.
Ensure data integrity by handling missing values, duplicates, and inconsistencies.
Create new columns to generate additional insights from the existing data:
time_of_day: Categorize sales into Morning, Afternoon, and Evening to analyze peak sales times.
day_name: Extract the day of the week for each transaction to determine the busiest days.
month_name: Track sales and profitability trends by month.
Exploratory Data Analysis (EDA):

Perform detailed analysis to address the project's objectives and answer key business questions.
Key Business Questions
Generic Questions:

How many unique cities are represented in the data?
In which city is each branch located?
Product Analysis:

How many unique product lines are present?
What is the most common payment method?
Which product line has the highest sales?
What is the total revenue generated each month?
Which month recorded the highest cost of goods sold (COGS)?
Which product line generated the highest revenue?
Which city recorded the highest revenue?
Which product line had the largest VAT contribution?
How do product lines compare against average sales ("Good" or "Bad")?
Which branch exceeded average product sales?
What is the most common product line by gender?
What is the average customer rating for each product line?
Sales Analysis:

What are the sales trends by time of day and weekday?
Which customer type contributes the most revenue?
Which city has the highest VAT percentage?
Which customer type pays the most in VAT?
