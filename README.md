# 🏦 Bank Management System

> 💰 A simple **Bank Management System built in C** that allows users to manage deposits, withdrawals, money transfers, account details, and transaction history through a console-based interface.

---

## ✨ Features

| Feature | Description |
|---|---|
| 💵 **Deposit Money** | Add money to the account balance |
| 💸 **Withdraw Money** | Withdraw money with insufficient-balance checking |
| 🔄 **Transfer Money** | Transfer money to another account number |
| 👤 **Account Details** | View account holder information and current balance |
| 📜 **Transaction Details** | View transactions stored in the account file |
| ⏰ **Date & Time** | Automatically records transaction date and time |
| 💾 **File Storage** | Stores account and transaction information in `Account.txt` |
| 🚪 **Exit** | Display final account details and safely exit |

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

🔧 Technologies Used

💻 C Programming

📂 File Handling

⏰ Date & Time

🧠 Functions

🔢 Global Variables

🔀 Switch Case

🔁 Loops

📥 User Input

🖥️ Console Interface



---

📚 C Libraries Used

#include <stdio.h>  // printf(), scanf()
#include <stdlib.h> // exit(), system()
#include <conio.h>  // getch()
#include <time.h>   // time(), ctime()


---

📂 Project Structure

Bank-Management-System/
│
├── 📄 main.c
├── 📄 Account.txt
└── 📄 README.md

> 💡 Account.txt is automatically created by the program to store account information and transaction records.




---

⚙️ How It Works

1️⃣ Create Account

When the program starts, the user enters:

Enter your name :
Enter your account no. :

The account information is stored in Account.txt.


---

2️⃣ 💵 Deposit Money

The user can enter an amount to deposit.

DEPOSITING MONEY
--------------------------------------------------
Enter the amount you want to deposit
5000

*Money Deposited*
Now balance : 15000

The transaction is saved with the date and time.


---

3️⃣ 💸 Withdraw Money

Users can withdraw money from their account.

The program checks whether sufficient balance is available.

WITHDRAWING MONEY
--------------------------------------------------
Enter the amount you want to withdraw
3000

Money withdrawn
Current balance : 12000

If the requested amount is greater than the available balance:

*Insufficient balance*


---

4️⃣ 🔄 Transfer Money

Users can transfer money by entering another account number.

TRANSFERRING MONEY
--------------------------------------------------
Enter the account no. in which you want to transfer the money : 123456

Enter the amount you want to transfer
2000

*Money Transferred*
Current balance : 10000

The transfer information is recorded in Account.txt.


---

5️⃣ 👤 Account Details

The account details option displays the account holder's information, account number, current balance, and transaction count.

ACCOUNT DETAILS
--------------------------------------------------
Name : Hemanth
Account No. : 123456
Total balance = 10000

3 transactions have been made from your account


---

6️⃣ 📜 Transaction Details

The transaction details option reads information from Account.txt and displays it on the console.

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

This project uses a text file called:

📄 Account.txt

The file is used to store:

👤 Account holder name

🔢 Account number

💵 Deposit records

💸 Withdrawal records

🔄 Transfer records

⏰ Transaction date and time



---

📄 File Modes Used

✏️ Write Mode

fopen("Account.txt", "w");

Creates or overwrites the account file.

➕ Append Mode

fopen("Account.txt", "a");

Adds new transaction information without deleting existing records.

📖 Read Mode

fopen("Account.txt", "r");

Reads stored account and transaction information.


---

🧩 Functions Used

The project is divided into multiple functions for better organization.

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

Function	Purpose

main()	Controls the overall program
menu()	Displays the main menu
deposit_money()	Handles deposits
withdraw_money()	Handles withdrawals
transfer_money()	Handles transfers
checkDetail()	Displays account details
transaction_details()	Displays transaction history
LastDetail()	Displays final account information
divider()	Prints the separator line



---

🚀 How To Run

🪟 Windows

This project is primarily designed for a Windows C compiler/environment because it uses:

#include <conio.h>

and:

system("cls");


---

1️⃣ Clone the Repository

git clone https://github.com/your-username/Bank-Management-System.git


---

2️⃣ Open the Project

Open the project in your preferred C development environment.

Recommended:

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

The main objective of this project is to understand how a real-world banking workflow can be represented using basic C programming concepts.

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

✨ Beginner-friendly C project

🏦 Banking operations simulation

💵 Deposit functionality

💸 Withdrawal functionality

🔄 Money transfer functionality

👤 Account details

📜 Transaction history

📂 File-based storage

⏰ Automatic transaction timestamps

🧩 Function-based program structure

🖥️ Console-based interface



---

🔮 Future Improvements

Some features that could be added in future versions:

🔐 Security Improvements

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

💳 Different account types

💰 Interest calculation

📊 Account statements

🧾 Improved transaction receipts

↩️ Transaction rollback


🗄️ Database Integration

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

⚠️ Important Note

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

1️⃣ Fork

🍴 Fork the repository.

2️⃣ Clone

📥 Clone the repository to your computer.

3️⃣ Create a Branch

🌱 Create a new branch for your feature.

4️⃣ Make Changes

🛠️ Improve the project or add a new feature.

5️⃣ Commit

💾 Commit your changes.

6️⃣ Push

🚀 Push your branch to GitHub.

7️⃣ Pull Request

🔀 Create a Pull Request.


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