
# 🏦  Bank Ltd. – Java Console-Based Banking System

Welcome to ** Bank Ltd.**, a fully console-driven banking application developed in **Java** that simulates core banking operations like login, account creation, fund transfer, and account management.

This project is ideal for **educational purposes**, helping developers understand file handling, OOP principles, and console-based user interaction in Java.

---

## 📋 Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Application Flow](#application-flow)
- [Data Storage Details](#data-storage-details)
- [Security & Limitations](#security--limitations)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## ✅ Features

- 👤 **User Authentication**: Login system with file-based credential verification.
- 🆕 **Account Creation**: Easily create new accounts with user details and initial deposit.
- 💰 **Balance Inquiry**: Check your account balance at any time.
- 📝 **Account Details**: View your personal account information.
- 🔁 **Fund Transfer**: Transfer money to another registered account.
- 📈 **Bank Statement**: View your transaction history.
- ❌ **Account Closure**: Delete your account permanently.
- 🔒 **Logout & Exit Options**: Securely log out or exit the application.
- 🗂️ **File-based Data Persistence**: All data is stored using local text files.

---

## 🧱 Project Structure

```plaintext
accountdetails/
├── Main.java                # Main class: handles app flow and user interaction
├── Login.java               # Login logic
├── Creation.java            # Account creation logic
├── BalanceInquiry.java      # Balance checking logic
├── AccountDetails.java      # Retrieves and displays user info
├── Transaction.java         # Handles fund transfers
├── BankStatement.java       # Displays transaction history
├── Deletion.java            # Account closure and cleanup
└── db/                      # Data storage
    ├── credentials.txt      # Stores usernames and passwords
    ├── userDB.txt           # Stores user information
    ├── balanceDB.txt        # Stores balances
    └── transactionDB.txt    # (Optional) Records transaction logs
```

---

## 🛠️ Technologies Used

- **Java SE (Standard Edition)**
- File I/O (`java.io`)
- Scanner for console input
- OOP principles (Composition, Encapsulation)
- Exception Handling

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/AhmeRezk-22/bank-OOP/
cd bank-OOP
```

### 2. Compile the Code
```bash
javac accountdetails/*.java
```

### 3. Run the Application
```bash
java accountdetails.Main
```

---

## 🔄 Application Flow

```plaintext
Start → Welcome Menu
     ├── 1: Login
     │     └── Validate → Main Menu
     └── 2: Create Account
            └── Register → Main Menu

Main Menu:
  ├── Balance Inquiry
  ├── Account Details
  ├── Fund Transfer
  ├── Bank Statement
  ├── Account Closure
  ├── Logout → Welcome Menu
  └── Exit
```

---

## 📂 Data Storage Details

- **credentials.txt**:  
  Format: `accountNo:password`  
  Used for login authentication.

- **userDB.txt**:  
  Format: `accountNo|name|phone|email|dob|address`  
  Stores user profile data.

- **balanceDB.txt**:  
  Format: `accountNo:balance`  
  Stores user balance information.

- **transactionDB.txt** *(optional)*:  
  Logs details of every transaction for statement viewing.

> All files are stored under the `db/` folder. Make sure this directory exists before running the application.

---

## 🔐 Security & Limitations

- Passwords are stored in **plain text** (no hashing or encryption).
- No input sanitization for names, phone, etc.
- No database or GUI integration — strictly file-based and console-driven.
- **No concurrency control** — simultaneous access may cause data corruption.

This app is meant for **educational/demo purposes only**.

---

## 🌱 Future Improvements

- 🔐 Add password hashing (e.g., BCrypt)
- 📊 GUI integration (JavaFX/Swing)
- ☁️ Migrate to a database (e.g., SQLite, MySQL)
- 📅 Add transaction timestamps and categories
- 🧪 Implement unit tests

---

## 📄 License

This project is open source.

---

