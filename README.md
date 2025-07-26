# Advanced Java Core: Transaction System

## Overview

This is a Java project which use CLI. You can see your transaction story and your finance in special menu.
Project was my learning project at SkillBox. In that project I used: OOP, arrays and work with data.

---

## Technology 

- OpenJDK24
- Library: Scanner
- IDE: IntelliJ IDEA 

---

## Feature
- Add income and expense transactions
- Display total balance, income, and expenses
- Show last 5 transactions
- Data stored in memory using an array
- Console-based navigation using Enums

---

## Project architecture
```
src/
└── java_string_and_dates/
├── Main.java 
│
├── model/
│ ├── Transaction.java 
│ └── TransactionType.java
│
└── services/
├── FinancialAccounting.java 
├── UserMenu.java 
└── UserOption.java
```
### Description
```
- Main.java                                                   # this is entery point
- model/Transaction.java                                      # record class for transaction object description
- model/TransactionType.java                                  # enum class for transaction type description
  - public static boolean checkTransactionType(String type)   # used to check the transaction type from the user
- services/FinancialAccounting.java                           # using for finance operations
  - public String toLowerUpperCase(String description)        # formating transaction description, do first letter Upper and rest to lower
  - public void addTransaction()                              # add transactions to array, if in array there are 5 transaction new transaction goes to 0 index
  - public void reportOption()                                # show income, expenses, balance and last 5 transactions
  - public void exitOption()                                  # show income, expenses, balance, last 5 transactions and exit from app
- services/UserMenu.java                                      # using for app navigation system
  - public static void selectMenuOption()                     # using for app navigation
  - public static void helpOptionMenu()                       # show app menu
- services/UserOption.java                                    # enum class for useer option description
  - public static UserOption checkUserOption(String option)   # used to check selected option
```
---

## How to Run

To run the project locally:

```
git clone https://github.com/mihaidaniel-it/TransactionSystem.git

cd java_string_and_dates

javac Main.java

java Main
```
---

## Future Improvements
-  Save/load transactions from a file (CSV or JSON)
- Add unit tests with JUnit

---


## Author

- **Developed:** Mihai Daniel
- **Email:** [mihaidaniel.it@gmail.com](mailto:mihaidaniel.it@gmail.com)
