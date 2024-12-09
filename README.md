Overview of the Banking Application 
This Java application simulates a simple banking system where users can create bank accounts, deposit and withdraw money, and check their account balances. 
The application is organized into four main parts, each represented by a class. 
1. Transaction Class Purpose: This class keeps track of individual transactions (money movements). 
   Key Features:
     Type: Indicates whether the transaction is a deposit (adding money) or a withdrawal (taking money out).
     Amount: The amount of money involved in the transaction.
     Date: The date when the transaction took place.
   Functionality: It has a method that formats the transaction details into a readable string, making it easy to display.
 2. Account Class Purpose: This class represents a bank account.
     Key Features:
       Account Number: A unique identifier for the account.
       Account Holder Name: The name of the person who owns the account.
       Balance: The current amount of money in the account.
       Transactions: A list that records all deposits and withdrawals made from the account.
     Functionality:
       Deposit Method: Allows users to add money to their account. It checks if the amount is positive before adding it.
       Withdraw Method: Allows users to take money out of their account. It checks if there are enough funds before allowing the withdrawal.
       Get Balance Method: Returns the current balance of the account.
       Get Transaction History Method: Returns a list of all transactions for that account.
3. Bank Class Purpose: This class manages multiple bank accounts.
     Key Features:
       Accounts Map: A collection that stores all accounts, using the account number as the key to find each account easily.
     Functionality:
       Create Account Method: Allows users to create a new account if the account number doesn’t already exist.
       Get Account Method: Retrieves an account based on the account number.
       List Accounts Method: Displays all accounts along with their details, such as account number, holder name, and balance.
4. BankAppl Class Purpose: This is where the program starts running.
    Functionality:
    It creates an instance of the Bank class to manage accounts.
    It uses a loop to display a menu to the user, allowing them to choose actions like creating an account, depositing money, withdrawing money, or checking their balance.
    The program continues to run until the user decides to exit.
How It All Works Together
 User Interaction: When the program runs, it shows a menu to the user. The user can select options to perform different banking operations.
 Creating Accounts: Users can create accounts by providing a unique account number and their name.
 Depositing and Withdrawing: Users can add money to their accounts or take money out, with checks in place to ensure they can only withdraw what they have.
 Viewing Balances and Transactions: Users can check their current balance and see a history of their transactions.
