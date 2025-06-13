# Sales-Analysis
This project is a comprehensive sales analysis of a pizza business using a transactional dataset. The project aims to uncover insights into sales trends, customer preferences, and product performance. SQL is used for data querying and report generation, while Power BI is used for dashboard visualization, DAX measures, and Power Query for data cleaning and modeling. This project is built to showcase the capability of end-to-end business intelligence workflows and is aimed to be used as part of a professional data analytics portfolio.

##  Problem Statement
### KPI's Requirement
  1. <b>Total Revenue:</b> The sum of the total price of all pizza orders.
  2. Average Order Value: The average amount spent per order, calculated by dividing the total revenue by the total number of orders.
  3. Total Pizzas Sold: The sum of the quantities of all pizzas sold.
  4. Total Orders: The total number of orders placed.
  5. Average Pizzas Per Order: The average number of pizzas sold per order, calculated by dividing the total number of pizzas sold by the total number of orders.
  We would like to visualize various aspects of our pizza sales data to gain insights and understand key trends. We have identified the following requirements for creating charts:
### Charts Requirement
  1. Daily Trend for Total Orders:Create a bar chart that displays the daily trend of total orders over a specific time period. This chart will help us identify any patterns or fluctuations in order volumes on a daily basis.
  2. Monthly Trend for Total Orders:Create a line chart that illustrates the hourly trend of total orders throughout the day. This chart will allow us to identify peak hours or periods of high order activity.
  3. Percentage of Sales by Pizza Category:Create a pie chart that shows the distribution of sales across different pizza categories. This chart will provide insights into the popularity of various pizza categories and their contribution to overall sales.
  4. Percentage of Sales by Pizza Size:Generate a pie chart that represents the percentage of sales attributed to different pizza sizes. This chart will help us understand customer preferences for pizza sizes and their impact on sales.
  5. Total Pizzas Sold by Pizza Category:Create a funnel chart that presents the total number of pizzas sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.
  6. Top 5 Best Sellers by Revenue, Total Quantity and Total Orders:Create a bar chart highlighting the top 5 best-selling pizzas based on the Revenue, Total Quantity, Total Orders. This chart will help us identify the most popular pizza options.
  7. Bottom 5 Best Sellers by Revenue, Total Quantity and Total Orders:Create a bar chart showcasing the bottom 5 worst-selling pizzas based on the Revenue, Total Quantity, Total Orders. This chart will enable us to identify underperforming or less popular pizza options.

## Tools & Technologies Used
- Excel: For basic dataset overview and schema verification.
- Microsoft SQL Server: For querying, filtering, and preparing data reports.
- Power Query: For data cleaning and transformation.
- DAX (Data Analysis Expressions): For building measures and calculated fields.
- Power BI Desktop: For creating interactive dashboard visualizations.

## Processes Involved
1. Data Collection
- A CSV dataset of pizza sales transactions was used, containing fields like order_id, date, pizza_name, category, size, price, and quantity.
2. Data Cleaning & Preprocessing (Power Query)
- Removed inconsistencies in  size fields.
- Extracted additional columns like month and day.
3. DAX Measures
- Total Revenue = SUM(quantity * price)
- Total Orders = DISTINCTCOUNT(order_id)
- Total Pizzas Sold = SUM(quantity)
- Average Order Value = [Total Revenue] / [Total Orders]
- Average Pizzas Per Order = [Total Pizzas Sold] / [Total Orders]
4. Data Analysis with SQL
- Created SQL queries for:
  - Total revenue and total orders
  - Monthly/daily trend of orders
  - Top/Bottom 5 pizzas by quantity/revenue/orders
  - Pizza category and size analysis
5. Dashboard Creation (Power BI)
- Page 1: Overall KPIs, Daily Trend, Pizza Category Sales, Sales by Size
- Page 2: Funnel Chart, Top/Bottom 5 Best Sellers
- Used slicers for time range and pizza category filters
- Used buttons to navigate between dashboard pages

## Dashboard Interaction
Home Dashboard
![Dashboard page 1](https://github.com/user-attachments/assets/ef76bfe7-e8cc-4ccd-8a81-f8555147eb47)
Best/Worst Seller Dashboard
![Dashboard page 2](https://github.com/user-attachments/assets/c70c4ef7-5113-4eaa-962f-71f5662ca8ce)

## Conclusion
This project effectively demonstrates the ability to perform end-to-end business intelligence using a sales dataset. The insights derived from the analysis can help stakeholders:
- Optimize inventory and product offerings
- Focus on best-selling products
- Identify underperforming items
- Make data-driven marketing and pricing decisions

@Prepared by: Priyambada Acharya

