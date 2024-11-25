
# Banking System using JDBC

Welcome to the **Banking System** project! This is a Java-based application that uses JDBC (Java Database Connectivity) to interact with a MySQL database, allowing users to manage their bank accounts, perform transactions, and ensure secure financial data management.

## 🚀 Getting Started

Follow these steps to set up and run the project on your local machine:

### 1. **Clone the Repository**
If you haven't cloned the repository yet, use the following command to clone it:

```bash
git clone https://github.com/YourUsername/BankingSystem.git
```

### 2. **Database Setup**

Before running the application, you need to set up the MySQL database. Use the SQL script below to create the database and tables.

```sql
CREATE DATABASE banking_system;

USE banking_system;

CREATE TABLE User (
    id INT AUTO_INCREMENT PRIMARY KEY,
    full_name VARCHAR(255),
    email VARCHAR(255) UNIQUE,
    password VARCHAR(255)
);

CREATE TABLE Account (
    account_number BIGINT PRIMARY KEY,
    full_name VARCHAR(255),
    email VARCHAR(255) UNIQUE,
    balance DECIMAL(10, 2),
    security_pin VARCHAR(10)
);
```

Make sure to replace the database connection details in `Database.java` with your MySQL credentials.

### 3. **Build and Run the Project**

1. **Compile the Java Code**:
   ```bash
   javac *.java
   ```

2. **Run the Application**:
   ```bash
   java BankingSystem
   ```

### 4. **Usage**

- **User Registration**: Users can register by providing their full name, email, and password.
- **Account Creation**: After registering, users can create a new bank account.
- **Login**: Registered users can log in by providing their email and password.
- **Account Operations**: Once logged in, users can perform operations like checking balance, transferring money, and updating their security pin.

---

## 📂 Project Structure

- **`src/`**: Contains the Java source code files.
- **`database/`**: Includes SQL scripts for database setup.
- **`screenshots/`**: Screenshots of the application in action.

---

## 📦 Features

- **User Registration & Login**: Users can register, log in, and manage their personal information.
- **Account Creation**: Users can open a new bank account with an initial deposit.
- **Balance Inquiry**: Check the balance of a bank account.
- **Money Transfer**: Transfer money between different accounts.
- **Security**: Uses a security PIN to validate transactions and account access.

---

## 🌐 Technologies Used

- **Java**: Programming language used to build the application.
- **JDBC**: Java Database Connectivity to interact with the MySQL database.
- **MySQL**: Database system used for storing user and account information.

---

## 📸 Screenshots

- **Registration Screen**: ![Registration Screenshot](screenshots/registration.png)
- **Login Screen**: ![Login Screenshot](screenshots/login.png)

---

## 🤝 Contributing

We welcome contributions to improve the project! Feel free to submit issues or pull requests.

### Steps to Contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Create a new Pull Request.

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🏁 Final Note

Thank you for checking out the **Banking System** project! 🎉 Happy coding!

