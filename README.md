# vityarthi-project
vidyarthi project - banking system

 Project Overview
This project is a console-based Banking System in Python that allows a user to:
Create an in-memory bank account.​
Deposit money into the account.​
Withdraw money with basic validation (no negative or over-balance withdrawal).​
Check current balance through a simple text menu.​
It is designed as a small Object-Oriented Programming (OOP) project suitable for a college assignment.​

2. System Requirements and Setup
2.1 Software Requirements
Python 3.x (any recent version like 3.8+).​
Any text editor or IDE such as VS Code, PyCharm, or IDLE.​
Operating system: Windows, macOS, or Linux that supports Python 3.​

2.2 Installation Steps
Install Python 3 from the official Python website and make sure “Add Python to PATH” is selected during installation.​
Open your editor/IDE and create a new file named bank_system.py.​
Copy the Python code (from the previous answer) into bank_system.py and save the file.​
Open a terminal/command prompt in the folder where bank_system.py is saved.​
Run the program using:
python bank_system.py (or py bank_system.py on some Windows setups).​

3. Code Structure and Explanation
3.1 BankAccount Class
The project uses a BankAccount class to represent a single bank account.​
Key attributes:
account_holder: Stores the name of the account holder as a string.​
balance: Stores the current account balance as a float, default 0.0.​

Key methods:
__init__(self, account_holder, balance=0.0):
Constructor that initializes a new BankAccount object with the holder’s name and an optional starting balance.​
deposit(self, amount):
Validates that amount is positive.
Adds the amount to self.balance.
Prints confirmation and the new balance.​
withdraw(self, amount):
Validates that amount is positive.
Checks whether amount is less than or equal to self.balance.
If there is enough balance, subtracts the amount and prints the new balance; otherwise shows “Insufficient balance.”​
check_balance(self):
Prints the current balance to the user.​
This design follows basic OOP by grouping data (balance, holder name) and behavior (deposit, withdraw, check) into one class.​

3.2 main() Function and Program Flow
The main() function controls user interaction and the menu loop.​

Steps:
Display a welcome message for the banking system.​
Ask the user to enter the account holder’s name and create a BankAccount object.​
Show a menu inside an infinite loop:
Option 1: Deposit Money
Option 2: Withdraw Money
Option 3: Check Balance
Option 4: Exit the program
​

Read menu choice as a string. Depending on the choice:
"1": Ask for deposit amount, convert to float, call account.deposit(amount).​
"2": Ask for withdrawal amount, convert to float, call account.withdraw(amount).​
"3": Call account.check_balance() to display current balance.​
"4": Print a thank-you message and break the loop to end the program.​

Any other input: Print an “Invalid choice” message.​
The if __name__ == "__main__": main() block ensures that main() runs only when the file is executed directly, which is standard Python project structure.​

4. How to Run and Test
Start the program from the terminal or your IDE.​
Enter a sample name (e.g., “Rahul”) when asked for the account holder name.​
Use the menu:
First choose Deposit and add any positive amount (for example 1000).​
Then choose Check Balance to verify that the balance updated correctly.​
Try Withdraw with an amount less than the balance (e.g., 500) and confirm that balance decreases.​
Try Withdraw with an amount greater than the balance to see the “Insufficient balance” validation.​

Finally, select Exit to close the application.
