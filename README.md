# Big Data Analytics Using Spark

Programming Assignments and Examples from UC San Diego - DSE230X
>https://www.edx.org/course/big-data-analytics-using-spark

## Notes

* ## Resilient Distributed Datasets (RDD)
   * Think of RDD as data in a list distributed among executors or different computers.
   * It is a distributed immutable array.
   * The Spark Context / Head Node is our gateway to these RDDs from our main program.
   ---
   * Map - Applies operation to each element of RDD in parallel.
   ---
   * Reduce - Uses reduce operators on all executors to give one final output.
   * Reduce operator takes two inputs, gives one output.
   ---
   * Filter - Selectively chooses some elements out of total.
   ---
   * Parallelize - Turns a list to an RDD.
   * Collect - Inverse operation that materializes RDD.
   ---
   * Lazy Evaluation - Instead of mapping all data, then reducing all of it (which goes through data twice)
   * Map first value, reduce it , map second value, reduce it and update the result, ...
   * When same RDD is needed for different computations use .cache() after .map()
   * This is in contrast to lazy eval. Spark usually doesn't cache but uses pipelined eval (lazy).
   ---
   * Partitioning used to dedicate workers to parts of RDD.
   * glom() can be used to investigate each partition.
   ---
   
* ## Spark SQL
   * Dataframes are more restricted than RDDs.
   * It is essentially an RDD of rows , plus additional information of schema.
   ---
   * Dataframe can be created from an RDD that is a list of rows.
   * If schema is explicitly passed it can be created from tuples. (Usual content of RDD)
   ---
   * Parquet is an underlying data structure on disk from which we can load dataframes.
   * Spark SQL can query a database without going through all of it.
   ---

   
   
   
