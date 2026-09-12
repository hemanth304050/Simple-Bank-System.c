🏦 Bank Management System in C
A lightweight, console-based Bank Management System written in C. This application allows users to perform fundamental banking operations such as depositing, withdrawing, transferring funds, and tracking account activity with timestamped logs saved locally to a file.
✨ Features
 * Account Initialization: Prompts user for account holder name and account number upon startup.
 * Deposit Funds: Add money to your account with real-time balance updates.
 * Withdraw Funds: Secure withdrawal with built-in insufficient balance checks.
 * Fund Transfer: Transfer money to another account ID with validation.
 * Transaction Logs: Automatically records all transactions with precise dates and times using <time.h>.
 * Persistent Storage: Saves account details and transaction logs into an external Account.txt file.
 * Interactive Console UI: Clean, menu-driven interface using system clearances and custom dividers.
🛠️ Tech Stack
 * Language: C (C99 or later)
 * Libraries Used:
   * <stdio.h> for file handling and standard I/O operations.
   * <stdlib.h> for system commands and memory management.
   * <conio.h> for console input/output (getch()).
   * <time.h> for real-time transaction timestamps.
🚀 Getting Started
Prerequisites
Make sure you have a C compiler installed on your system (such as GCC, Clang, or MinGW for Windows). Note: This program utilizes <conio.h> and system("cls"), which are natively optimized for Windows environments.
Installation & Execution
 * Clone the repository:
   git clone https://github.com/your-username/bank-management-system.git
cd bank-management-system

 * Compile the source code:
   gcc bank.c -o bank

 * Run the executable:
   * Windows:
     bank.exe

   * Linux / macOS (Note: Requires adjustments for Windows-specific headers like <conio.h>):
     ./bank

📖 How to Use
 * Startup: Enter your Name and Account Number when prompted.
 * Main Menu: Select from the available options using numeric keys (1–6):
   * 1 ➡ Deposit money into your account.
   * 2 ➡ Withdraw money securely.
   * 3 ➡ Transfer money to another account number.
   * 4 📦 View current account details and total transaction counts.
   * 5 📄 View detailed transaction history logs.
   * 6 🚪 Exit the application.
📂 File Structure
📦 Bank-Management-System
 ┣ 📜 bank.c          # Main source code file
 ┣ 📜 Account.txt     # Generated local file storing user info & logs
 ┗ 📜 README.md       # Project documentation

💡 Future Enhancements
 * [ ] Support for multiple user accounts using structures and arrays/linked lists.
 * [ ] Password-protected login system for enhanced security.
 * [ ] Cross-platform compatibility (removing dependency on Windows-specific headers).
👤 Author
Hemanth
