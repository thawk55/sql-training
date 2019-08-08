# SQL - Structured Query Language

SQL is a language used for to handle data stored in a relational database. It allows you to create, edit, remove, and look up data in a structured way. There are many databases that use SQL. Some of them are MySQL, Oracle, Microsoft SQLServer, SQLite3, Postgres. We will focus on Postgres for these lessons but many of the principles remain the same across databases.

Databases are organized by database, schema, and table.

A database has multiple schemas. A schema has multiple tables.

A table is defined by columns and each row is a data entry.
Databases, schemas, tables, and columns are written as snake case. Example: user_first_name

In Postgres the default schema is called `public` and works for most use cases.

Example:

database = `my_first_database`
schema = `public`
table = `users` with columns `first_name`, `last_name`, and `role`.

You can query it directly by either `my_first_database.public.users.first_name` or `my_first_database.users.first_name` as `public` is the default schema.

If you are already in the context of the database `users.first_name` would also work.

The majority of keywords should be written in UPPER_SNAKE_CASE and all statements will end with a `;`.

