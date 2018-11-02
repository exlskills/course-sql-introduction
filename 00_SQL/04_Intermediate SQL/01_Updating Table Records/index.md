### Changing Table Records and Data Using SQL

#### This section we will learn how to update and delete table records and data using SQL!


#### Updating Records

The update statement is used to update or change records that match a specified criteria. This is accomplished by carefully constructing a where clause.

```SQL
UPDATE "tablename"
SET "columnname" = "newvalue"
WHERE "columnname";
```

Notice how the new function calls are on their own line and the operator calls are indented. The end of the SQL call ends with `;`.

#### Example
Changing an employees information in the company database.

```SQL
UPDATE Customers
SET ContactName = 'Will Smith', City= 'San Francisco'
WHERE CustomerID = 1;
```

#### Deleting Records

The delete statement is used to delete records or rows from the table.

```SQL
DELETE FROM table_name WHERE condition;
```

#### More Examples with W3 Schools
```
DELETE FROM Customers WHERE CustomerName='Will Smith';
```
