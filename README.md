# Home_Sales

I used Google Colab, and SparkSQL to determine key metrics about home sales data. Then I created temporary views, partition the data, cached and uncached the temporary tables, and verified that the tables were uncached.


I answered the following questions using SparkSQL:

What is the average price for a four-bedroom house sold for each year? I rounded off the answer to two decimal places.

What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? I rounded off the answer to two decimal places.

What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? I rouded off the answer to two decimal places.

What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

I cached the temporary table `home_sales_data` and checked if the temporary table was cached.

Using the cached data, I ran the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. I determined the runtime and compared it to uncached runtime.

I partition by the "date_built" field on the formatted parquet home sales data and created a temporary table for the parquet data.

I ran the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. I determined the runtime and compared it to uncached runtime.

I uncached the home_sales temporary table and verified that the home_sales temporary table was uncached using PySpark.

