# Banking Management System using MySQL and Python

## About
__________
In this project, I developed a Virtual Bank named *COLONY BANK OF INDIA* using *Python* and *MySQL. The system allows users to perform various banking operations, with all data being stored in a MySQL database in a structured tabular format. The project focuses on **CRUD (Create, Read, Update, Delete)* operations, ensuring efficient management of customer records. The code is designed to be *100% user-friendly*, with extensive use of exception handling to ensure smooth operation.

This system is specifically designed for bank staff to manage customer records efficiently. Only authorized users can access the program. Once logged in, users can view all customer records, modify them, create new customer accounts, update existing records, delete customer records, and manage loan details. The system also allows users to view transaction histories and generate detailed reports for individual accounts.

The project uses *Python* as the front end for user interaction and *MySQL* as the back end for data storage and management.

---

## Requirements
______________________________ 
To run this project, the following tools and technologies are required:
1. *Python* (Latest Version)
2. *Visual Studio Code* (or any other Python IDE)
3. *MySQL* (for database management)
4. *Python MySQL Connector* (to establish a connection between Python and MySQL)

---

## Modules Used in Python Code
______________________________
The following Python modules were used in the development of this project:
1. *datetime* (to handle date and time operations)
2. *mysql.connector* (to connect Python with MySQL)

---

## About MySQL Code
__________________________
The MySQL database used in this project is named *Hubnet*. The connection details are as follows:
- *Address*: Localhost
- *User*: root
- *Password*: 12345678

### Key Points:
- *UserName* is the *Primary Key* in the Bank table.
- *UserName1* is the *Foreign Key* in the Transaction table, linking it to the Bank table.

---

## SQL Code for Creating Tables

### Table: Bank
This table stores customer details.
sql
CREATE TABLE bank (
    name VARCHAR(30),
    UserName VARCHAR(30) PRIMARY KEY,
    password TINYTEXT,
    Date_of_birth DATE,
    address VARCHAR(40),
    Mobile_Number VARCHAR(30),
    Aadhar_no VARCHAR(30),
    Balance INT
);


### Table: Transaction
This table stores transaction details for each customer.
sql
CREATE TABLE Transaction (
    credited INT,
    debited INT,
    username1 VARCHAR(20),
    FOREIGN KEY (username1) REFERENCES bank(UserName)
);


---

## Features of the Project
______________________________
1. *User Authentication*: Only authorized users can access the system.
2. *Customer Record Management*:
   - Create new customer records.
   - Update existing customer details.
   - Delete customer records.
3. *Transaction Management*:
   - View transaction history for individual accounts.
   - Update loan details for customers.
4. *Exception Handling*: Ensures the program runs smoothly even in case of invalid inputs or errors.
5. *User-Friendly Interface*: The system is designed to be intuitive and easy to use.

---

## How to Run the Code
______________________________
1. Ensure that MySQL is installed and running on your system.
2. Create the bank and Transaction tables using the SQL code provided above.
3. Install the required Python modules (mysql.connector).
4. Run the Bank-Project.py file in your Python IDE (preferably IDLE for better compatibility).

---

## Personal Contribution
______________________________
I designed and developed this project from scratch, focusing on creating a robust and user-friendly banking management system. The project demonstrates my skills in *Python programming, **MySQL database management, and **software development. I also implemented advanced features like **exception handling* and *user authentication* to ensure the system is secure and reliable.

---

## Glimpse of the Project
______________________________
Below are some screenshots of the project in action:
1. *Login Interface*: Authorized users can log in to access the system.
2. *Customer Record Management*: Staff can view, add, update, or delete customer records.
3. *Transaction History*: Detailed transaction records for each customer.
4. *Loan Management*: Update and manage loan details for customers.

---

This project showcases my ability to develop practical, real-world applications using Python and MySQL. It reflects my understanding of database management, user interface design, and software development principles.
