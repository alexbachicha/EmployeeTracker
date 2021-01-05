# Employee Tracker Application

![GitHub License](https://img.shields.io/badge/made%20by-%40alexbachicha-orange)

## Description 

The Employee Tracker is a command-line application that allows for the management of a company's employees. It is designed with a Content Management System that makes it easier for non-developers to view and iteract with the information stored in the database. At minimum, it allows the user to add departments, roles and employees, view departments, roles and employees, and update employee roles. This application uses Node, Inquirer and MySQL.

## Table of Contents

- [Installation](#Installation)
- [User Story](#UserStory)
- [Usage](#Usage)
- [Licence](#Licence)

## User Story

```
As a business owner
I want to be able to view and manage the departments, roles, and employees in my company
So that I can organize and plan my business
```

## Installation 

To begin, initialize dependencies by running:

```
npm i 
```

The application is invoked with the following line of code:

```
node app.js
```

## Instructions and Demo

The employee database schema contains the following tables:

* **department**:

  * **id** - INT PRIMARY KEY
  * **name** - VARCHAR(30) to hold department name

* **role**:

  * **id** - INT PRIMARY KEY
  * **title** -  VARCHAR(30) to hold role title
  * **salary** -  DECIMAL to hold role salary
  * **department_id** -  INT to hold reference to department role belongs to

* **employee**:

  * **id** - INT PRIMARY KEY
  * **first_name** - VARCHAR(30) to hold employee first name
  * **last_name** - VARCHAR(30) to hold employee last name
  * **role_id** - INT to hold reference to role employee has
  * **manager_id** - INT to hold reference to another employee that manages the employee being Created. This field may be null if the employee has no manager


## License 

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)
