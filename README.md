# 💊 Pharmacy Management System (Medical Store System)

A C-based Medical Store System designed to enable seamless management of pharmaceutical sales, inventory, and user interactions. This application was developed to simulate the essential operations of a medical store with different access levels: **Admin**, **Manager**, and **Customer**.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [System Architecture](#system-architecture)
- [How to Run](#how-to-run)
- [Screenshots](#screenshots)
- [Project Contributors](#project-contributors)
- [References](#references)

---

## 📖 Overview

The project was designed in response to challenges faced during the pandemic, offering a digital platform for small medical stores to manage sales, inventory, customer feedback, and online orders. With structured roles and persistent file storage, the system mirrors real-world operations of a retail pharmacy.

---

## ✨ Features

### 👤 User Roles
- **Admin**
  - Manage customer accounts
  - View sales and profit reports
  - Handle feedback and manager requests
  - Send messages to managers
- **Manager**
  - View and manage inventory
  - Process pending orders
  - Generate sales reports
  - Communicate with Admin
- **Customer**
  - Sign up / Sign in
  - Browse available medicines
  - Place orders with optional voucher discounts
  - Submit feedback

### 📦 Core Functionalities
- Medicine stock management (Add / Modify / Delete)
- Customer account management
- Sales tracking and reports
- Order processing and voucher validation
- Feedback and messaging system
- Persistent file storage for all data

---

## 🧰 Technology Stack

- **Language**: C
- **Platform**: Windows
- **Compiler**: Turbo C / Code::Blocks / Dev-C++
- **Libraries Used**:
  - `<stdio.h>`, `<stdlib.h>`, `<conio.h>`, `<string.h>`, `<windows.h>`, `<ctype.h>`, `<time.h>`

---

## 🏗 System Architecture

```text
Main.c
├── login() → Sign In / Sign Up
│   ├── Admin → mainadminmenu()
│   ├── Manager → mainmanagermenu()
│   └── Customer → maincustomermenu()
│
├── File-Based Storage:
│   ├── customers.txt     → Stores user credentials
│   ├── medicines.txt     → Stores medicine inventory
│   ├── sales.txt         → Stores sales logs
│   ├── feedback.txt      → Stores customer feedback
│   ├── message.txt       → Admin-to-Manager messages
│   ├── requests.txt      → Manager-to-Admin requests
│   └── vouchers.txt      → Discount vouchers
```
---

## 🛠 How to Run

### 1. Compile the Code

Use any Windows-compatible C compiler like Turbo C, Dev-C++, or Code::Blocks:
```text
gcc "Pharmacy Final Project.c" -o PMS.exe
```
### 2. Run the Executable
```text
PMS.exe
```
Ensure all .txt files mentioned above are created in the working directory or will be created during runtime.

---

## 📚 References

## 📚 References

- [C Programming with File Handling](https://www.geeksforgeeks.org/basics-file-handling-c/)
- [Windows Console Functions (gotoxy, SetConsoleCursorPosition)](https://learn.microsoft.com/en-us/windows/console/setconsolecursorposition)
- [Turbo C / Dev C++ for Beginners](https://www.tutorialspoint.com/cprogramming/index.htm)

---

## 💡 This project is a semester-based final assignment built using C, demonstrating concepts like structures, file handling, conditionals, loops, modular design, and basic UI using the console.
