🏦 Bank Management System

«💰 A simple Bank Management System built in C that allows users to manage deposits, withdrawals, money transfers, account details, and transaction history through a console-based interface.»

---

✨ Features

Feature | Description
# 💵 Deposit Money| Add money to the account balance
# 💸 Withdraw Money| Withdraw money with insufficient-balance checking
# 🔄 Transfer Money| Transfer money to another account number
# 👤 Account Details| View account holder information and current balance
# 📜 Transaction Details| View transactions stored in the account file
# 🚪 Exit| Display final account details and safely exit

---

🖥️ Menu

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

🔧 Technologies Used

💻 C Programming

📂 File Handling

⏰ Date & Time

🧠 Functions

🔢 Global Variables

🔀 Switch Case

📥 User Input

🖥️ Console Interface

---

📚 C Libraries Used

#include <stdio.h>
#include <stdlib.h>
#include <conio.h>
#include <time.h>

---

📂 Project Structure

Bank-Management-System/
│
├── 📄 main.c
├── 📄 Account.txt
└── 📄 README.md

«"Account.txt" is automatically created by the program to store account information and transaction records.»

---

⚙️ How It Works

1️⃣ Create Account

When the program starts, the user enters:

Enter your name :
Enter your account no. :

The information is stored in "Account.txt".

---

2️⃣ 💵 Deposit Money

The user can enter an amount to deposit.

Example:

Enter the amount you want to deposit
5000

*Money Deposited*
Now balance : 15000

The transaction is also recorded with the date and time.

---

3️⃣ 💸 Withdraw Money

Users can withdraw money from their account.

The program checks whether sufficient balance is available.

Enter the amount you want to withdraw
3000

Money withdrawn
Current balance : 12000

If the requested amount is greater than the balance:

*Insufficient balance*

---

4️⃣ 🔄 Transfer Money

Users can transfer money by entering another account number.

Enter the account no. in which you want to transfer the money : 123456

Enter the amount you want to transfer
2000

*Money Transferred*
Current balance : 10000

The transfer is recorded in "Account.txt".

---

5️⃣ 👤 Account Details

The account details option displays:

ACCOUNT DETAILS
--------------------------------------------------

Name : Your Name
Account No. : 123456
Total balance = 10000

3 transactions have been made from your account

---

6️⃣ 📜 Transaction Details

All stored account and transaction information can be viewed through the transaction details option.

Example:

TRANSACTION DETAILS
--------------------------------------------------

Name : Your Name
Account no. : 123456

Rs5000 had been deposited to your account
Date/Time of transaction : ...

Rs2000 had been withdrawn from your account
Date/Time of transaction : ...

Rs1000 had been transferred from your account to 987654
Date/Time of transaction : ...

---

📁 File Handling

This project uses a text file called:

Account.txt

The file is used to store:

👤 Account holder name

🔢 Account number

💵 Deposit records

💸 Withdrawal records

🔄 Transfer records

⏰ Transaction date and time

---

📄 File Modes Used

fopen("Account.txt", "w");

Creates/overwrites the account file.

fopen("Account.txt", "a");

Adds new transaction information to the existing file.

fopen("Account.txt", "r");

Reads transaction information from the file.

---

🧩 Functions

The project is divided into multiple functions for better organization.

void deposit_money();
void withdraw_money();
void transfer_money();
void checkDetail();
void LastDetail();
void transaction_details();
void menu();
void divider();

Function Responsibilities

Function| Purpose
# "menu()"| Displays the main menu
# "deposit_money()"| Handles deposits
# "withdraw_money()"| Handles withdrawals
# "transfer_money()"| Handles transfers
# "checkDetail()"| Displays account details
# "transaction_details()"| Displays transaction history
# "LastDetail()"| Displays final account information
# "divider()"| Prints the separator line

---

🚀 How to Run

🪟 Windows

This project uses:

#include <conio.h>

and:

system("cls");

So it is primarily designed for a Windows C compiler/environment.

▶️ Compile

Using GCC:

gcc main.c -o bank

▶️ Run

bank

---

💻 Example

Enter your name :
Hemanth

Enter your account no. : 123456

--------------------------------------------------
                    MENU
--------------------------------------------------
1.Deposit Money
2.Withdraw Money
3.Transfer Money
4.Account details
5.Transaction details
6.Exit
--------------------------------------------------

Enter your choice :
1

DEPOSITING MONEY
--------------------------------------------------
Enter the amount you want to deposit
5000

*Money Deposited*
Now balance : 15000

---

🧠 Concepts Demonstrated

This project is useful for learning fundamental C programming concepts such as:

📝 Variables

🌍 Global variables

🔧 Functions

🔀 "switch" statements

🔁 Loops

📂 File handling

⏰ Time/date functions

🧮 Arithmetic operations

✅ Conditional statements

📥 Input/output

🖥️ Console-based applications

---

⚠️ Important Note

This is an educational project created to demonstrate C programming and basic banking operations.

It is not a real banking application and should not be used for handling real financial information or transactions.

The current version stores account information in a plain text file and does not include authentication, encryption, database security, or real banking connectivity.

---

🔮 Future Improvements

Some features that could be added in future versions:

🔐 Login system with PIN/password

🗄️ Database integration

👥 Multiple bank accounts

💳 Account creation and deletion

🔎 Search accounts

📊 Transaction reports

🧾 Better transaction history

💰 Interest calculation

🔒 Password encryption

🛡️ Input validation

↩️ Transaction rollback

🌐 Online banking functionality

🖥️ GUI interface

📱 Mobile application

---

🎯 Learning Objective

The main objective of this project is to understand how a real-world banking workflow can be represented using basic C programming concepts.

It combines:

👤 User Input
      ↓
🧠 C Functions
      ↓
💰 Account Operations
      ↓
📂 File Storage
      ↓
📜 Transaction History

---

⭐ Project Highlights

✨ Beginner-friendly C project

💰 Basic banking operations

📂 File-based transaction storage

⏰ Automatic transaction timestamps

🧩 Function-based program structure

🖥️ Simple console interface

📚 Great for C programming practice

---

🤝 Contributing

Contributions are welcome! 🎉

If you would like to improve this project:

1. 🍴 Fork the repository
2. 📥 Clone the repository
3. 🌱 Create a new branch
4. 🛠️ Make your changes
5. 💾 Commit your changes
6. 🚀 Push the branch
7. 🔀 Create a Pull Request

---

📜 License

This project is intended for educational purposes.

Feel free to use, modify, and improve the code for learning and academic projects.

---

👨‍💻 Author

Dhannodi Hemanth Kumar

⭐ If you found this project useful, consider giving the repository a Star!

---

🏦 Simple Banking. Built with C. 💻

╔══════════════════════════════════════════════╗
║        🏦 BANK MANAGEMENT SYSTEM 🏦          ║
║                                              ║
║       💰 Deposit • Withdraw • Transfer      ║
║       👤 Account • 📜 Transactions           ║
║                                              ║
║              Built with ❤️ in C              ║
╚══════════════════════════════════════════════╝