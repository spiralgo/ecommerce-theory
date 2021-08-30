https://www.ecommerce-nation.com/color-psychology-for-ecommerce/

General E-commerce System Design:
https://medium.com/double-pointer/system-design-interview-amazon-flipkart-ebay-or-similar-e-commerce-applications-35a0bc764421

## TOOLS
### REDIS
- The main funcion of `Redis`:

For example, a user gets a `Product list` in 20-30 seconds on a real-life project.
It is rather a long duration to wait for a user in each call for the service.
`Redis` comes on the scene at that point to reduce the time getting the Product list, for instance.
Similar to what we have done `memoization/DP problems`, when we get the `Product list` for the first time, `Redis` caches the list.
Whenever a user requests the same data; our system, first checks if the data exists in Redis. 
If data exists, we retrieve data from Redis, otherwise, we call the Product List service to get the data from the database instead. 
(Then we can update Redis with this data retrieved from DB, as well. But a `Cache Worker` seems a more convenient way to keep Redis up-to-date.)

- Redis on Spring:
https://www.youtube.com/watch?v=Yq8Cc7eOgF8&ab_channel=SpringDeveloper

### Hadoop and Spark

- Hadoop stores `BigData` (large datasets ranging in size from gigabytes to petabytes of data) and provides a file-system called `Hadoop Distributed File System (HDFS)` to organize data.
- Spark uses HDFS (as well as the other file systems) to process BigData.

### Spark features/modules:
 
-   [Spark Streaming](https://spark.apache.org/streaming/)  can be used for processing the real-time streaming data. This is based on the micro batch style of computing and processing. 
 
-   [Spark SQL](https://spark.apache.org/sql/)  provides the capability to expose the Spark datasets over JDBC API and allow running the SQL like queries on Spark data using traditional BI and visualization tools
 
-   [MLlib](https://spark.apache.org/mllib/)  is Spark’s scalable machine learning library consisting of common learning algorithms and utilities, including classification, regression, clustering, collaborative filtering, dimensionality reduction, as well as underlying optimization primitives.
 
  -  [GraphX](https://spark.apache.org/graphx/)  is the new (alpha) Spark API for graphs and graph-parallel computation.
