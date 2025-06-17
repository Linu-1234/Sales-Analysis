# Sales-Analysis
This project is a comprehensive sales analysis of a pizza business using a transactional dataset. The project aims to uncover insights into sales trends, customer preferences, and product performance. SQL is used for data querying and report generation, while Power BI is used for dashboard visualization, DAX measures, and Power Query for data cleaning and modeling. This project is built to showcase the capability of end-to-end business intelligence workflows and is aimed to be used as part of a professional data analytics portfolio.

##  Problem Statement
### KPI's Requirement
  1. <b>Total Revenue:</b> The sum of the total price of all pizza orders.
  2. <b>Average Order Value:</b> The average amount spent per order, calculated by dividing the total revenue by the total number of orders.
  3. <b>Total Pizzas Sold:</b> The sum of the quantities of all pizzas sold.
  4. <b>Total Orders:</b> The total number of orders placed.
  5. <b>Average Pizzas Per Order:</b> The average number of pizzas sold per order, calculated by dividing the total number of pizzas sold by the total number of orders.
### Charts Requirement
1. <b>Daily Trend for Total Orders:</b> Create a bar chart that displays the daily trend of total orders over a specific time period. This chart will help us identify any patterns or fluctuations in order volumes on a daily basis.
2. <b>Monthly Trend for Total Orders:</b> Create a line chart that illustrates the hourly trend of total orders throughout the day. This chart will allow us to identify peak hours or periods of high order activity.
3. <b>Percentage of Sales by Pizza Category:</b> Create a pie chart that shows the distribution of sales across different pizza categories. This chart will provide insights into the popularity of various pizza categories and their contribution to overall sales.
4. <b>Percentage of Sales by Pizza Size:</b> Generate a pie chart that represents the percentage of sales attributed to different pizza sizes. This chart will help us understand customer preferences for pizza sizes and their impact on sales.
5. <b>Total Pizzas Sold by Pizza Category:</b> Create a funnel chart that presents the total number of pizzas sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.
6. <b>Top 5 Best Sellers by Revenue, Total Quantity and Total Orders:</b> Create a bar chart highlighting the top 5 best-selling pizzas based on the Revenue, Total Quantity, Total Orders. This chart will help us identify the most popular pizza options.
7. <b>Bottom 5 Best Sellers by Revenue, Total Quantity and Total Orders:</b> Create a bar chart showcasing the bottom 5 worst-selling pizzas based on the Revenue, Total Quantity, Total Orders. This chart will enable us to identify underperforming or less popular pizza options.

## Tools & Technologies Used
1. <b>Excel:</b> For basic dataset overview and schema verification.
2. <b>Microsoft SQL Server:</b> For querying, filtering, and preparing data reports.
3. <b>Power Query:</b> For data cleaning and transformation.
4. <b>DAX:</b> For building measures and calculated fields.
5. <b>Power BI Desktop:</b> For creating interactive dashboard visualizations.

## Processes Involved
### Data Collection
- A CSV dataset of pizza sales transactions was used, containing fields like order_id, date, pizza_name, category, size, price, and quantity.
### Data Cleaning & Preprocessing (Power Query)
- Removed inconsistencies in  size fields.
- Extracted additional columns like month and day.
### DAX Measures
- Total Revenue = SUM(quantity * price)
- Total Orders = DISTINCTCOUNT(order_id)
- Total Pizzas Sold = SUM(quantity)
- Average Order Value = [Total Revenue] / [Total Orders]
- Average Pizzas Per Order = [Total Pizzas Sold] / [Total Orders]
### Data Analysis with SQL
- Created SQL queries for:
  - Total revenue and total orders
  - Monthly/daily trend of orders
  - Top/Bottom 5 pizzas by quantity/revenue/orders
  - Pizza category and size analysis
### Dashboard Creation (Power BI)
- Page 1: Overall KPIs, Daily Trend, Pizza Category Sales, Sales by Size
- Page 2: Funnel Chart, Top/Bottom 5 Best Sellers
- Used slicers for time range and pizza category filters
- Used buttons to navigate between dashboard pages

## Dashboard Interaction
#### Home Dashboard


![Dashboard page 1](https://github.com/user-attachments/assets/ef76bfe7-e8cc-4ccd-8a81-f8555147eb47)


#### Best/Worst Seller Dashboard


![Dashboard page 2](https://github.com/user-attachments/assets/c70c4ef7-5113-4eaa-962f-71f5662ca8ce)



## Insights
### 🧾 Page 1: Sales Overview Dashboard
- 🔹 KPIs
  - Total Revenue: ₹817.86K
  - Average Order Value: ₹38.31
  - Total Pizzas Sold: 49,574
  - Total Orders: 21,350
  - Average Pizzas Per Order: 2.32
- 📅 Daily Trend for Total Orders
  - Orders steadily increase from Sunday to Friday.
  - Friday shows the highest number of orders (~3.5K).
  - Sunday has the lowest order count (~2.6K).
- 📈 Monthly Trend for Total Orders
  - Highest orders in July and January.
  - September and October see a noticeable drop in orders.
  - Seasonal patterns may exist — ideal for targeting promotions.
- 🍕 Percentage of Sales by Pizza Category
  - Classic: 26.91% (Top-selling category)
  - Supreme: 25.46%
  - Chicken: 23.96%
  - Veggie: 23.68%
- 🍕 Percentage of Sales by Pizza Size
  - Large: 45.89% (Most preferred)
  - Medium: 30.49%
  - Regular: 21.77%
  - X-Large: 1.72%
  - XX-Large: 0.12%
- 📊 Total Pizzas Sold by Category-
  - Classic: 14,888
  - Supreme: 11,987
  - Veggie: 11,649
  - Chicken: 11,050
- 🗓️ Busy Days and Times
  - Days: Maximum orders on Friday and Saturday evenings.
  - Months: Peak sales during July and January.
- 🏆 Sales Performance Highlights
  - Category: Classic contributes to maximum sales and total orders.
  - Size: Large-size pizzas generate the highest sales.
### 🧾 Page 2: Best/Worst Sellers Dashboard
- 🥇 Top 5 Pizzas by Revenue
  - The Thai Chicken Pizza – ₹43K
  - The Barbecue Chicken Pizza – ₹43K
  - The California Chicken Pizza – ₹41K
  - The Classic Deluxe Pizza – ₹38K
  - The Spicy Italian Pizza – ₹35K
- 🥇 Top 5 Pizzas by Quantity
  - The Classic Deluxe Pizza – 2.5K
  - The Barbecue Chicken Pizza – 2.4K
  - The Hawaiian Pizza – 2.4K
  - The Pepperoni Pizza – 2.4K
  - The Thai Chicken Pizza – 2.4K
- 🥇 Top 5 Pizzas by Orders
  - The Classic Deluxe Pizza – 2.3K
  - The Hawaiian Pizza – 2.3K
  - The Pepperoni Pizza – 2.3K
  - The Barbecue Chicken Pizza – 2.3K
  - The Thai Chicken Pizza – 2.2K
- 🧊 Bottom 5 Pizzas by Revenue
  - The Brie Carre Pizza – ₹12K
  - The Green Garden Pizza – ₹14K
  - The Spinach Supreme Pizza – ₹15K
  - The Mediterranean Pizza – ₹15K
  - The Spinach Alfredo Pizza – ₹16K
- 🧊 Bottom 5 Pizzas by Quantity
  - The Brie Carre Pizza – 490
  - The Mediterranean Pizza – 933
  - The Calabrese Pizza – 937
  - The Spinach Supreme Pizza – 950
  - The Soppressata Pizza – 961
- 🧊 Bottom 5 Pizzas by Orders
  - The Brie Carre Pizza – 480
  - The Mediterranean Pizza – 912
  - The Spinach Supreme Pizza – 918
  -  The Calabrese Pizza – 918
  - The Chicken Caesar Pizza – 938


## Conclusion
This project effectively demonstrates the ability to perform end-to-end business intelligence using a sales dataset. The insights derived from the analysis can help stakeholders:
- Optimize inventory and product offerings
- Focus on best-selling products
- Identify underperforming items
- Make data-driven marketing and pricing decisions

@Prepared by: Priyambada Acharya

