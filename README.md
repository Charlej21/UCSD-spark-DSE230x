# Big Data Analytics Using Spark

Programming Assignments from UC San Diego - DSE230X
>https://www.edx.org/course/big-data-analytics-using-spark

## Useful Code Snippets

* ## Resilient Distributed Datasets (RDD)
   * Map - ```rdd.map(lambda x: x*x) ```
   * Filter - ```rdd.filter(lambda x: x==10) ```
   * Collect - ```print(rdd.collect()) ```
   * Key - Iterator(or a list of values for that key) Pair - ```rdd.groupByKey().mapValues(list)```
