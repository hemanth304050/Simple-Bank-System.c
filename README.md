# 🏦 Bank Management System

A simple **console-based Bank Management System** built in C, allowing users to perform basic banking operations such as deposits, withdrawals, transfers, and transaction tracking — all through an interactive menu.

---

## ✨ Features

- 💰 **Deposit Money** — Add funds to your account
- 💸 **Withdraw Money** — Withdraw funds with balance validation
- 🔄 **Transfer Money** — Transfer funds to another account number
- 📋 **Account Details** — View name, account number, and current balance
- 🧾 **Transaction History** — View all past transactions with timestamps
- 🚪 **Exit** — Safely exit and view final account summary

---

## 🖥️ Tech Stack

| Component | Details |
|-----------|---------|
| Language  | C |
| Libraries | `stdio.h`, `stdlib.h`, `conio.h`, `time.h` |
| Storage   | Flat file (`Account.txt`) |
| Platform  | Windows (uses `conio.h` & `system("cls")`) |

---

## 📂 Project Structure

```

Bank-Management-System/
│
├── bank.c          # Main source code
├── Account.txt     # Auto-generated file storing account & transaction data
└── README.md        # Project documentation
```

---

## ⚙️ How It Works

1. On startup, the program asks for your **name** and **account number**.
2. These details are saved to `Account.txt`.
3. A menu is displayed with 6 options:

```
--------------------------------------------------
                    MENU
--------------------------------------------------
1. Deposit Money
2. Withdraw Money
3. Transfer Money
4. Account Details
5. Transaction Details
6. Exit
--------------------------------------------------
```

4. Every deposit, withdrawal, and transfer is logged with a **date & time stamp** into `Account.txt`.
5. Choosing **Exit** displays your final account summary before closing.

---

## 🚀 Getting Started

### Prerequisites
- A Windows machine (due to `conio.h` and `cls`)
- A C compiler (e.g., **MinGW / GCC**, Turbo C, or Code::Blocks)

### 🔧 Compile & Run

```bash
gcc bank.c -o bank
./bank
```

> 💡 If using an older compiler like Turbo C, you can compile and run directly within the IDE.

---

## 🧮 Default Balance

The system starts every account with a default balance of:

```
₹10,000
```

---

## ⚠️ Known Limitations

- Uses `gets()`, which is **deprecated and unsafe** — consider replacing with `fgets()`.
- Windows-only due to `conio.h` and `system("cls")`.
- No password/authentication layer — single-user session only.
- Balance and count reset every time the program restarts (not persisted, only transaction logs are).

---

## 🌱 Future Improvements

- [ ] Add multi-user/account support with login system
- [ ] Persist balance across sessions (not just logs)
- [ ] Replace unsafe `gets()` with `fgets()`
- [ ] Make cross-platform (remove `conio.h`, `system("cls")`)
- [ ] Add input validation for negative/invalid amounts

---

## 👤 Author

**Hemanth**
🔗 [Portfolio](https://dhkmyportfolio.netlify.app)

---

## 📄 License

This project is open-source and available for learning purposes.
