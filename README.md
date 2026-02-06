# Employee Management System (Java Swing + MySQL)

A simple **Employee Management System** desktop application built using **Java Swing** for GUI and **MySQL** for database connectivity.  
This project allows users to add and search employee details in a structured and user-friendly way.

---

## 🛠️ Technologies Used

- Java (JDK 8+)
- Java Swing (GUI)
- MySQL
- JDBC (Database Connectivity)
- Apache NetBeans IDE

---

## ✨ Features

- Add new employee details
- Search employee by **Employee ID only**
- Store employee data permanently in MySQL database
- Simple and clean Swing-based user interface
- Input validation before inserting data
- **Exit confirmation dialog (Yes / No)** before closing the form
- Proper project structure with separated GUI and database logic

---

## 🗂️ Project Structure

EmployeeManagementSystem/
├── src/
│   └── employeemanagementsystem/
│       ├── EmployeeForm.java           # Main GUI class (MAIN CLASS)
│       ├── InsertEmployee.java         # Database connection & insert logic
│       └── EmployeeManagementSystem.java
│                                      # Empty class (for project structure / future use)
├── database/
│   └── employeedb.sql                 # MySQL database schema & table
├── README.md

---

## ▶️ Main Class

✅ **EmployeeForm.java** is the **ONLY main class** of this project.

```java
public static void main(String[] args) {
    new EmployeeForm().setVisible(true);
}
Other classes DO NOT contain a main() method and are used only for logic and structure.

---

##🗄 Database Details
Database Name: employee_db
Table Name: employee
Table Structure
CREATE TABLE employee (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    designation VARCHAR(100),
    salary INT
);

---

## 🔐 Validation & Confirmation

- Input fields are validated before inserting into database
- On closing the application, a confirmation dialog (**Yes / No**) is shown to avoid accidental exit.

---

##🚀 How to Run the Project

1. Clone or download this repository
2. Open the project in Apache NetBeans IDE
3. Open MySQL Workbench
4. Import the database using employeedb.sql
5. Update database username/password in InsertEmployee.java if required
6. Press F6 (Run Project)

👉 The EmployeeForm GUI will open successfully.


## 👤 Developed By
Abinaya Y


