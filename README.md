# Expense Tracker

## Description

A responsive web-based Expense Tracker built with HTML, CSS, and JavaScript. The application allows users to record income and expenses, automatically calculate their current balance, and manage transaction history with persistent browser storage.

---

## About This Project

This project was created to further develop and enhance my front-end web development skills, particularly in:

* JavaScript DOM manipulation
* Event-driven programming
* Working with the Local Storage API
* Dynamic UI updates
* Array manipulation and data processing
* Responsive web design
* Currency formatting using the Internationalization API
* Building interactive browser applications without frameworks
* Writing clean, maintainable JavaScript code

---

## Features

✨ **User Interface:**

* Clean and modern dashboard
* Real-time balance summary
* Responsive layout for desktop and mobile devices
* Organized transaction history
* Simple and intuitive transaction form

💰 **Core Functionality:**

* **Add Transactions** – Record income and expenses
* **Automatic Balance Calculation** – Instantly updates your remaining balance
* **Income & Expense Summary** – Separately tracks total income and expenses
* **Transaction History** – Displays transactions with the newest entries first
* **Delete Transactions** – Remove transactions with a single click
* **Persistent Storage** – Saves transactions using Local Storage
* **Currency Formatting** – Displays monetary values in a clean currency format
* **Responsive Design** – Works across desktop, tablet, and mobile devices

🔧 **Technology Stack:**

* **Markup:** HTML5
* **Styling:** CSS3
* **Programming Language:** JavaScript (ES6)
* **Storage:** Browser Local Storage
* **Architecture:** Vanilla JavaScript (No Frameworks)

---

## Project Structure

```text
04-Expense_Tracker/

├── Frontend
│   ├── index.html
│   ├── style.css
│   └── script.js
│
└── README.md
```

---

## How the Application Works

### Initial Load

* Loads previously saved transactions from Local Storage
* Displays the complete transaction history
* Calculates the current balance
* Updates the income and expense summaries automatically

### Add Transaction

* Users enter a transaction description
* Users enter an amount
* Positive amounts are treated as income
* Negative amounts are treated as expenses
* The transaction is saved instantly
* The dashboard updates automatically

### Delete Transaction

* Users click the **Delete (×)** button beside a transaction
* The selected transaction is removed
* The balance, income, and expense totals are recalculated immediately

### Persistent Storage

* Every transaction is stored in the browser using Local Storage
* Data remains available even after refreshing or reopening the application

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/04-Expense_Tracker.git
```

### 2. Navigate to the Project Folder

```bash
cd 04-Expense_Tracker
```

### 3. Run the Application

Open `Frontend/index.html` in your preferred web browser.

No installation, dependencies, or build process is required.

---

## Transaction Data Structure

Each transaction is stored as a JavaScript object:

```javascript
{
  id: Date.now(),
  description: "Salary",
  amount: 2500
}
```

The application automatically:

* Calculates the total balance
* Separates income from expenses
* Formats currency values
* Updates the dashboard whenever transactions are added or deleted
* Stores transaction data in Local Storage for future sessions
