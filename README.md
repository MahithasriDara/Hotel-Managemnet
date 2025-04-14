# Hotel-Managemnet
Hotel management using mysql &amp; c++
# 🏨 Hostel Management System — C++ with MySQL

A simple console-based Hostel Management System written in C++ that uses MySQL for database operations. This program allows you to insert hostel records, reserve beds for students, and manage bed availability directly from the terminal.

---

## 💡 Features

- Connects to a MySQL database.
- Inserts new hostel records.
- Reserves beds for students.
- Updates bed availability in real-time.
- Displays confirmation and fee instructions.
- Simple and clean console-based UI.

---

## 💃️ Database Setup

Before running the program, set up your MySQL database as follows:

```sql
CREATE DATABASE mydb;

USE mydb;

CREATE TABLE hostel (
    Name VARCHAR(50),
    Bed INT,
    Fee INT
);
```

---

## ⚙️ How to Run

1. Install **MySQL Server** and create the `mydb` database using the SQL commands above.
2. Install **MySQL Connector/C++**.
3. Update your C++ code with your MySQL password:

```cpp
const char* PW = "Your Password";  // Replace with your actual MySQL password
```

4. Compile the code using g++:

```bash
g++ hostel_management.cpp -o hostel_management -lmysql
```

5. Run the executable:

```bash
./hostel_management
```

---

## 💻 Sample Console Output

```
Welcome To Hostel Management System
***********************************
1. Reserve Bed:
2. Exit:
Enter Your Choice:
```

When a bed is reserved:

```
Bed is Reserved Successfully in 3star Hostel For Student John
Please Pay 5000 Rupees.
```

---

## 🚀 Future Enhancements

- Add support for multiple hostels.
- Implement student profile registration.
- Switch to a GUI using Qt or another C++ framework.
- Improve error handling and input validation.
- Add logging features for better tracking.

---





