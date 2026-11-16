# SQL-Database-Compiler
Java code designed to create and mimic a SQL compiler to accept and execute basic SQL queries. A parser and lexer is generated using Java CUP and JFlex respectively to accept input instructions from the user. The server handles all the execution and the client has a simple UI that allows the user to interact with the server.

The server must be running before the client - the client depends on the connection to the server.

The server creates a database by creating a folder in your "C://Users/" folder. All data tables and data are stored within that table.

The server accepts queries in the format:
CREATE <var>;                                                       -> create a database
USE <var>;                                                          -> use a database
CREATE TABLE <var> ( <var> int, <var> String, <var> String );       -> create a table
CREATE index on <var> (<var>);                                      -> create an index
SELECT <var/s> from <var>;                                          -> select
INSERT into <var> values (<val>, <val>, <val>);                     -> insert
DELETE from <var> where <condition>;                                -> delete
UPDATE <var> set <var> = <val> where <condition>;                   -> update
