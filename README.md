# Home_Sales

In pursuit of significant metrics for home sales data, Google Colab and SparkSQL were employed to extract essential insights. The process entailed creating temporary views, partitioning the data, and caching and uncaching the temporary tables. Furthermore, the verification of uncached tables was carried out to ensure the optimal application of resources.

I answered the following questions using SparkSQL:

What is the average price for a four-bedroom house sold for each year? I rounded off the answer to two decimal places.

![prices](https://github.com/Amarilli/Home_Sales/blob/main/Images/prices.png)

What is the average home price for each year a home with three bedrooms and three bathrooms was built? I rounded off the answer to two decimal places.

What is the average price of a home for each year? The home was built with three bedrooms, three bathrooms, and two floors and is greater than or equal to 2,000 square feet. I rounded off the answer to two decimal places.

What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Could you determine the run time for this query, and then turn your answer to two decimal places?

I cached the temporary table `home_sales_data` and checked if the temporary table was cached.

Using the cached data, I ran the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. I determined the runtime and compared it to the uncached runtime.

![difference](https://github.com/Amarilli/Home_Sales/blob/main/Images/difference.png)

I partitioned the formatted parquet home sales data by the "date_built" field and created a temporary table for the parquet data.

I ran the last query, which calculates the average price of a home per "view" rating with an average home price greater than or equal to $350,000. I determined the runtime and compared it to the uncached runtime.

![parquet](https://github.com/Amarilli/Home_Sales/blob/main/Images/parquet.png)

I uncached the home_sales temporary table and verified that the home_sales temporary table was uncached using PySpark.

See the remaining answers and process here: [Colab](https://github.com/Amarilli/Home_Sales/blob/main/Home_Sales_colab%20.ipynb)

