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

<br>Table tools-->New Column-->Category Type = 'Order Details'[Category]&"-"&'Order Details'[Sub-Category].

● Calculate Revenue per Order in Order Details Table: Create a calculated column in 
the Order Details table to compute the revenue (Amount * Quantity) per order.

<br>Table tools-->New Column-->Revenue = 'Order Details'[Amount]*'Order Details'[Quantity].

● Create a Calculated Column to Categorize Sales: Add a calculated column named 
‘Sales Category’ in the Order Details table that categorizes each order as 'Above 
Average' or 'Below  Average' based on the Amount value.

<br>Table tools-->New Column-->Sales category = IF('Order Details'[Amount]>=[Average amount],"Above Average","Below Average").

#### Calculated Measures: 

● Calculate Order Count: Define a measure to count the total number of orders in the 
Order Details table. 

<br>Table tools-->New Measures-->Count = COUNT('Order Details'[Order ID]).

● Calculate Average Profit in Delhi: Create a measure to calculate the average profit for 
orders placed in Delhi. 

<br>Table tools-->New Measures-->Average Profit = AVERAGE('Order Details'[Profit]).
<br>Table tools-->New Measures-->Average_profit = CALCULATE([Average Profit],'List of Orders'[City]="Delhi").

● Calculate Year-to-Date (YTD) Sales: Define a measure to calculate the total sales 
amount accumulated from the earliest order date up to each order date. 

<br>Table tools-->New Measures-->Total_Amount = SUM('Order Details'[Amount]).
<br>Table tools-->New Measures-->Ytd = TOTALYTD([Total_Amount],'List of Orders'[Order Date]).

#### Data Visualization: 

**Sales Target Achievement by Category:** Compare actual sales with sales targets by 
category using a clustered column chart. 
  <br>Drag and drop clustered column chart on canvas. Input X-axis, Y -axis, Legend as Target, Amount and Category.

**Max Profit Margin by Sub-Category:** Analyze the maximum profit margin for each 
sub-category of products using a donut chart. 
  <br>Drag and drop Donut chart on canvas. Input Legend and Values as Sub-category and Max of profit.

**Monthly Sales Trend:** Show the trend of monthly sales over time using a line chart.
  <br>Drag and drop line chart on canvas. Input X-axis, Y -axis, Legend as Month, Total Amount and Category.

**Comparison of Profit and Quantity by Sub-Category:** Compare the relationship between 
profit and quantity sold for different sub-categories using a scatter chart.
  <br>Drag and drop scatter chart on canvas. Apply field values.

**Comparison of Total Sales Amount and Target:** Create cards to succinctly display the total 
sales amount alongside the sales target for quick comparison and analysis. Also, create a 
multi-row card to display the minimum target for each segment. 
  <br>Drag and drop card on canvas. input value and category.

**Sales Performance Matrix:** Build a matrix view to analyze how actual sales compare to 
sales targets across different categories and months. 
  <br>Drag and drop matrix on canvas. Input rows,columns, values.

**Geographic Sales Analysis:** Visualize total sales on a map by city to identify regional sales 
patterns. 
  <br>Drag and drop map on canvas. Apply field values.

**Sales Distribution by Sub-Category:** Represent the sales distribution across different 
sub-categories using a treemap. 
  <br>Drag and drop treemap on canvas. Apply field values.
  
**Order Count Analysis by State:** Create a funnel chart to visualize the distribution of order 
counts across different states. 
<br>Drag and drop funnel chart on canvas. Input category category, values field as state , count of order ID.

