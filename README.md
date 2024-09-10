# Customer Banking Application

## Overview

This project implements an account management system with Savings and CD (Certificate of Deposit) accounts. It provides functionality to calculate interest, update account balances, and display the results to users based on their inputs.

The project consists of four key files:
1. **Account.py** - Defines the `Account` class with methods to set the balance and interest.
2. **savings_account.py** - Contains the `create_savings_account` function to calculate interest and update the balance for savings accounts.
3. **cd_account.py** - Contains the `create_cd_account` function to calculate interest and update the balance for CD accounts.
4. **customer_banking.py** - The main program file that interacts with the user, gathers inputs, and displays results for both account types.

## Files

### 1. `Account.py`
This file contains the `Account` class, which is used by both savings and CD accounts. The class has the following methods:
- `set_balance(balance)`: Sets the balance for the account.
- `set_interest(interest)`: Sets the interest earned for the account.

### 2. `savings_account.py`
This file defines the `create_savings_account` function, which:
- Takes in the initial balance, annual interest rate (APR), and number of months.
- Calculates the interest earned and updates the balance.
- Returns the updated balance and interest earned.

### 3. `cd_account.py`
This file defines the `create_cd_account` function, which:
- Takes in the initial balance, annual interest rate (APR), and number of months.
- Calculates the interest earned and updates the balance.
- Returns the updated balance and interest earned.

### 4. `customer_banking.py`
This file serves as the main entry point of the program. It:
- Prompts the user for savings and CD account details.
- Calls the appropriate functions (`create_savings_account` and `create_cd_account`) to process the input.
- Displays the updated balances and interest earned for both account types, formatted to two decimal places.

## How to Run the Program

1. Ensure all files are in the same directory.
2. Run the program by executing `customer_banking.py`:
    `python customer_banking.py`
3. The program will prompt you for the following inputs for both savings and CD accounts:
    - Initial balance
    - Annual interest rate (APR)
    - Number of months

4. The program will then calculate the interest earned and display the updated balances for both accounts.

## Example Output

```text
Enter the savings account balance: 1000
Enter the savings interest rate (APR): 5
Enter the number of months for the savings account: 12
Savings Account: Interest earned: $50.00, Updated balance: $1,050.00

Enter the CD account balance: 2000
Enter the CD interest rate (APR): 4
Enter the number of months for the CD account: 12
CD Account: Interest earned: $80.00, Updated balance: $2,080.00
