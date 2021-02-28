# Node.js, Express.js, and PostgreSQL: CRUD REST API example

RESTful API + CRUD API + PostgreSQL

To start you have to set up a PostgreSQL database with the following options

**postgres=#** CREATE ROLE me WITH LOGIN PASSWORD 'password';

**postgres=#** ALTER ROLE me CREATEDB;

**postgres=#** \q

**psql** -d postgres -U me

**postgres=>** CREATE DATABASE api;

**postgres=>** \c api

You are now connected to database "api" as user "me".

**api=>** CREATE TABLE users (

ID SERIAL PRIMARY KEY,

name VARCHAR(30),

email VARCHAR(30)

);

_Then insert table_

INSERT INTO users (name, email)

VALUES ('Jerry', 'jerry@example.com'), ('George', 'george@example.com');

md### Fixed

The table should look like this

**api=>** SELECT \* FROM users;

id | name | email

----+--------+--------------------

1 | Jerry | jerry@example.com

2 | George | george@example.com

Then get this project into your pc and NPM INSTALL

Enjoy your day
