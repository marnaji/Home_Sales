# Home_Sales_challenge
In this task, your objective is to leverage your knowledge of SparkSQL to extract key metrics from home sales data. You will utilize Spark to create temporary views, partition data, cache and uncache a temporary table, and confirm that the table has been successfully uncached.

## Instructions:

1. Begin by renaming the *Home_Sales_starter_code.ipynb* file as *Home_Sales.ipynb.*
2. Import the necessary PySpark SQL functions for this assignment.
3. Read the *home_sales_revised.csv* data from the starter code into a Spark DataFrame.
4. Create a temporary table named *home_sales*.
5. Use SparkSQL to answer the following questions:

    * Calculate the average price for a four-bedroom house sold each year, rounding your answer to two decimal places.
    * Determine the average price of homes for each year they were built, provided they have three bedrooms and three bathrooms. Round off your answer to two decimal places.
    * Find the average price of homes for each year with three bedrooms, three bathrooms, two floors, and a size greater than or equal to 2,000 square feet. Round your answer to two decimal places.
    * Calculate the "view" rating for homes costing $350,000 or more. Determine the query runtime and round it to two decimal places.

6. Cache your temporary table *home_sales*.
7. Verify if your temporary table is cached.
8. Utilizing the cached data, execute a query that filters view ratings with an average price greater than or equal to $350,000. Determine the runtime and compare it to the uncached runtime.
9. Partition the formatted parquet home sales data by the "date_built" field.
10. Create a temporary table for the parquet data.
11. Run a query to filter out view ratings with an average price of $350,000 or more. Determine the runtime and compare it to the uncached runtime.
12. Uncache the *home_sales* temporary table.
13. Verify that the **home_sales temporary** table is indeed uncached using PySpark.
14. Download your **Home_Sales.ipynb** file and upload it into your **Home_Sales** GitHub repository.