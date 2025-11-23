# vityarthi-project
vidyarthi project - banking system
Main idea
A BankAccount class is created to represent one bank account.
The program then creates one object of this class and repeatedly asks the user what they want to do (deposit, withdraw, check balance, or exit).​​
What the class does
The class stores two main things: the account holder’s name and the current balance.​
deposit(amount) adds a positive amount to the balance and shows the new balance.
withdraw(amount) subtracts money only if the amount is positive and not more than the current balance; otherwise it shows an error message.
check_balance() simply prints the current balance.​

How the program runs
In main(), the program asks for the user’s name and creates a BankAccount object with balance 0.​
Then it shows a looped menu:
1 → deposit
2 → withdraw
3 → check balance
4 → exit

Based on the choice, it calls the corresponding method on the same BankAccount object. The loop continues until the user chooses exit.
