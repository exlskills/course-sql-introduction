### Let's see how we can begin to select data from tables through code!

The `select` statement is used to query the database and retrieve data that matches what you're looking for and specify within your code!

The format can be shown below: 

~~~~sql
 SELECT "column1"
  [,"column2" ,etc]
  FROM "tablename"
  [WHERE "condition"];
~~~

You can select as many column as you would like, or you can use a `*` to select all columns.

Conditional selections used in the `where` clause are:  

* `= equal`
* `> greater`
* `< less than`
* `>= Greater than or equal`
* `<= Less than or equal`
* `<> Not equal to`


The `LIKE` pattern matching operator can also be used in the conditional selection of the where clause. Like is a very powerful operator that allows you to select only rows that are similar to what you specify.

The percent sign `%` can be used as a wild card variable to match any possible character that might appear before or after the characters specified. For example:

```SQL
SELECT first, last, city
   FROM empinfo
   WHERE first LIKE 'Wi%';
```

This will match and select any matches of names that start with `Wi`

But remember... Strings must be in single quotes!

### Specifying Exact Data Queries

We can also specify exact data we are looking to select,

```SQL
SELECT first, last
   FROM empinfo
   WHERE last LIKE %o;
```

This statement will match any last names that end in an `o`.

or.. use the `*` to select all records of a function. For example:

```SQL
SELECT * FROM empinfo
   WHERE first = Will;
```

This will pull all names that start with `Will` from the database that you have selected from.

Easy enough? Perfect, Let's move on!
