### Changing Table Records and Data Using SQL

#### This section we will learn how to update and delete table records and data using SQL!


#### Updating Records

The update statement is used to update or change records that match a specified criteria. This is accomplished by carefully constructing a where clause.

```SQL
update "tablename"
set "columnname" = "newvalue"
 [,"nextcolumn" = "newvalue2"...]
where "columnname"
  OPERATOR "value" [and|or "column" OPERATOR "value"];
```

Notice how the new function calls are on their own line and the operator calls are indented. The end of the SQL call ends with `;`.

#### Example
Changing an employees information in the company database.

```SQL
update employee
  set age = age+1
  where first_name='Will' and last_name='Smith';
```

#### Deleting Records

The delete statement is used to delete records or rows from the table.

```SQL
delete from "tablename" where "columnname"
  OPERATOR "value" [and|or "column"
  OPERATOR "value"];
```

#### More Examples

```SQL
delete from employee;
```
Note: if you leave off the where clause, all records will be deleted!

```SQL
delete from employee
  where lastname = Will;
```  

```SQL
delete from employee
  where firstname = Will or firstname = Tom;
```

Here are a few SQL queries for you to practice on your own!
