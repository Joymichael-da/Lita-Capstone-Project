# Lita-Capstone-Project
### Goals And Objectives
We had a 3month virtual training session with Incubator Hub as our trainer.This repository is a project given to the student to test our knowledge of what we have learnt in the past months.This project contains a sales data created in an Excel format to analyze the sales performance of a retail store. This project will explore the sales data to uncover key insights such as;
- Top selling Products.
- Regional Performance.
- Monthly Sales Trends.
The goal is to produce an interactive Power BI dashboard that highlights these findings.

### Methodology and Tools Needed
- Microsoft Excel for Data cleaning and Visualization.
- SQL - Structured Query Language for quering of data.
- Power BI for data visualization.
- Github for submission.

### Data Sources
The primary source of data used here is sale data.csv and this ia an open source data provided by our instructors.

### Analysis and Results
#### PROJECT 1
#### On Microsoft Excel
  1) Summary of Total Sales by Product Using Pivot Table

![image](https://github.com/user-attachments/assets/23c0b792-9cc7-469e-8ab1-4c737a8a49ba)

  2) Summary of Total Sales by Region using Pivot Table

![image](https://github.com/user-attachments/assets/d8eb31e0-8726-4c15-a393-a1bbb797dac6)

  3) Summary of Total Sales by Month

![image](https://github.com/user-attachments/assets/c9c4d5eb-92eb-4cb3-a276-39863933d05b)

  4) Average Sales Per Product Using Excel Formula Averageif;
- Shirt  - 326.6667
- Shoes - 308.75
- Hat - 158.75
- Socks - 121.6667
- Jacket - 140
- Gloves - 200

  5) Total Revenue by Region Using Excel Formula Sumif;
- East	- 2450000
- North	- 1950000
- South	- 4675000
- West	- 1512500

#### On SQL
 1) Total Sales for Each Product Category using the query Select Sum(Quantity*UnitPrice) as TotalSales from lita_capstone_project group by Product;
- Shirt - 2367280
- Shoes - 2983085
- Hat - 1533700
- Jacket - 1014420
- Gloves - 1449200

 2) Number of Sales Transaction in Each Region using the query Select count(Quantity) from lita_capstone_project group by Region;
- North - 12078
- South - 12078
- East - 12077
- West - 12077

 3) Highest Selling Product by Total Sales Value using the query
- Shoes - 2983085

4) Monthly Sales Totals for the current year using the query Select month(OrderDate) asd month,sum(Quantity*UnitPrice) as monthly_sales from lita_capstone_project where year(OrderDate)=2023 group by month(OrderDate) order by month;
 - 1 - 241600
 - 2 - 1208000
 - 3 - 253680
 - 4 - 36240
 - 5 - 289920
 - 6 - 483200
 - 7 - 1159680
 - 8 - 144960
 - 9 - 169120
 - 10 - 652320
 - 11 - 507150
 - 12 - 241500

5) The Top 5 Customers by Total Purchase Amount using the query Select CustomerId,Sum(quantity*UnitPrice) as total_purchase_amount from lita_capstone_project group by CustomerId order by total_purchase_amount desc limit 5;
- Cus1375 - 28155
- Cus1023 - 27695
- Cus1353 - 27655
- Cus1171 - 27470
- Cus1367 - 27360

6) Calculate the percentage of Total Sales contribution by each region using the query Select Region,Sum(Quantity*UnitPrice) as total_purchase_amount,(Sum(Quantity*UnitPrice)/(Select Sum(Quantity*UnitPrice) from lita_capstone_project))*100 as percent_total_sales from lita_capstone_Project group by Region order by total_purchase_amount;
- West - 1461150 - 14.2838%
- North - 1883990 - 18.4173%
- East - 2367285 - 23.1419%
- South - 4517020 - 44.1570%

7)  Identify Products with no sales

#### On Power BI    
- Showing the data for Products by Total Sales

![Screenshot (27)](https://github.com/user-attachments/assets/e6435037-b895-4569-a573-c920b1b81c66)

From the data above we can deduce that Shoes was the highest selling product and Socks was the least selling product.

- Showing Total Sales per Region

![Screenshot (29)](https://github.com/user-attachments/assets/b27929b3-0ce4-41c0-a2f0-bc9326c1cb65)

From the data above we can deduce that the top selling product per region is South and the least selling product per region is West.

- Showing Total sales per Month

  ![Screenshot (28)](https://github.com/user-attachments/assets/e46baaa4-9a9b-4f45-aa66-e313510ffdad)

  From the data above we can deduce that the best month of sales is February and the least month of sales is September.

  #### In summary;
  - Top selling product in Descending Order:
  
  Shoes

  Shirt

  Hat

  Gloves

  Jacket

  Socks

  - Regional Performance in Descending Order:
  
  South

  East

  North

  West
 
  - Monthly Sales Trend in Descending Order:
  
  February

  July

  January/June

  August

  October

  March

  May/November

  December

  April

  September

























 


  



