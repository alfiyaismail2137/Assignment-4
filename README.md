 Assignment-4
# DAX and Data Visualization
## Power BI Assignment 2 – DAX & Data Visualization 
### E-Commerce Sales Analysis 
This assignment will help you explore e-commerce sales data analysis using Power BI. 
Below are the files you will be working with (click on each to download): 
<br>
★ List of Orders.csv 
<br>★ Order Details.csv 
<br>★ Sales target.csv 
<br>In this exercise, you will use DAX (Data Analysis Expressions) to analyze and transform 
e-commerce sales data, generating key metrics and insights. You will then create compelling 
visualizations and perform detailed analysis to gain valuable insights into sales trends, 
profitability, and performance metrics within the e-commerce domain. 

Note: Data modeling must be completed prior to data visualization. Ensure that relationships 
are established between the necessary tables, and calculations are performed to derive key 
metrics required for visualization. After creating the charts, make sure to format and 
customize them to enhance visual appeal and comprehension.
Instructions:- 

#### Calculated Columns: 

● Create a Calculated Column for 'Category Type': Add a calculated column in the 
Order Details table that combines the 'Category' and 'Sub-Category' columns into a 
single 'Category Type' column. 

● Calculate Revenue per Order in Order Details Table: Create a calculated column in 
the Order Details table to compute the revenue (Amount * Quantity) per order.

● Create a Calculated Column to Categorize Sales: Add a calculated column named 
‘Sales Category’ in the Order Details table that categorizes each order as 'Above 
Average' or 'Below  Average' based on the Amount value.
Calculated Measures: 

● Calculate Order Count: Define a measure to count the total number of orders in the 
Order Details table. 

● Calculate Average Profit in Delhi: Create a measure to calculate the average profit for 
orders placed in Delhi. 

● Calculate Year-to-Date (YTD) Sales: Define a measure to calculate the total sales 
amount accumulated from the earliest order date up to each order date. 

#### Data Visualization: 

**Sales Target Achievement by Category:** Compare actual sales with sales targets by 
category using a clustered column chart. 

**Max Profit Margin by Sub-Category:** Analyze the maximum profit margin for each 
sub-category of products using a donut chart. 

**Monthly Sales Trend:** Show the trend of monthly sales over time using a line chart. 

**Comparison of Profit and Quantity by Sub-Category:** Compare the relationship between 
profit and quantity sold for different sub-categories using a scatter chart.

**Comparison of Total Sales Amount and Target:** Create cards to succinctly display the total 
sales amount alongside the sales target for quick comparison and analysis. Also, create a 
multi-row card to display the minimum target for each segment. 

**Sales Performance Matrix:** Build a matrix view to analyze how actual sales compare to 
sales targets across different categories and months. 

**Geographic Sales Analysis:** Visualize total sales on a map by city to identify regional sales 
patterns. 

**Sales Distribution by Sub-Category:** Represent the sales distribution across different 
sub-categories using a treemap. 

**Order Count Analysis by State:** Create a funnel chart to visualize the distribution of order 
counts across different states. 
