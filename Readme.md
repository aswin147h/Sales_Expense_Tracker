# Smart Expense Tracker 💸

A Python-based Smart Expense Tracker application that helps users manage their daily expenses efficiently.  
This project demonstrates the implementation of:

- Python Fundamentals
- Object-Oriented Programming (OOP)
- File Handling
- Exception Handling
- REST API Integration
- Database Management

---

# 📌 Features

✅ Add Expenses  
✅ View Expenses  
✅ Update Expenses  
✅ Delete Expenses  
✅ Search Expenses by Category  
✅ Currency Conversion using API  
✅ Monthly Expense Reports  
✅ Export Reports to CSV/TXT  
✅ Database Storage using SQLite/MySQL  
✅ Proper Error Handling  

---

# 🛠 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core Programming |
| SQLite/MySQL | Database |
| Requests Library | API Integration |
| CSV Module | File Export |
| OOP | Project Structure |
| Exception Handling | Error Management |

---

# 📂 Project Structure

```text
smart_expense_tracker/
│
├── main.py
├── models/
│   ├── user.py
│   └── expense.py
│
├── services/
│   ├── expense_manager.py
│   ├── currency_api.py
│   └── report_generator.py
│
├── database/
│   └── db_manager.py
│
├── files/
│   ├── monthly_report.txt
│   └── expenses.csv
│
└── README.md
```

---

# ⚙️ Requirements

Install required packages:

```bash
pip install requests
```

If using MySQL:

```bash
pip install mysql-connector-python
```

---

# 🗄 Database Schema

## Users Table

```sql
CREATE TABLE users (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT,
    email TEXT
);
```

## Expenses Table

```sql
CREATE TABLE expenses (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    user_id INTEGER,
    title TEXT,
    amount REAL,
    category TEXT,
    date TEXT,
    currency TEXT,
    converted_amount REAL
);
```

---

# 🚀 How to Run the Project

## Step 1: Clone the Repository

```bash
git clone <repository-link>
```

---

## Step 2: Move into Project Folder

```bash
cd smart_expense_tracker
```

---

## Step 3: Run the Application

```bash
python main.py
```

---

# 📌 Main Functionalities

## 1. Add Expense

User can add:

- Expense Title
- Amount
- Category
- Currency
- Date

---

## 2. View Expenses

Displays all stored expenses from the database.

---

## 3. Update Expense

Allows editing existing expense details.

---

## 4. Delete Expense

Removes unwanted expense records.

---

## 5. Currency Conversion

Uses live API data to convert currencies into INR.

Example API:

```text
https://api.exchangerate-api.com/
```

---

## 6. Generate Monthly Report

Creates reports such as:

- Total Spending
- Category-wise Spending
- Highest Expense

---

## 7. Export Reports

Exports data into:

- TXT File
- CSV File

---

# 🧠 OOP Concepts Used

| Concept | Usage |
|---|---|
| Class | Expense, User |
| Object | Expense Entries |
| Encapsulation | Private Attributes |
| Inheritance | Optional Extensions |
| Polymorphism | Report Methods |

---

# ⚠️ Exception Handling

The project handles:

- Invalid Input Errors
- Database Errors
- File Errors
- API Connection Errors
- Currency Conversion Errors

Example:

```python
try:
    amount = float(input("Enter amount: "))
except ValueError:
    print("Invalid amount entered")
```

---

# 📁 File Handling

The project uses file handling for:

- Saving Reports
- Exporting CSV Files
- Reading Configurations

Example:

```python
with open("monthly_report.txt", "w") as file:
    file.write(report)
```

---

# 🌐 API Integration

This project uses a Currency Exchange API.

Example:

```python
import requests
```

API Features:

- Real-time exchange rates
- Currency conversion
- JSON response handling

---

# 📊 Future Improvements

✅ GUI using Tkinter  
✅ Authentication System  
✅ Charts using Matplotlib  
✅ Email Notifications  
✅ Cloud Database Integration  
✅ Web Version using Flask/Django  

---

# 🎯 Learning Outcomes

By building this project, you will learn:

- Real-world Python Development
- Database Operations
- API Consumption
- File Management
- Error Handling
- Clean Project Structure
- OOP Design Principles

---

# 👨‍💻 Author

Aswin

Python Developer | Data Engineering Enthusiast