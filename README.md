# SQL-411

## Index

## Starting PSQL:
* Open termianl window
* Type `psql`*`nameOfDatabase`*

## How to create a database:
* run `createdb`*`databaseName`*

## How to list tables in a database:
* From inside psql, run `\l`

## How to connect to a database in psql:
* From inside psql, run `\c`*`databaseName`*

## How to get a description of list tables in a database:
* From inside psql, run `\dt`

## How to get columns from a table:
* From inside psql, run `\d` *`tableName;`*

## How to create a table:
* From inside of psql, run `CREATE TABLE`*`databaseName`*`(key value, key value, key value);`

## CRUD commands:

### For querying a table:
`SELECT * from` *`table;`* -> gets all the things from the table.

`SELECT * from` *`table`*` WHERE` *`keyValue`*` =` *`searchValue;`* -> gets specifically what you search for.

`SELECT` *`keyValue`* `,` *`additionalKeyValue`*`,`*` asManyAsYouWantKeyValues`* `from` *`table`* `WHERE` *`keySearchValue`* `>\<\=/any/` *`searchCriteria`*`;` -> You can narrow your search through setting any number of keys to match the specific criteria.

### Adding to the database in PSQL:
`INSERT into` *`table`* `VALUES ('values','you', 'want', 'to', 'add','as','long', 'as', 'these','values','sync','up','with','the','key','order');`-> assigns these values to keys already set up in the table.

`INSERT into` *`table`*

### Updating information in PSQL:

`UPDATE `*`table`*` set `*`value`*` =` *`'yourValue'`* ` WHERE `*`key`*` = `*`searchCriteria;`* -> lets you update specific key values based on your search criteria.

### Deleting data from PSQL:


### How to add a column to an existing table:
* From inside of psql, run `ALTER TABLE` *`tableName`* `ADD COLUMN` *`ColumnName;`*

### How to get a total number of entries in a table:
* From inside of psql, run `SELECT COUNT(*) FROM`*`tableName;`*

### How to sum the values in a single column:
From inside of psql, run `SELECT SUM(key) FROM` *`table;`*

### How to average the values in a single column:
From inside of psql, run `SELECT AVG(key) FROM` *`table;`*

### Exporting your database into a sql file:
`pg_dump` *`nameOfDatabase`* `>` *`file.sql`*

### Importing your sql file to a database:
`psql`*`dataBase`*`<`*`file.sql`*
