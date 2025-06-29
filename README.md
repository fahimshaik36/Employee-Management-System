# Employee Management System

This project is a desktop-based application developed using Java Swing for managing employee records. It provides a user-friendly graphical interface for handling employee data such as adding, viewing, updating, and deleting records. The application is connected to a MySQL database using JDBC.

## Features

- Admin login authentication
- Add new employee details through a form
- View all employee records in a table format
- Update employee information based on ID
- Delete employee records from the database
- GUI built using Java Swing for better user interaction

## Technologies Used

- **Language:** Java  
- **GUI Framework:** Java Swing  
- **Database:** MySQL  
- **Connectivity:** JDBC (Java Database Connectivity)  
- **IDE:** NetBeans  
- **Libraries:** DbUtils (for displaying `ResultSet` in `JTable`)  

## Folder Structure

- `Splash.java` – Entry screen with title animation
- `Login.java` – Login form with credential check
- `Home.java` – Main dashboard with navigation
- `AddEmployee.java` – Adds a new employee
- `ViewEmployee.java` – Displays employee data in a table
- `UpdateEmployee.java` – Updates existing records
- `RemoveEmployee.java` – Deletes selected records
- `Conn.java` – Handles database connection

## Setup Instructions

1. Clone this repository to your local system.
2. Create a MySQL database named `employeemanagementsystem`.
3. Use the below SQL script to create the required table.
4. Open the project in NetBeans IDE.
5. Add the MySQL JDBC connector to the project libraries.
6. Run the application starting from `Splash.java`.

## Database Schema

```sql
CREATE TABLE employee (
    name VARCHAR(50),
    fname VARCHAR(50),
    dob VARCHAR(20),
    salary VARCHAR(20),
    address VARCHAR(100),
    phone VARCHAR(15),
    email VARCHAR(50),
    education VARCHAR(30),
    designation VARCHAR(50),
    aadhar VARCHAR(20),
    empId VARCHAR(10) PRIMARY KEY
);
