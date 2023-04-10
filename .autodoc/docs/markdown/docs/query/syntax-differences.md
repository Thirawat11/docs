[View code on GitHub](https://dune.com/docs/query/syntax-differences.md)

The app technical guide provides a comprehensive guide for migrating queries from Postgres to Dune SQL and from SparkSQL to DuneSQL. The guide covers the syntax and operator differences between Postgres, Spark, and Dune SQL. It provides a detailed comparison of the syntax and keyword operator differences between the three databases. The guide explains the differences in syntax for various operations such as math or numeric operations, array-based indexing, implicit type conversions, addresses, selecting keyword columns, alias naming, exponentiation notation, interval argument, generate_series, handling decimals for prices.usd, defining NULL array, encoding strings to hex, get JSON object differences, group by an alias, explicit date/time casting, checking if an item exists in an array, explode, median, using “is True/False,” string data type, casting as strings, aggregate functions, user-generated views, and event logs topic indexing.

The guide provides examples for each of the syntax differences and explains how to use them in Dune SQL. It also highlights the differences in syntax between Dune SQL and other databases, such as Postgres and Spark SQL. The guide recommends avoiding the use of double quotes in Dune SQL, as the parser sometimes treats words in double quotes as a string and sometimes as an object like a column name.

Overall, the app technical guide provides a comprehensive guide for migrating queries from Postgres and Spark SQL to Dune SQL. It is a valuable resource for developers who are new to Dune SQL and need to migrate their queries from other databases.
## Questions: 
 1. What are the differences in handling decimals for prices.usd in Dune SQL compared to Postgres and Spark SQL?
- In Dune SQL, decimals for prices.usd are replaced by tokens_[blockchain].erc20.decimals.

2. How does Dune SQL handle implicit type conversions between character and numeric types compared to Postgres and Spark SQL?
- Dune SQL does not have implicit type conversions between character and numeric types, unlike Postgres and Spark SQL.

3. What is the recommended approach for using double quotes in Dune SQL?
- Double quotes are not recommended in Dune SQL, as the parser sometimes treats words in double quotes as a string and sometimes as an object like a column name.