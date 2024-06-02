# Home Sales Challenge
---
**Brief Description**: This challenge uses SparkSQL to determine key metrics about home sales data:
> - *Part 1: Create Temporary Views* - A temporary table named `home_sales` is created using Spark for the analysis and is subsequently cached and uncached.
> - *Part 2: Partition the dataset* - The dataset is partitioned using the `date_built` field and the query runtime is compared with that of the cached version.<br>

**Inputs**: The challenge takes in as input a sample dataset from AWS S3 bucket that contains key metrics about home sales data. The corresponding input file is named as *home_sales_revised.csv*. <br>

**Outputs**: The challenge provides the following outputs as described below:
> - *Average Home Price*: The average price of a home for each year it was built, rounded to the nearest two decimal places.     
> - *Average Home Price - Cached vs. Uncached*: Average home price for homes in excess of `$350,000 USD` based on the cached versus uncached versions of the temporary table `home_sales`.
> - *Partitioned Dataset*: The same query above is run against the partiontioned dataset as described above and the runtime is compared against that of the cached version.<br>

**References**:
> - Databricks Documentation: Spark Session, https://api-docs.databricks.com/python/pyspark/latest/pyspark.sql/spark_session.html, accessed May 2024.
> - Handling Data Skew in Apache Spark, https://medium.com/@suffyan.asad1/handling-data-skew-in-apache-spark-techniques-tips-and-tricks-to-improve-performance-e2934b00b021, accessed May 2024. 
---
