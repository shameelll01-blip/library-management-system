
#  Library Management System (MySQL Project)

##  Overview

This project is a **Library Management System** implemented using **MySQL**. It manages information about books, customers, employees, and transactions such as issuing and returning books.

---

##  Database Name

**library**

---

##  Tables Created

### 1. Branch

Stores branch details.

* Branch_no (Primary Key)
* Manager_Id
* Branch_address
* Contact_no

---

### 2. Employee

Stores employee information.

* Emp_Id (Primary Key)
* Emp_name
* Position
* Salary
* Branch_no (Foreign Key → Branch)

---

### 3. Books

Stores book details.

* ISBN (Primary Key)
* Book_title
* Category
* Rental_Price
* Status (Yes/No)
* Author
* Publisher

---

### 4. Customer

Stores customer details.

* Customer_Id (Primary Key)
* Customer_name
* Customer_address
* Reg_date

---

### 5. IssueStatus

Tracks issued books.

* Issue_Id (Primary Key)
* Issued_cust (Foreign Key → Customer)
* Issued_book_name
* Issue_date
* Isbn_book (Foreign Key → Books)

---

### 6. ReturnStatus

Tracks returned books.

* Return_Id (Primary Key)
* Return_cust
* Return_book_name
* Return_date
* Isbn_book2 (Foreign Key → Books)

---

##  Features

* Manage books and their availability
* Track issued and returned books
* Maintain employee and branch details
* Store customer registration data
* Perform analytical queries

---

##  Queries Implemented

1. Display available books (title, category, rental price)
2. List employees by salary (descending)
3. Show issued books with customer names
4. Count books by category
5. Employees earning more than ₹50,000
6. Customers registered before 2022 with no issued books
7. Employee count per branch
8. Customers who issued books in June 2023
9. Books containing "history" in title
10. Branches with more than 5 employees
11. Managers and their branch addresses
12. Customers who issued books with rental price > ₹25

---

##  Sample Operations

* Insert data into all tables
* Retrieve records using SELECT queries
* Use JOIN operations for relational data
* Apply aggregate functions (COUNT, SUM)

---

##  Tools Used

* MySQL Workbench
* SQL (Structured Query Language)

---

##  Outcome

This project demonstrates:

* Database design using relational models
* Use of primary and foreign keys
* Query writing and data retrieval
* Real-world database application (Library System)

---

##  Conclusion

The Library Management System efficiently organizes and manages library data, making it easier to track books, customers, and transactions.

---
