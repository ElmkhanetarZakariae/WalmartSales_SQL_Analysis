# WalmartSales_SQL_Analysis

This project aims to analyze Walmart's sales data to identify top-performing branches and products, examine sales trends across different product categories, and better understand customer behavior. The goal is to explore ways to enhance and optimize sales strategies. The dataset used in this analysis comes from the Kaggle Walmart Sales Forecasting Competition (https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting) 

In this competition, participants are given historical sales data from 45 Walmart stores in various regions. Each store features multiple departments, and the task is to forecast sales for each department at each location. To increase the challenge, the dataset includes selected holiday markdown events, which are known to influence sales, but predicting their impact on specific departments and the extent of the effect is a complex task.

# Project Objective
The objective of this project is to analyze Walmart's sales data in order to identify the factors that impact sales performance across different branches. Through this analysis, the project seeks to uncover insights that can guide the improvement and optimization of sales strategies for various store locations.

# Approach used

# 1. Data Wrangling:
The first step is data inspection to ensure that any NULL or missing values are identified. Appropriate methods are then applied to handle these missing values, either by replacing or removing them.
- Build a database and create tables to store the data.
- Insert the data into the tables and then identify any columns containing NULL values. In this case, since the tables were created with the NOT NULL constraint, NULL values are automatically excluded during insertion.
# 2. Feature Engineering:
This step focuses on creating new columns from existing data to provide more insights into the sales trends.
- Time of Day: A new column, time_of_day, is added to categorize sales into Morning, Afternoon, and Evening. This helps answer the question of which part of the day generates the most sales.
- Day of the Week: A column, day_name, is created to extract and store the day of the week on which a transaction occurred (e.g., Mon, Tue, Wed). This helps identify the busiest days of the week for each branch.
- Month of the Year: Another column, month_name, is created to extract and store the month of the year (e.g., Jan, Feb, Mar). This can help determine which months see the highest sales and profits.
# 3. Exploratory Data Analysis (EDA):
EDA is performed to answer the key business questions and goals of the project. This involves summarizing the main characteristics of the dataset, visualizing trends, and analyzing the relationship between various factors, such as sales, time of day, and day of the week.
This approach ensures that the dataset is clean and enriched with meaningful features, allowing for a deeper analysis and better insights into sales performance across different stores and times.

# Business Questions To Answer

# Generic Question

- How many unique cities does the data have?
- In which city is each branch?

# Product

- How many unique product lines does the data have?
- What is the most common payment method?
- What is the most selling product line?
- What is the total revenue by month?
- What month had the largest COGS?
- What product line had the largest revenue?
- What is the city with the largest revenue?
- What product line had the largest VAT?
- Fetch each product line and add a column to those product line showing "Good", "Bad". Good if its greater than average sales
- Which branch sold more products than average product sold?
- What is the most common product line by gender?
- What is the average rating of each product line?

# Sales

- Number of sales made in each time of the day per weekday
- Which of the customer types brings the most revenue?
- Which city has the largest tax percent/ VAT (Value Added Tax)?
- Which customer type pays the most in VAT?

# Customer

- How many unique customer types does the data have?
- How many unique payment methods does the data have?
- What is the most common customer type?
- Which customer type buys the most?
- What is the gender of most of the customers?
- What is the gender distribution per branch?
- Which time of the day do customers give most ratings?
- Which time of the day do customers give most ratings per branch?
- Which day fo the week has the best avg ratings?
- Which day of the week has the best average ratings per branch?
