# Payroll Management System

## Getting Started

## Requirements

- Any operating system (i.e. Linux, Windows, MacOS X)
- A little knowledge of React and Node.js . Don't worry if you are new to it, you just need knack to learn.


## Development Setup

- Install node, npm.

## To start FrontEnd React Server
```bash
cd PayrollManagement/payroll-frontend
npm i
npm start
```

## To start Backend Server
```bash
cd PayrollManagement/backend
npm i
nodemon index.js
```

## To [Create User](https://blog.logrocket.com/nodejs-expressjs-postgresql-crud-rest-api-example/#:~:text=have%20superuser%20privileges.-,Creating%20a%20role%20in%20Postgres,-First%2C%20we%E2%80%99ll%20create) in Postgresql

- create a role called **me** and give it a password of **password**. A role can function as a user or a group , so in this case, we’ll be using it as a user.
- We want **me** to be able to create a database.So run the following :-
 ```bash
 ALTER ROLE me CREATEDB ;
 ```
 - After that create a database named api
 ```bash
 CREATE DATABASE api ;
 ```
- For connecting postgres with **me**.Run :
```bash
psql -d postgres -h localhost -U me
```

## To Create Tables

- Run the sql commands mentioned in PayrollManagement/commands/DDL.sql file.
