# Superstore-data-analysis

# Data Cleaning and Manipulation for Visualization

# Overview of Dataset
The dataset consists of 9,994 rows and 21 columns. It contains information related to orders from a superstore, including details such as order date, ship date, customer information, product details, and sales metrics.

# Data Cleaning Steps
Handling Null Values Fortunately, there are no null values in the dataset as indicated by the column summary (Non-Null Count is 9994 for all columns). However, if there were null values, the following actions would be considered:

# Remove rows with missing values in critical fields (e.g., Sales, Profit).
Impute missing values for non-critical fields (e.g., City, Postal Code) based on the available data.

# Standardization
Date Fields
Ensure that Order Date and Ship Date fields are in the correct datetime format (which they already are).
Text Fields
Convert all string values (e.g., Customer Name, Product Name, Category) to lowercase or uppercase for consistency.
Strip any leading or trailing spaces to avoid errors during grouping or filtering.
Removing Duplicates: Check for duplicate entries, especially across columns like Order ID, Customer ID, or Product ID. For instance, if the same order is entered multiple times, duplicates should be removed.

Outliers Detection: Check for any outliers in numerical columns like Sales, Quantity, and Profit. Extreme values could distort the analysis and might need to be reviewed or removed if they are invalid.

# Consistency in Categorical Data
Ensure that categorical values (e.g., Ship Mode, Segment, Region) are consistent. For instance, Second Class and second class should be standardized to a single format.

# Data Manipulation
Creating New Calculated Fields For a more robust analysis, new calculated columns could be added:
Profit Margin A calculated column to determine profit margin could be created: Profit Margin = Profit / Sales
Order Processing Time Calculate the difference between Order Date and Ship Date to get the processing time: Processing Time = Ship Date - Order Date
Filtering and Grouping
Group the data by Category, Sub-Category, Region, or Segment for summary statistics such as total sales, average profit, and total orders.
Filter the data for specific regions or categories if only a subset of the dataset is needed for analysis.

# Tableau Analysis

# Sales and Profit Overview
Sales and Profit by Region: One of the charts likely compares total sales and profit by region (e.g., South, West). This analysis highlights which regions are performing well in terms of revenue and profitability.

# Category-wise Sales 
Another part of the dashboard might show sales distribution across different product categories (e.g., Furniture, Office Supplies, Technology). It helps to identify the top-selling categories and their contribution to total revenue.

Profitability and Discounts: The dashboard may also showcase how profit correlates with discounts. High discounts might lead to lower profits, which can be visualized through scatter plots or bar charts.

# Top Products and Customers
Top-Selling Products: A table or chart showing the products with the highest sales can offer insights into customer preferences.

# Customer Segmentation 
The analysis might categorize customers based on their segment (e.g., Corporate, Home Office) and show how much each segment contributes to sales and profit.

# Geographical Analysis
State/City-Level Analysis: The dashboard could include a map visualizing sales and profit data at the state or city level. This is useful for understanding geographical trends and targeting high-performing locations.

# Overview
The dataset contains 9,994 rows and 21 columns focused on superstore orders. The data cleaning involved handling null values, standardizing text and date fields, removing duplicates, and ensuring consistency in categorical data. Data manipulation included creating calculated fields like profit margin and order processing time, and grouping data by categories like region, segment, and product for summary insights.

The Tableau dashboard visualizes key metrics like sales, profit, and order trends across regions, categories, and customer segments, helping to identify top products, profitable regions, and overall performance trend

[[Here](https://public.tableau.com/app/profile/babajide.onanibosi/viz/superstore_16571232715590/Dashboard1?publish=yes)]
