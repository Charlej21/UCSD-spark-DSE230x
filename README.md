# Big Data Analytics Using Spark

Programming Assignments from UC San Diego - DSE230X
>https://www.edx.org/course/big-data-analytics-using-spark

## Notes

* ## Resilient Distributed Datasets (RDD)
   * Think of RDD as data in a list distributed among executors or different computers.
   * The Spark Context / Head Node is our gateway to these RDDs from our main program.
   
   * Map - Applies operation to each element of RDD in parallel.
   * ```rdd.map(lambda x: x*x) ```
   
   * Reduce - Uses reduce operators on all executors to give one final output.
   * Reduce operator takes two inputs, gives one output.
   * ```rdd.reduce(lambda x,y:x+y)```
   
   * Filter - Selectively chooses some elements out of total.
   *  ```rdd.filter(lambda x: x==10) ```
   
   * Parallelize - Turns a list to an RDD.
   * Collect - ```print(rdd.collect()) ```
   
   * Key - Iterator(or a list of values for that key) Pair - ```rdd.groupByKey().mapValues(list)```
   
   * Lazy Evaluation - Instead of mapping all data, then reducing all of it (which goes through data twice)
   * Map first value, reduce it , map second value, reduce it and update the result, ...
   * When same RDD is needed for different computations use .cache() after .map()
   
   
   
