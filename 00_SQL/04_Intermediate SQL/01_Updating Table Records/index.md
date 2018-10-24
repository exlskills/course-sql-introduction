### Changing Table Records and Data Using SQL

#### This section we will learn how to update and delete table records and data using SQL!


#### Updating Records

The update statement is used to update or change records that match a specified criteria. This is accomplished by carefully constructing a where clause.

```SQL
UPDATE "tablename"
SET "columnname" = "newvalue"
 [,"nextcolumn" = "newvalue2"...]
WHERE "columnname"
  OPERATOR "value" [AND|OR "column" OPERATOR "value"];
```

Notice how the new function calls are on their own line and the operator calls are indented. The end of the SQL call ends with `;`.

#### Example
Changing an employees information in the company database.

```SQL
UPDATE employee
  SET age = age+1
  WHERE first_name='Will' AND last_name='Smith';
```

#### Deleting Records

The delete statement is used to delete records or rows from the table.

```SQL
DELETE FROM "tablename" WHERE "columnname"
  OPERATOR "value" [AND|OR "column"
  OPERATOR "value"];
```

#### More Examples

```SQL
DELETE FROM employee;
```
Note: if you leave off the where clause, all records will be deleted!

```SQL
DELETE FROM employee
  WHERE lastname = Will;
```  

```SQL
DELETE FROM employee
  WHERE firstname = Will OR firstname = Tom;
```

Here are a few SQL queries for you to practice on your own!
