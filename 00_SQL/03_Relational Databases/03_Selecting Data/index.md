### Let's see how we can begin to select data from tables through code!

The `select` statement is used to query the database and retrieve data that matches what you're looking for and specify within your code!

The format can be shown below:

Enter this query into this [link](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all) from W3 Schools and see the result!

```sql
 SELECT * FROM "Customers";
```

You can select as many columns as you would like, or you can use a `*` to select all columns!

As you can see the resulting query shows the number of records is equal to 91 and shows all of the records of customers in the database.

### The WHERE Clause

Conditional selections used in the `where` clause are:  

* `= equal`
* `> greater`
* `< less than`
* `>= Greater than or equal`
* `<= Less than or equal`
* `<> Not equal to`

In the web3 Schools try copying the following query and see the result.

```SQL
SELECT * FROM Customers
WHERE CustomerID = 1;
```  
Try playing witht he `WHERE` clause and see the different results you get!!

### The LIKE Conditional Selection

The `LIKE` pattern matching operator can also be used in the conditional selection of the where clause. Like is a very powerful operator that allows you to select only rows that are similar to what you specify.

The percent sign `%` can be used as a wild card variable to match any possible character that might appear before or after the characters specified. For example:

```SQL
SELECT * FROM [Customers]
WHERE CustomerName LIKE 'A%';
```

This will match and select any matches of customer names that start with `A`

But remember... Strings must be in single quotes!

### Specifying Exact Data Queries

We can also specify exact data we are looking to select.

The `*` to select all records of a function. For example:


Easy enough? Perfect, Let's move on!
