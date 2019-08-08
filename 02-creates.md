# SQL Creates

## Database

The first way to get started is to create a database. The syntax is fairly straight forward.

Easiest way: `CREATE DATABASE your_database_name;`

There are additional options you can add if you want to specify the owner of the database, encoding rules, or limit connections. These are listed https://www.postgresql.org/docs/9.0/sql-createdatabase.html

## Schema

If you need to create a schema, it's very similar.

`CREATE SCHEMA your_schema_name;`

There are additional options for this as well. These are listed https://www.postgresql.org/docs/9.0/sql-createdatabase.html

## Table
Creating a table takes a bit more effort. Here we need to define all of the column types for the table.

```
CREATE TABLE films (
    code        char(5),
    title       varchar(40),
    did         integer,
    date_prod   date,
    kind        varchar(10),
    len         interval hour to minute
);
```

You can also set contraints and indexes in this create as well. We'll cover these more at a later point. More info at https://www.postgresql.org/docs/9.0/sql-createtable.html (there's a lot).

