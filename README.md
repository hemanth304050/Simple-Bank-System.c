# 🏦 Bank Management System in C

<p align="center">
  <img src="https://img.shields.io/badge/Language-C-blue?style=for-the-badge&logo=c" alt="C">
  <img src="https://img.shields.io/badge/Platform-Windows-informational?style=for-the-badge&logo=windows" alt="Windows">
  <img src="https://img.shields.io/badge/File%20Handling-Enabled-success?style=for-the-badge" alt="File Handling">
  <img src="https://img.shields.io/badge/Project-Beginner%20Friendly-orange?style=for-the-badge" alt="Beginner Friendly">
</p>

<p align="center">
  💰 <b>A simple console-based Bank Management System built using C programming.</b> 💰
</p>

<p align="center">
  <i>Deposit • Withdraw • Transfer • Account Details • Transaction History</i>
</p>

---

## 🌟 About The Project

**Bank Management System** is a beginner-friendly C programming project designed to demonstrate how basic banking operations can be implemented using fundamental programming concepts.

The program provides a simple **menu-driven console interface** where users can:

- 💵 Deposit money
- 💸 Withdraw money
- 🔄 Transfer money
- 👤 View account details
- 📜 View transaction history
- 🚪 Exit the application

Transaction information is stored in a text file named **`Account.txt`**, along with the date and time of transactions.

---

## ✨ Features

| 🔧 Feature | 📖 Description |
|---|---|
| 💵 **Deposit Money** | Add money to the current account balance |
| 💸 **Withdraw Money** | Withdraw money after checking available balance |
| 🔄 **Transfer Money** | Transfer money to another account number |
| 👤 **Account Details** | Display name, account number, balance and transaction count |
| 📜 **Transaction Details** | Display stored account and transaction information |
| ⏰ **Date & Time** | Automatically records transaction date and time |
| 💾 **File Storage** | Stores account and transaction information in `Account.txt` |
| 🚪 **Exit** | Displays final account details before exiting |

---

## 🖥️ Application Menu

```text
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


---

🔄 Program Workflow

🏦 BANK MANAGEMENT SYSTEM
                              │
                              ▼
                       👤 Enter Name
                              │
                              ▼
                     🔢 Enter Account No.
                              │
                              ▼
                         🖥️ Main Menu
                              │
          ┌───────────────────┼───────────────────┐
          ▼                   ▼                   ▼
      💵 Deposit         💸 Withdraw         🔄 Transfer
          │                   │                   │
          └───────────────────┼───────────────────┘
                              ▼
                     💰 Update Balance
                              │
                              ▼
                       📜 Save Transaction
                              │
                              ▼
                       📂 Account.txt


---

💵 1. Deposit Money

The user can deposit money into the account.

Example

DEPOSITING MONEY
--------------------------------------------------
Enter the amount you want to deposit
5000

*Money Deposited*
Now balance : 15000

The transaction is saved in Account.txt with its date and time.


---

💸 2. Withdraw Money

The user can withdraw money from the account.

Before withdrawing, the program checks whether sufficient balance is available.

Example

WITHDRAWING MONEY
--------------------------------------------------
Enter the amount you want to withdraw
3000

Money withdrawn
Current balance : 12000

❌ Insufficient Balance

If the withdrawal amount is greater than the available balance:

*Insufficient balance*


---

🔄 3. Transfer Money

The user can transfer money by entering the destination account number and transfer amount.

Example

TRANSFERRING MONEY
--------------------------------------------------
Enter the account no. in which you want to transfer the money : 123456

Enter the amount you want to transfer
2000

*Money Transferred*
Current balance : 10000

The transfer details are also stored in Account.txt.


---

👤 4. Account Details

The account details option displays important account information.

Example

ACCOUNT DETAILS
--------------------------------------------------
Name : Hemanth
Account No. : 123456
Total balance = 10000

3 transactions have been made from your account


---

📜 5. Transaction Details

The transaction details option reads information from Account.txt and displays it on the console.

Example

TRANSACTION DETAILS
--------------------------------------------------

Name : Hemanth
Account no. : 123456

Rs5000 had been deposited to your account
Date/Time of transaction : ...

Rs2000 had been withdrawn from your account
Date/Time of transaction : ...

Rs1000 had been transferred from your account to 987654
Date/Time of transaction : ...


---

📁 File Handling

This project uses a text file:

📄 Account.txt

The file stores:

👤 Account holder name

🔢 Account number

💵 Deposit transactions

💸 Withdrawal transactions

🔄 Transfer transactions

⏰ Transaction date and time



---

📂 File Modes Used

✏️ Write Mode

fopen("Account.txt", "w");

Used when the program starts to create or overwrite the account file.


---

➕ Append Mode

fopen("Account.txt", "a");

Used to add new transaction information without deleting previous records.


---

📖 Read Mode

fopen("Account.txt", "r");

Used to read and display stored account and transaction information.


---

🧩 Functions Used

The program is divided into separate functions to keep the code organized.

void deposit_money();
void withdraw_money();
void transfer_money();
void checkDetail();
void LastDetail();
void transaction_details();
void menu();
void divider();


---

📋 Function Responsibilities

Function	Responsibility

main()	Controls the overall program
menu()	Displays the main menu
deposit_money()	Handles money deposits
withdraw_money()	Handles money withdrawals
transfer_money()	Handles money transfers
checkDetail()	Displays account details
transaction_details()	Displays transaction history
LastDetail()	Displays final account details
divider()	Prints the separator line



---

🔧 Technologies Used

💻 C Programming
📂 File Handling
⏰ Date & Time
🧠 Functions
🔢 Variables
🔀 Switch Case
🔁 Loops
📥 User Input
🖥️ Console Interface


---

📚 C Libraries

The project uses the following C libraries:

#include <stdio.h>  // printf(), scanf()
#include <stdlib.h> // exit(), system()
#include <conio.h>  // getch()
#include <time.h>   // time(), ctime()

📌 Library Usage

Library	Purpose

stdio.h	Input/output and file handling
stdlib.h	exit() and system()
conio.h	getch()
time.h	Date and time information



---

📂 Project Structure

Bank-Management-System/
│
├── 📄 main.c
├── 📄 Account.txt
└── 📄 README.md

> 💡 Account.txt is created by the program and is used to store account and transaction information.




---

🚀 How To Run

🪟 Windows

This project is designed primarily for a Windows C environment because it uses:

#include <conio.h>

and:

system("cls");


---

1️⃣ Clone the Repository

git clone https://github.com/your-username/Bank-Management-System.git


---

2️⃣ Open the Project

Open the project folder in your preferred C development environment.

Examples:

💻 Visual Studio Code

🟦 Code::Blocks

🟢 Dev-C++

🟣 Visual Studio

⚙️ Any Windows-compatible C compiler



---

3️⃣ Compile

Using GCC:

gcc main.c -o bank


---

4️⃣ Run

bank


---

💻 Sample Program Execution

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

🧠 C Concepts Demonstrated

This project demonstrates several important C programming concepts:

📝 Variables

🌍 Global Variables

🔧 Functions

🔀 switch Statements

🔁 while Loop

🔄 for Loop

✅ if-else Conditions

📂 File Handling

⏰ Date & Time Functions

🧮 Arithmetic Operations

📥 User Input

📤 Console Output

💾 Data Storage

🚪 Program Termination



---

🎯 Learning Objective

The main objective of this project is to understand how a basic real-world banking workflow can be represented using C programming.

The project combines:

👤 User Input
      ↓
🧠 C Functions
      ↓
💰 Banking Operations
      ↓
🧮 Balance Calculation
      ↓
📂 File Handling
      ↓
📜 Transaction History


---

⭐ Project Highlights

<div align="center">💡	Highlight

💻	Beginner-friendly C project
🏦	Banking operations simulation
💵	Deposit functionality
💸	Withdrawal functionality
🔄	Money transfer functionality
👤	Account details
📜	Transaction history
📂	File-based storage
⏰	Automatic transaction timestamps
🧩	Function-based program structure
🖥️	Console-based interface


</div>
---

🔮 Future Improvements

The project can be further improved by adding:

🔐 Security

🔑 Login system

🔢 PIN authentication

🔒 Password protection

🛡️ Data encryption


👥 Account Management

➕ Create multiple accounts

🗑️ Delete accounts

🔎 Search accounts

✏️ Update account information


💰 Banking Features

💳 Account types

💰 Interest calculation

📊 Account statements

🧾 Improved transaction receipts

↩️ Transaction rollback


🗄️ Database

Replace the text file with:

🗄️ MySQL
🗄️ SQLite
🗄️ PostgreSQL

for more structured data management.

🖥️ User Interface

Future versions could include:

🖥️ GUI Application
🌐 Web Application
📱 Mobile Application


---

⚠️ Important Disclaimer

> 🚨 Educational Project Only



This project is created for learning and educational purposes.

It is not a real banking application and should not be used to handle real financial information, real bank accounts, passwords, or transactions.

The current version stores information in a plain text file and does not provide:

❌ Authentication

❌ Password encryption

❌ Database security

❌ Secure transaction processing

❌ Real banking connectivity

❌ Multi-user security



---

🤝 Contributing

Contributions are welcome! 🎉

If you would like to improve this project:

1️⃣ Fork the repository
        ↓
2️⃣ Clone the repository
        ↓
3️⃣ Create a new branch
        ↓
4️⃣ Make your changes
        ↓
5️⃣ Commit your changes
        ↓
6️⃣ Push your changes
        ↓
7️⃣ Create a Pull Request

Example

git clone https://github.com/your-username/Bank-Management-System.git

git checkout -b feature/new-feature

git add .

git commit -m "Add new feature"

git push origin feature/new-feature

Then open a Pull Request 🚀


---

📜 License

This project is intended for educational purposes.

Feel free to use, modify, and improve the code for learning and academic projects.


---

👨‍💻 Author

Dhannodi Hemanth Kumar

💻 C Programming Enthusiast
🏦 Bank Management System Project

⭐ If you found this project useful, please consider giving the repository a Star!


---

❤️ Support

If you like this project:

⭐ Star the repository

🍴 Fork the repository

📢 Share the project

🐛 Report issues

💡 Suggest improvements


---

🏦 Bank Management System

╔══════════════════════════════════════════════╗
║                                              ║
║        🏦 BANK MANAGEMENT SYSTEM 🏦          ║
║                                              ║
║       💰 Deposit • Withdraw • Transfer      ║
║       👤 Account • 📜 Transactions           ║
║                                              ║
║              Built with ❤️ in C              ║
║                                              ║
╚══════════════════════════════════════════════╝

<p align="center">
  <b>💻 Simple Banking • Built with C • Made for Learning ❤️</b>
</p><p align="center">
  ⭐ <b>Don't forget to Star the Repository!</b> ⭐
</p>
```