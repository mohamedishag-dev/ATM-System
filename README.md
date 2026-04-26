# ATM-System
## 📌 Overview
This project simulates a basic ATM system using C++.
It allows users to log in with their Account Number and Pin Code, then perform standard banking operations such as:

- Quick Withdraw (predefined amounts)
- Normal Withdraw (custom amount, multiple of 5)
- Deposit
- Check Balance
- Logout

The system stores client data in a text file (``Clients.txt``) and updates balances after each transaction.

## ⚙️ Features
- Login System: Validates account number and pin code.
- File Handling: Reads and writes client data from Clients.txt.
- Withdraw Options:
   - Quick withdraw (20, 50, 100, 200, 400, 600, 800, 1000).
   - Normal withdraw (any multiple of 5).
- Deposit: Add funds to account balance.
- Balance Check: Displays current account balance.
- Data Persistence: Updates saved client records after transactions.
---
## 🗂️ Data Structure
Each client is represented by the following structure:

```cpp
struct sClient {

    string AccountNumber;
    string PinCode;
    string Name;
    string Phone;
    double AccountBalance;
    bool MarkForDelete;
    
};
```
## 📄 File Format
Clients are stored in Clients.txt with the following format:
```
Code
AccountNumber#//#PinCode#//#Name#//#Phone#//#AccountBalance
```
Example:
```
Code
A1001#//#1234#//#Mohamed Ali#//#01012345678#//#5000.75
```
## ▶️ How to Run
1- Compile the program:
```
bash
g++ ATM.cpp -o ATM
```
2- Run the executable:
```
bash
./ATM
```
3- Enter your **Account Number** and **Pin Code** to log in.

4- Choose from the main menu options.
