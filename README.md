This SQL program creates and manages a customer SIM information table. The database used is aids. The table stores details such as the customer's mobile number, network provider, name, Aadhaar number, port number, and SIM status.

Table Description
The table user1 contains the following fields:

mobile_no – Stores the customer's mobile number. It is declared UNIQUE, so duplicate mobile numbers are not allowed.

network – Stores the customer's network provider, such as Jio, Airtel, BSNL, or Idea.

customer_name – Stores the name of the customer.

aadhar_no – Stores the customer's Aadhaar number. It is also declared UNIQUE.

port – Stores the port number associated with the customer.

sim_status – Stores whether the SIM is active or inactive.

Purpose of the Queries
The program performs different operations to retrieve customer information:

Display all customer details

SELECT * FROM user1;

Displays all columns and all records.

Search customer using Aadhaar number

SELECT customer_name FROM user1
WHERE aadhar_no = 123456789123;

Displays the name of the customer having the specified Aadhaar number.

Display active SIM customers

SELECT customer_name FROM user1
WHERE sim_status = 'active';

Displays customers whose SIM is currently active.

Display inactive SIM customers

SELECT customer_name FROM user1
WHERE sim_status = 'inactive';

Displays customers whose SIM is inactive.

Find customers using port number

SELECT customer_name FROM user1
WHERE port = 2;

Displays customers whose port number is 2.

Short Description for Record/Assignment
Description: This SQL program creates a customer SIM database and stores information about mobile numbers, network providers, customer names, Aadhaar numbers, port numbers, and SIM status. It demonstrates the use of CREATE TABLE, INSERT, and SELECT statements along with the WHERE clause and UNIQUE constraint to manage and retrieve customer information.


