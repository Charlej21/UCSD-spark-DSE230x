# Big Data Analytics Using Spark

Programming Assignments from UC San Diego - DSE230X
>https://www.edx.org/course/big-data-analytics-using-spark

## Notes

* ## Resilient Distributed Datasets (RDD)
   * Think of RDD as data in a list distributed among executors or different computers.
   * The Spark Context is our gateway to these RDDs from our main program.
   * Map - ```rdd.map(lambda x: x*x) ```
   * Filter - ```rdd.filter(lambda x: x==10) ```
   * Collect - ```print(rdd.collect()) ```
   * Key - Iterator(or a list of values for that key) Pair - ```rdd.groupByKey().mapValues(list)```
