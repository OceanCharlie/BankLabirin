# Bank Labirin - Customer Data Management System

**Version:** 3.1

A simple console application developed in **C++** to manage bank customer data. It utilizes a **Linked List** structure (*Stack*) for data storage and includes features for **Linear Search** and **Bubble Sort**. Customer data can be loaded from and exported to **CSV** files.

-----

## Key Features

  * **New Customer Input:** Add new customer data interactively through the console.
  * **Data Loading:** Load existing customer records from a **CSV** file.
  * **Data Structure:** Uses a **Stack** implemented with a **Linked List** (`push` and `pop` operations).
  * **Data Display:** Show all customer data in a clear, formatted table.
  * **Data Search:** Search for customers by name using **Linear Search**.
  * **Data Sorting:** Sort customer records by account type (*Tabungan, Giro, Investasi*) using **Bubble Sort**.
  * **Data Deletion:** Delete specific customer records based on a name search.
  * **File Output:** Save the current data set (all records or search results) to a new **CSV** file.

-----

## Requirements and Setup

### Prerequisites

  * A C++ Compiler (e.g., GCC, Clang) that supports standard C++.
  * An operating system (Windows or Linux/macOS).

### Compilation

Use a C++ compiler to compile the source file:

```bash
g++ bank-labirin.cpp -o bank-labirin
```

### Running the Application

**Linux/macOS:**

```bash
./bank-labirin
```

**Windows:**

```bash
bank-labirin.exe
```

-----

## Code Overview

The program uses the following structures to organize data:

| Structure Name | Description |
| :--- | :--- |
| `PersonalInfo` | Holds personal details (full name, birth place/date, address, etc.). |
| `AccountInfo` | Holds account details (account number, card number, account type, profession, etc.). |
| `Nasabah` | Combines `PersonalInfo` and `AccountInfo`. |
| `Node` | The element of the Linked List, containing `Nasabah` data and a pointer to the next node. |

-----

## How to Use

1.  **Start the Program:** Run the compiled executable.
2.  **Main Menu:**
      * **Option 1 (Load):** Enter the path to a `.csv` file to load existing customer data.
      * **Option 2 (Input):** Manually input data for a new customer.
3.  **Sub Menu (After Loading/Input):**
      * **Display:** View all current records.
      * **Search:** Find specific customers by name.
      * **Sort:** Order the list by account type.
      * **Delete:** Remove a record from the list.
      * **Output:** Save the current list (or search results) to a new `.csv` file.
