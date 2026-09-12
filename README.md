# 🏦 Bank Management System

> 💳 A simple **Console-Based Bank Management System** developed in **C programming** to perform basic banking operations such as depositing money, withdrawing money, transferring money, checking account details, and viewing transaction history.

---

## 📌 Project Overview

The **Bank Management System** is a beginner-friendly C programming project that simulates basic banking operations through a command-line interface.

The project demonstrates important C programming concepts such as:

- 🧮 Variables and data types
- 🌍 Global variables
- 🔀 Conditional statements
- 🔁 Loops
- 🎯 Functions
- 📁 File handling
- ⏰ Date and time functions
- 🖥️ Console-based menus
- 🔐 Basic account information handling

All transaction details are stored in an `Account.txt` file.

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| 💰 Deposit Money | Add money to the account balance |
| 💸 Withdraw Money | Withdraw money from the account |
| 🔄 Transfer Money | Transfer money to another account number |
| 👤 Account Details | Display account holder information and balance |
| 📜 Transaction Details | View transaction history stored in the file |
| 🚪 Exit | Display final account details and exit the program |
| ⏰ Transaction Time | Records the date and time of transactions |
| 📁 File Storage | Saves account and transaction information in `Account.txt` |

---

## 🖥️ Menu

```text
--------------------------------------------------
                    MENU
--------------------------------------------------
1. Deposit Money
2. Withdraw Money
3. Transfer Money
4. Account details
5. Transaction details
6. Exit
--------------------------------------------------


---

## 🔄 How the System Works

1️⃣ Create Account

When the program starts, the user enters:

👤 Name

🔢 Account Number


The information is saved in:

Account.txt


---

2️⃣ 💰 Deposit Money

The user enters the amount they want to deposit.

Enter the amount you want to deposit
5000

*Money Deposited*
Now balance : 15000

The deposited amount and transaction time are stored in the account file.


---

3️⃣ 💸 Withdraw Money

The user enters the withdrawal amount.

The system checks whether the account has sufficient balance.

Enter the amount you want to withdraw
2000

Money withdrawn
Current balance : 13000

If the balance is insufficient:

*Insufficient balance*


---

4️⃣ 🔄 Transfer Money

The user enters:

🏦 Receiver's account number

💰 Transfer amount


Example:

Enter the account no. in which you want to transfer the money : 123456

Enter the amount you want to transfer
3000

*Money Transferred*
Current balance : 10000

The transaction is recorded in Account.txt.


---

5️⃣ 👤 Account Details

Displays:

Name

Account number

Current balance

Number of transactions


Example:

ACCOUNT DETAILS
--------------------------------------------------
Name : Hemanth
Account No. : 123456
Total balance = 10000

3 transactions have been made from your account


---

6️⃣ 📜 Transaction Details

The program reads Account.txt and displays the stored transaction history.

Example:

TRANSACTION DETAILS
--------------------------------------------------

Rs5000 had been deposited to your account
Date/Time of transaction : ...

Rs2000 had been withdrawn from your account
Date/Time of transaction : ...

Rs3000 had been transferred from your account to 123456
Date/Time of transaction : ...


---

## 📂 Project Structure

📦 Bank-Management-System
 ┣ 📜 Bank_Management_System.c
 ┣ 📄 Account.txt
 ┗ 📜 README.md


---

## 🛠️ Technologies Used

💻 Programming Language

🇨 C Programming


📚 C Libraries Used

## Library	Purpose

stdio.h	Input/output operations such as printf(), scanf(), fopen(), fprintf()
stdlib.h	Functions such as exit() and system()
conio.h	Console functions such as getch()
time.h	Date and time functions such as time() and ctime()



---

## 🧩 C Concepts Used

## 🎯 Functions

The project is divided into multiple functions for better organization:

deposit_money();
withdraw_money();
transfer_money();
checkDetail();
LastDetail();
transaction_details();
menu();
divider();


---

## 📁 File Handling

The program uses file handling to store account and transaction information.

FILE *ptr;

Different file modes are used:

"w"  // Write
"a"  // Append
"r"  // Read


---

## ⏰ Date & Time

Transaction date and time are recorded using:

time_t tm;
time(&tm);
ctime(&tm);


---

## 🔢 Global Variables

The program uses global variables to maintain account information and transaction data.

char name[20];
int dip_amt;
int amt = 10000;
int acc_no;
int ac;
int count = 0;
int trans_amt;
int with_amt;


---

## 💾 File Storage

The program creates a file named:

Account.txt

The file contains:

👤 Account holder name

🔢 Account number

💰 Deposit records

💸 Withdrawal records

🔄 Transfer records

⏰ Transaction date and time


Example:

Name : Hemanth
Account no. : 123456

Rs5000 had been deposited to your account
Date/Time of transaction : ...

Rs2000 had been withdrawn from your account
Date/Time of transaction : ...


---

## ⚙️ Requirements

To run this project, you need:

💻 A C compiler

🖥️ Windows environment recommended

📝 C-compatible IDE or compiler


## Recommended IDEs

🟦 Code::Blocks

🟩 Dev-C++

🟪 Visual Studio / Visual Studio Code with C compiler

🟨 Turbo C (for legacy conio.h support)


> ⚠️ Note: This project uses conio.h, getch(), and system("cls"), which are primarily associated with Windows/DOS environments. Some modern compilers may require modifications.




---

## 🚀 How to Run

Step 1️⃣ Clone the Repository

git clone https://github.com/your-username/Bank-Management-System.git

Step 2️⃣ Open the Project

Open the .c file using your preferred C IDE or editor.

Step 3️⃣ Compile the Program

Example:

gcc Bank_Management_System.c -o bank

Step 4️⃣ Run

bank

On Windows:

bank.exe


---

🧪 Example Workflow

🏦 BANK MANAGEMENT SYSTEM

Enter your name :
Hemanth

Enter your account no. :
123456

--------------------------------------------------
                    MENU
--------------------------------------------------

1. Deposit Money
2. Withdraw Money
3. Transfer Money
4. Account details
5. Transaction details
6. Exit

Enter your choice :

💰 Deposit

Enter the amount you want to deposit
5000

*Money Deposited*
Now balance : 15000

💸 Withdraw

Enter the amount you want to withdraw
2000

Money withdrawn
Current balance : 13000

🔄 Transfer

Enter the account no. in which you want to transfer the money :
987654

Enter the amount you want to transfer
3000

*Money Transferred*
Current balance : 10000


---

## 🧠 Learning Objectives

This project is useful for learning how to:

✅ Create functions in C

✅ Use global variables

✅ Work with files

✅ Read and write data

✅ Use loops and conditions

✅ Handle user input

✅ Create menu-driven programs

✅ Record date and time

✅ Build a simple real-world application using C



---

## 🔮 Future Improvements

This project can be upgraded with more advanced banking features:

🔐 PIN/password authentication

👥 Multiple user accounts

💾 Permanent account balance storage

🏦 Separate sender and receiver accounts

💳 ATM simulation

📱 Better user interface

🧾 Printable transaction statements

🔎 Search account functionality

🗑️ Delete account functionality

✏️ Update account information

💵 Balance validation

🚫 Prevention of negative deposits/withdrawals

🔒 Improved security

🗄️ Database integration

🌐 Online banking functionality



---

## ⚠️ Disclaimer

> 🚨 This is an educational C programming project created for learning purposes. It is not a real banking application and should not be used for handling real financial information or transactions.




---

## 📸 Project Type

🏦 Bank Management System
💻 Console Application
📝 C Programming Project
📁 File-Based Storage
🎓 Educational Project


---

## 👨‍💻 Author

Hemanth

💻 C Programming | 🚀 Software Development | 📚 Learning & Building


---

⭐ Support

If you found this project useful:

⭐ Star this repository

🍴 Fork the repository

🐛 Report issues

💡 Suggest improvements


---

## 📜 License

This project is intended for educational and learning purposes.


---

<div align="center">🏦 Bank Management System

Built with ❤️ using C

⭐ Star the repository if you like it!

</div>