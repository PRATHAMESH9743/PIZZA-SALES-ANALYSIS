# PIZZA SALES ANALYSIS - SQL SERVER 2023 / POWER BI

This project delves deep into the realm of data analysis, utilizing SQL and Power BI to uncover crucial insights into Pizza sales. The featured eye-catching dashboards aid the pizza business in making informed decisions and strategic workforce planning, providing substantial benefits to the business.

Source Data:
pizza sales.csv
The source data contained Pizza sales 48621 records of year 2015. This is included in the repository.

## Database and Tools
1. MySQL
2. POWER BI

## PROBLEM STATEMENT
Analyze the key indications for our pizza sales data to gain insights into our business performance. specifically, to calculate the following metrices:

1. Total Revenue:
   
   The sum of the total price of all pizza orders.
2. Average Order Value:
   
   The average amount spent per order, calculate by dividing the total revenue by the total numbers of orders.
3. Total Pizzas Sold:
   
   The sum of the quantities of all pizzas sold.
4. Total orders:
   
   The total numbers of orders placed.
5. Average Pizzas Per Order:
   
   The average number of pizzas sold per order, calculated by dividing the total number of pizzas sold  by the total numbers of orders.

 ## CHARTS REQIREMENTS
 To visualize various aproach of our pizza sales data to gain insights and understand key trends. we have identified the following requirements for creating charts:

1. Daily Trend For Total Orders:

   Create a bar chart that displays the daily trend of total orders over a specific time period. this chart will help us identify any patterns or fluctuations in order volumes on a daily 
   basis.
3. Monthly Trend for Total Orders:

   Create a line chart that illustrates the hourly trend of total orders throughout the day. This chart will allow us to identify peak hours or periods of high order activity.
5. Percentage of Sales by Pizza Category:

   Create a pie chart that shows the distribution os sales across different pizza categories. this chart will provide insights into the popularity of various pizza categories and their 
   contributions to overall sales      
4. Percentage of Sales by pizza size:

   Generate a pie chart that represents the percentage of sales attributed to different pizza sizes. this chart will help us undertsand customer preferences for pizza sizes and their impact 
   on sales.
5. Total Pizzas Sold by Pizza Category:

   Create a funnel chart that presents the total number of pizza sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.
6. Top 5 Best Sellers by Revenue, Total Quality and Total Orders:

   Create a bar chart highlighting the top 5 best selling pizza based on the revenue. Total Quantity, Total Orders. This chart will help us identify the most popular pizza options.
7.  Bottom 5 Worst Sellers by Revenue, Total Quality and Total Orders:

    Create a bar chart showcasing the bottom 5 worst selling pizza based on the revenue. Total Quantity, Total Orders. This chart will help us identify the most popular pizza options.

## Open Microsoft SQL Server Management Studio
![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/eace9bfc-add8-4153-9c49-fa95cc7a024b)

 ### 1) Create Database
``` SQL
CREATE DATABASE Pizza_sales;
```
![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/96c8a885-a05b-4e59-8e72-866052f85798)

   ### 2) Import Data to SQL Server
- Right-click on  Pizza_sales > Tasks > Import Data
- Use import wizard to import Pizza_sales.csv.
- ![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/0af2635a-b60d-4ec6-aa1c-0d358ac06a0f)
  
![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/0157c838-e670-466a-b009-362750b83135)

![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/58cb2583-cdd9-466a-8cfe-ef66c95accd3)

![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/2eabe31f-71e5-4ecc-9fdb-5034aa2174ef)

## 3) DATA CLEANING (we should modify the column)
## 1. change nvarchar(50) to varchar(50)
   
![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/5a58ca6b-a55f-4d53-b474-39b7eb342ff3)

## 2. Pizza ingredients should be changed from nvarchar(50) to varchar(100), because the pizza ingredients length text is more , so change it to varchar(100).


![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/cd07ebd4-e74c-440d-a45e-797874023801)
- - Verify that the import worked:

## Change the pizza_id from small integer(smallint) to integer(int) and order_id from tiny integer(tinyint) to integer(int), 
Because the data is in 48621, then the id will be in thousands of numbers (the id will be of more integers), so it should not be in the small integers(smallint) so change it to integers(int), same should be done in case of the order id - change it to integers(int).
![image](https://github.com/PRATHAMESH9743/PIZZA-SALES-ANALYSIS/assets/154798147/16ceeaa9-dbc6-4168-b9b7-29397143988b)

      
``` SQL
USE Pizza_sales;
```
``` SQL
select * from Pizza_sales;
```


### 3) DATA CLEANING
The termdate was imported as nvarchar(50). This column contains termination dates, hence it needs to be converted to the date format.
   












         
