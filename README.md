# 🏦 Bank Management System

A **console-based Bank Management System** developed using **Python** and **MySQL**. This project provides secure banking operations through separate **User** and **Admin** modules. Users can manage their bank accounts, while administrators can monitor users and transactions efficiently. 

---

# 📌 Description

The Bank Management System is designed to perform essential banking operations using a command-line interface. It securely stores customer information in a MySQL database and allows users to perform transactions while providing administrators with complete control over account management and transaction monitoring.

---

# 🚀 Technologies Used

🐍 Python

🗄️ MySQL

💻 VS Code

🛠️ MySQL Workbench

---

# ✨ Features

## 👤 User Module

✅ Register New User

🔐 Secure Login

👀 View Account Details

💸 Debit Money

💰 Credit Money

🔑 Change PIN

📄 View Transaction Statement

🚪 Logout

---

## 👨‍💼 Admin Module

🔐 Secure Admin Login

👥 View All Users

🔍 View User Details

📜 View User Transactions

📅 View Day-wise Transactions

🚪 Logout

---

# 📂 Project Structure

```text
Bank-Management-System/
│
├── bank_management_system.py
├── database.sql
└── README.md
```

---

# 🖥️ Python Console Output

## 🏠 Main Menu

```text
--- Bank Management System ---

1. Register User
2. User Login
3. Admin Login
4. Exit
```

---

## 📝 User Registration

```text
Enter Name: Diya
Enter Account Type (Savings/Current): Savings
Set 4-digit PIN: 1234
Enter Initial Deposit: 30000

✅ Registration successful!
🏦 Your Account Number is: 238007537223
```

---

## 🔐 User Login

```text
Enter Account Number: 238007537223
Enter PIN: 1234

🎉 Welcome Diya!

1. View Account
2. Debit
3. Credit
4. Change PIN
5. Statement
6. Logout
```

---

## 👀 View Account

```text
Name: Diya
Account No: 238007537223
Type: Savings
Balance: 30000.0
```

---

## 💸 Debit Transaction

```text
Enter amount to debit: 3000

✅ Amount debited successfully!
```

---

## 💰 Credit Transaction

```text
Enter amount to credit: 1200

✅ Amount credited successfully!
```

---

## 🔑 Change PIN

```text
Enter old PIN: 1234
Enter new PIN: 0099

✅ PIN changed successfully!
```

---

## 📄 Transaction Statement

```text
(1, 238007537223, 'Debit', 3000.0, datetime.datetime(2026, 7, 4, 12, 25, 40))

(2, 238007537223, 'Credit', 1200.0, datetime.datetime(2026, 7, 4, 12, 25, 44))
```

---

## 👨‍💼 Admin Login

```text
Enter Admin ID: 1
Enter Password: Diya123

✅ Admin Login Successful!
```

---

## 👥 View All Users

```text
Account No: 238007537223
Name: Diya
Type: Savings
Balance: 28200.0
```

---

## 🔍 View User Details

```text
Account No: 238007537223
Name: Diya
Type: Savings
Balance: 28200.0
```

---

## 📜 View User Transactions

```text
(1, 238007537223, 'Debit', 3000.0, datetime.datetime(2026, 7, 4, 12, 25, 40))

(2, 238007537223, 'Credit', 1200.0, datetime.datetime(2026, 7, 4, 12, 25, 44))
```

---

## 📅 View Day Transactions

```text
Enter Date (YYYY-MM-DD): 2026-07-04

(1, 238007537223, 'Debit', 3000.0, datetime.datetime(2026, 7, 4, 12, 25, 40))

(2, 238007537223, 'Credit', 1200.0, datetime.datetime(2026, 7, 4, 12, 25, 44))
```

---

# 🗄️ MySQL Database Output

## 👤 Users Table

| 🏦 Account No | 👤 Name | 💳 Account Type | 🔑 PIN | 💰 Balance |
|---------------|--------- |----------------|-------- |------------ |
| 238007537223  | Diya     | Savings        | 0099    | 28200       |
| 238007537224  | Likhitha | Current        | 0909    | 18000       |
| 238007537225  | Lavanya  | Savings        | 3645    | 59000       |
| 238007537227  | Rupa     | Savings        | 2901    | 57000       |
| 238007537228	 | Jhansi   | Current        | 7676    | 25000       |

---

## 📜 Transactions Table

| 🆔 Transaction ID | 🏦 Account No | 🔄 Action | 💵 Amount | 🕒 Date & Time      |
| ----------------- | ------------- | --------- | --------: | ------------------- |
| 1                 | 238007537223  | Debit     |      3000 | 2026-07-04 12:25:40 |
| 2                 | 238007537223  | Credit    |      1200 | 2026-07-04 12:25:44 |
| 3                 | 238007537224  | Debit     |      7000 | 2026-07-04 21:16:49 |
| 4                 | 238007537225  | Debit     |      6000 | 2026-07-04 21:20:14 |
| 5                 | 238007537226  | Credit    |      7000 | 2026-07-04 21:22:52 |
| 6                 | 238007537228  | Debit     |     30000 | 2026-07-04 21:26:35 |
| 7                 | 238007537228  | Credit    |     10000 | 2026-07-04 21:26:51 |

---

## 👨‍💼 Admin Table

| 👤 Admin ID | 🔐 Password |
|-------------|------------- | 
|    1        | Diya123      |
|    2        | Likhitha123  |
|    3        | Lavanya123   |
|    4        | Rupa123      |
|    5        | Jhansi123    | 

---

# 🎯 Future Enhancements

🎨 Develop a GUI Version

🔒 Encrypt User PINs

💳 Add Fund Transfer Between Accounts

📑 Generate PDF Account Statements

📧 Email/SMS Notifications

📊 Dashboard with Banking Analytics

☁️ Cloud Database Integration

🔐 OTP-based Authentication
