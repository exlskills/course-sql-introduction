### Changing Table Records and Data Using SQL
#### This section we will learn how to update and delete table records and data using SQL!


#### Updating Records
The update statement is used to update or change records that match a specified criteria. This is accomplished by carefully constructing a where clause.

update "tablename"
set "columnname" = "newvalue"
 [,"nextcolumn" = "newvalue2"...]
where "columnname"
  OPERATOR "value" [and|or "column" OPERATOR "value"];

 [] = optional

Notice how new function calls are on their own line and the operator calls are indented. The end of the SQL call ends with `;`.

Example: Changing an employees information in the company database.
```
update employee
  set age = age+1
  where first_name='Will' and last_name='Smith';
  ```

#### Deleting Records

The delete statement is used to delete records or rows from the table.

```
delete from "tablename" where "columnname"
  OPERATOR "value" [and|or "column"
  OPERATOR "value"];
```
[ ] = optional


Examples:
```
delete from employee;
```
Note: if you leave off the where clause, all records will be deleted!
```
delete from employee
  where lastname = 'Will';
```  
```
delete from employee
  where firstname = 'Will' or firstname = 'Tom';
```

Here are a few SQL queryies for you to practice on your own!

[ToDO]
