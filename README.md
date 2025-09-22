# Banking Database System

This project defines a relational database schema for a banking system using SQL.  
It covers banks, branches, accounts, loans, and clients.

---

## Tables Overview

1. **BANK**
   - Stores bank information.
   - Columns: `bank_ID`, `bank_name`, `bank_address`

2. **BRANCH**
   - Each bank can have multiple branches.
   - Columns: `branch_ID`, `branch_name`, `branch_address`, `bank_ID (FK)`

3. **ACCOUNT**
   - Holds customer accounts linked to branches.
   - Columns: `account_ID`, `branch_ID (FK)`, `name`, `account_type`

4. **LOAN**
   - Tracks loans given to account holders.
   - Columns: `loan_ID`, `account_ID (FK)`, `name`, `loan_type`, `loan_amount`

5. **CLIENT**
   - Stores client details linked to accounts.
   - Columns: `client_ID`, `account_ID (FK)`, `name`, `client_address`

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Cbaesparta/bank-database.git
   cd bank-database
