
# Intermediate Assessment 

## Part -1 Data Cleaning and Loading 
Remove duplicate rows

Standardize OrderDate

Handle missing values - null and Replace With to Unknown

Columns UnitPrice, Sales, Cost, Profit are replaced by new colunms with the given eqautions

UnitPrice = Sales ÷ Quantity

Sales = Quantity × UnitPrice

Cost = Sales − Profit

Profit = Sales − Cost

## Part - 2 Visualizations and Insights 

### Pie chart: orders by region

Drag Region into Legend.

Drag OrderID into Values.

### Column chart: top 5 products by number of orders

Drag Product into X-axis.

Drag OrderID into Y-axis

Filter type: Top N
Show items: Top, 5
By value: drag OrderID

### Line chart: profit trend over time

Drag OrderDate into X-axis

Drag TotalProfit into Y-axis.

## Part -3 DAX Calculations 

EastRegionOrders = FILTER ( SalesData, SalesData[Region] = "East" )

ProfitCostDifference = SalesData[Profit] - SalesData[Cost]

TotalProfit = SUM ( SalesData[Profit_New] )
