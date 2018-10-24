### How to Insert Into Tables

#### Now let's take a look into how to insert data into a table ourselves!

The insert statement is used to insert or add a row of data into the table.

To insert records into a table, enter the key words insert into followed by the table name, followed by an open parenthesis, followed by a list of column names separated by commas, followed by a closing parenthesis, followed by the keyword values, followed by the list of values enclosed in parenthesis.

 The values that you enter will be held in the rows and they will match up with the column names that you specify. Strings should be enclosed in single quotes, and numbers should not.

```SQL
insert into "tablename"
 (first_column,...last_column)
  values (first_value,...last_value);
```

#### Example:

In the example below, the column name `first` will match up with the value `Will`, and the column name `state` will match up with the value `California`.

```SQL
insert into employee
  (first, last, age, address, city, state)
  values ('Will', 'Smith', 25, '1234 EXL St',
          'Silicon Valley', 'California');
```       

##### Note

All strings should be enclosed between single quotes: `'string'`. 
