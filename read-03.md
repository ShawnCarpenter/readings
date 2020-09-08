# Computer parts and Pieces

Computers are made of lots of different parts.
THe motherboard holds the processor, ram, and power connectors. (Most motherboards also include network connections, USB ports, integrated video, and disk controllers)
Desktop computers have slots to connect expansion devices, most laptops don't.


# SQL ISERT
INSERT is the command to add data to a SQL database. 

```SQL
INSERT INTO table_name (column_1, column_2, ... columnX)
VALUES (value_1, value_2, ... value_X)
RETURNING return_values;
```

- You must match the order of the values and the column names.
- The `RETURNING` clause is optional
- You can insert multiple rows in the values clause.
- Strings are surrounded by single quotes, if you have a string that contains a single quote character, double the single quote like so:  `'That''s a confusing sentence'`. 

# SQL SELECT

SELECT is used to retrieve data from the database.

```SQL
SELECT
  column_1,
  column_2,
  ...
  column_X
FROM
  table_name;
     
```

- You can use the `*` as a wildcard to select all columns, but it is usually better to request only the data needed to avoid sending too much data over the network.
- You can also use expressions in a select statement `SELECT first_name || ' ' || last_name` to return a full name.


# SQL UPDATE

UPDATE is the statement that changes existing data.

```SQL
UPDATE 
  table_name
SET
  (column_1 = new_value_1, column_2 = new_value_2, ... column_X = new_value_X)
WHERE
  condition;
```

- Name the table you are updating
- Set the new values
- Define what rows should be updated, if the WHERE clause is omitted all rows will be updated

# SQL DELETE

Delete removes rows from the table.

``` SQL
DELETE FROM
  table_name
WHERE
  condition
```

- The `WHERE` clause is optional but if you omit it you delete everything in the table.
- There is a `RETURNING` statement that will return the rows that were deleted.