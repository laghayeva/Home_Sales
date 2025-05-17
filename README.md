# Home_Sales


---

## Key Tasks

1. Read the CSV file from AWS S3 into a PySpark DataFrame.
2. Create a temporary view and run SparkSQL queries to:
   - Calculate average home prices by bedroom count and year
   - Filter by square footage, floor count, and view rating
   - Round all results to two decimal places
3. Measure query runtime with and without caching
4. Write data to a parquet file partitioned by `date_built`
5. Read parquet data and compare query performance
6. Cache and uncache temporary tables

---

## Results Summary

- **Caching** significantly reduced the runtime of SQL queries on repeat execution.
- **Partitioning by `date_built`** improved read efficiency on filtered queries.
- The average price of homes with high view ratings often exceeded $350,000.


