Bank Management System
Overview
The Bank Management System is a Java-based console application designed to manage bank accounts, transactions, and administrative tasks. It provides a secure and efficient platform for bank administrators and managers to handle customer accounts, perform financial operations, and maintain system security. The system is built using Object-Oriented Programming (OOP) principles, ensuring modularity, scalability, and maintainability.

Author: Muhammad Sami Choudhary
Version: 1.0.0
Date: June 16, 2025
License: Copyright © 2025 Muhammad Sami Choudhary. All Rights Reserved.

Features
Admin Features

Account Management:

Add Account: Create new saving or current accounts with details like CNIC, name, father's name, phone, email, address, and initial balance.
Deactivate/Activate Account: Toggle account status to active or inactive.
Edit Account Details: Modify account information such as CNIC, name, email, phone, address, or status.
Find Account: Search for an account using CNIC and display its details.
Show All Accounts: List all accounts with their details.


Transaction Management:

Deposit Cash: Deposit money into an active account.
Withdraw Cash: Withdraw money from an active account, respecting account-specific rules (e.g., overdraft for current accounts).
Transfer Money: Transfer funds between accounts, ensuring valid sender and receiver accounts.


Interest Calculation:

Calculate and apply interest for saving accounts based on the specified interest rate and time period.


Secure Login:

Admin login with ID, username, and password. The system locks after three failed attempts, requiring manager intervention to unlock.



Bank Manager Features

Admin Management:

Add Admin: Create new admin accounts with unique IDs, usernames, and passwords.
Edit Admin Settings: Update admin usernames or passwords.
View All Admins: Display a list of all admin accounts.
Find Admin: Search for an admin by ID.
Unlock Admin Panel: Reset failed login attempts to unlock an admin account.


Manager Settings:

Change Manager Password: Update the manager's password after successful login.


Secure Login:

Manager login with ID, username, and password, ensuring secure access to administrative functions.



Account Types

Saving Account: Supports interest calculation and restricts withdrawals to available balance.
Current Account: Allows overdraft up to a specified limit for withdrawals.

Project Structure
bankmanagementsystem/
├── Account.java            # Abstract base class for accounts
├── Admin.java              # Admin class for managing accounts and transactions
├── BankManager.java        # Bank Manager class for admin management
├── CurrentAccount.java     # Current account class with overdraft functionality
├── SavingAccount.java      # Saving account class with interest calculation
├── BankManagementSystem.java # Main class with application entry point
└── README.md               # Project documentation

Installation

Prerequisites:

Java Development Kit (JDK) 8 or higher
A Java IDE (e.g., IntelliJ IDEA, Eclipse) or a text editor with command-line compilation


Steps:

Clone the repository:git clone https://github.com/sami786chakwal/Bank-Management-System-Java.git


Navigate to the project directory:cd bank-management-system


Compile the Java files:javac bankmanagementsystem/*.java


Run the application:java bankmanagementsystem.BankManagementSystem





Usage

Launch the application to access the main menu.
Choose between Admin (option 1) or Bank Manager (option 2) roles, or exit (option 0).
For Admin:
Log in with default credentials (ID: 123, Username: admin, Password: admin).
Access features like adding accounts, depositing/withdrawing cash, transferring money, or calculating interest.


For Bank Manager:
Log in with default credentials (ID: 123, Username: manager, Password: manager).
Manage admin accounts, unlock admin panels, or change the manager's password.


Follow the console prompts to interact with the system.

Security Features

Login Security: Both admin and manager accounts require ID, username, and password. Admin accounts lock after three failed login attempts.
Input Validation: The system handles invalid inputs (e.g., non-numeric CNIC, negative amounts) with appropriate error messages.
Account Uniqueness: Prevents duplicate accounts by checking CNIC during account creation.

Limitations

The system supports a maximum of 5 accounts and 5 admins due to fixed array sizes.
No persistent storage; data is reset when the application closes.
The commented DeleteAdmin method is not implemented in the main application.

Future Improvements

Implement persistent storage using a database (e.g., MySQL, SQLite).
Replace fixed-size arrays with dynamic data structures (e.g., ArrayList).
Add a graphical user interface (GUI) using JavaFX or Swing.
Enable admin deletion functionality.
Introduce transaction history and audit logs.

Contributing
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request. Ensure your code follows the existing structure and includes appropriate comments.
Contact
For questions or feedback, contact Muhammad Sami Choudhary at sami.mirza@gmail.com.
License
Copyright © 2025 Muhammad Sami Choudhary. All rights reserved.
