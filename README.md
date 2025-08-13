# 📚 Student Management System (PyQt6 + SQLite)

A simple yet functional **Student Management System** built with **Python**, **PyQt6** for the graphical interface, and **SQLite** for data storage.

## ✨ Features
- ➕ **Add Student** — Add a new student with name, course, and mobile number
- 🔍 **Search Student** — Search for a student by name
- ✏ **Edit Student** — Update existing student details
- ❌ **Delete Student** — Delete a student with confirmation prompt
- 📜 **About** — Displays basic app information
- 📊 Table view of all students with instant refresh after each operation
- ✅ Success messages for every operation (Add, Edit, Delete)

## 🛠 Technologies Used
- **Python 3.10+**
- **PyQt6** — GUI framework
- **SQLite** — Local database

## 📂 Project Structure
project/
│-- icons/ # Toolbar icons (e.g. add.png, search.png)
│-- database.db # SQLite database
│-- main.py # Main application file
│-- README.md # Project description


## 📥 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/student-management-system.git
   cd student-management-system
2. Install dependencies:
   pip install PyQt6
3. Create the database
import sqlite3
conn = sqlite3.connect("database.db")
conn.execute("""
CREATE TABLE students (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT NOT NULL,
    course TEXT NOT NULL,
    mobile TEXT NOT NULL
)
""")
conn.close()
4. Run the app
python main.py

