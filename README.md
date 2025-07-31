# 🎓 Student Management System (Java + MySQL)

A desktop-based Student Management System built using **Java Swing**, **JDBC**, and **MySQL**, developed in **NetBeans IDE**.

This application allows the user to **manage student data** with a simple GUI interface — including features like adding, updating, deleting, and searching for student records in a connected MySQL database.

---

## 🔐 Login Details

> ⚠️ The login system uses a **predefined username and password** (hardcoded in the code):

- **Username**: `admin`  
- **Password**: `1234`

_(Change these values inside the source code if you want to update credentials)_

---

## ✅ Features

- 📋 Add new student records
- 📝 Update existing records
- ❌ Delete records by roll number
- 🔍 Search for students
- 🔐 Login authentication (predefined user/pass)
- 🖼️ Simple and clean Java Swing GUI

---

## 🛠️ Tech Stack

| Tool       | Purpose                         |
|------------|----------------------------------|
| Java       | Application logic (Swing GUI)    |
| NetBeans   | IDE used for development         |
| MySQL      | Backend relational database      |
| JDBC       | Database connectivity in Java    |

---

## 🧰 How to Run This Project

1. **Clone or download** this repository to your local machine.
2. Open the project in **NetBeans IDE**.
3. Make sure MySQL server is running and the `college` database exists.
4. Create the required `student` table:

```sql
CREATE DATABASE IF NOT EXISTS college;
USE college;

CREATE TABLE IF NOT EXISTS student (
    Rollno INT PRIMARY KEY,
    StudentName VARCHAR(255),
    Class VARCHAR(100)
);
