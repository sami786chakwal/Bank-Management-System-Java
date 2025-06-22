# Bank Management System  

A Java console application for secure banking operations with admin and manager roles.  

## Features  

### Admin Features  
- **Account Management**: Create/edit saving/current accounts  
- **Transactions**: Deposit/withdraw/transfer funds  
- **Interest Calculation**: For saving accounts  
- **Security**: 3-attempt login limit  

### Manager Features  
- **Admin Management**: Add/edit admins  
- **System Control**: Unlock admin accounts  
- **Security**: Change manager password  

## Account Types  

| Feature         | Saving Account | Current Account |  
|----------------|----------------|-----------------|  
| Interest       | ✅ Yes         | ❌ No           |  
| Overdraft      | ❌ No          | ✅ Yes          |  

## Installation  

1. Clone the repo:  
```bash  
git clone https://github.com/sami786chakwal/Bank-Management-System-Java.git  
cd Bank-Management-System-Java
```
2.Compile and run:
```bash
javac bankmanagementsystem/*.java  
java bankmanagementsystem.BankManagementSystem
```
3.Usage
Default Logins:

Admin: ID 123, User: admin, Pass: admin

Manager: ID 123, User: manager, Pass: manager
```bash
Project Structure
bankmanagementsystem/  
├── Account.java            # Base account class  
├── Admin.java              # Admin operations  
├── BankManager.java        # Manager functions  
├── CurrentAccount.java     # Current accounts  
├── SavingAccount.java      # Saving accounts  
└── BankManagementSystem.java # Main app
```
4.Security
Secure login system

Input validation

Account locking

⚠️ Note: Data resets when program closes (max 5 accounts/admins).

5.Future Plans
Database integration

Transaction history

GUI implementation

© 2025 Muhammad Sami Choudhary
📧 Contact: samichakwal45@gmail.com
