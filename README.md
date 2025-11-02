🗂️ Python MySQL CRUD Application

This project is a command-line-based CRUD (Create, Read, Update, Delete) application built using Python, MySQL, and Tabulate.

It allows users to manage records in a MySQL database table (data) through a simple text menu interface.

🚀 Features

✅ Insert Records: Add new entries (Name, Age, Address, Contact, Mail) into the database.

📋 View Records: Display all stored records in a neatly formatted table using the tabulate library.

✏️ Update Records: Update specific fields (Name, Age, Address, Contact, Mail) for a selected record by ID.

🗑️ Delete Records: Remove a record from the database using its ID.

🔄 Menu-driven Interface: Simple loop-based menu for easy navigation.

🧰 Technologies Used

Python 3.x

MySQL Database

mysql-connector-python (for MySQL connection)

tabulate (for table display formatting)

⚙️ Setup Instructions


1️⃣ Install Required Libraries

Make sure Python is installed on your system, then install dependencies:

```
pip install mysql-connector-python
pip install tabulate
```
2️⃣ Create the Database and Table

In your MySQL command prompt or MySQL Workbench, create a database and table:

```
CREATE DATABASE ds_database;

USE ds_database;

CREATE TABLE data (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    address VARCHAR(255),
    contact VARCHAR(20),
    mail VARCHAR(100)
);

```
3️⃣ Update Database Credentials

In the Python code, update the connection settings as per your MySQL credentials:

```
con = mysql.connector.connect(
    host="localhost",
    user="root",
    password="your_password_here",
    database="ds_database"
)
```
4️⃣ Run the Program

Execute the script:

```
python app.py
```
🧮 Menu Options

When you run the program, you’ll see:

1. Insert Record

2. Select Record

3. Update Record

4. Delete Record

5. Exit


You can choose any option by entering the respective number.

📊 Example Output

Example table output using tabulate:

```
+----+----------+-------+----------------+-------------+---------------------+
| ID | NAME     | AGE   | ADDRESS        | CONTACT     | MAIL                |
+----+----------+-------+----------------+-------------+---------------------+
| 1  | Jyothi   | 21    | Coimbatore     | 9876543210  | jyothi@gmail.com    |
| 2  | Madesh   | 25    | Chennai        | 8765432109  | madesh@gmail.com    |
+----+----------+-------+----------------+-------------+---------------------+
```

🧑‍💻 Author

Jyothi Madesh

📧 Email: jyothimadesh00@gmail.com

💻 Project Type: Python + MySQL CRUD Application

🏁 License

This project is open-source and available for educational and personal use.
