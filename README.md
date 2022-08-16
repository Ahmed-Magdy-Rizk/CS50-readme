# Online Banking System
#### Video Demo:  <[URL HERE](https://www.youtube.com/watch?v=-NuLW24IjDU)>
#### Description:

My project is a web-based application using Flask. My web application is a simulation of an online banking system.

#### Project Files

##### 1-static
- the app image
- the css file


##### 2-templates
1- layout.html (the main templates, it contains the App logo, navigation var, logout and the footer)

2- register.html (you shoud type in your name, email and password to make a new account)

3- index.html (contains account name, account number (only six-digit number), account email, total input cash into the account (wether you deposit or other user transfered it from their account), total output cash from the account (wether you withdraw it or you transfered it to other account), and you total balance

4- deposit.html (it allows you to deposit money to your account)

5- withdrawl.html (it allows you to withdraw money from your account)

6- transfer.html (it allows you to transfer moeny to other account if you know the other account number)

7- report.html (it displays your bank statement)

8- change_email (it allows you to change your default email)

9- change_password (it allows you to change your password)

10- apology (this is the failure template to demonstrate to the user what exactly they did wrong)

11- login (you should to type in your name and your password to loging)


##### 3- helpers.py
- the implementation of apology. ity renders a template, apology.html. It also happens to define within itself another function, escape, that it simply uses to replace special characters in apologies. By defining escape inside of apology, we’ve scoped the former to the latter alone; no other functions will be able (or need) to call it.
- usd function, a short function that simply formats a float as USD (e.g., 10000 is formatted as $10,000.00).

##### 4-clints.db
- this data base contains two tables, first users and the second is ledger

##### 5-app.py
- all the code in this file

##### 6- requirements.txt

- That file simply prescribes the packages on which this app will depend.

#### Requirements:

1- cs50

2- Flask

3- Flask-Session

4- flask-mail <(pip install --user flask-mail)>

5- requests

6- werkzeug <(Werkzeug is a comprehensive WSGI web application library)>



##### [eatures:

- Register for a new account. You type in your name, e-mail, and password. Once you register, it will send a confirmation email via email.

- Deposit money into your account.

- Withdraw money from your account.

- Transfer money to another account using their account number.

- Display a bank statement including Transaction Date&Time, Transaction type(Deposit, Withdrawl, Transfer from/to another account), amount of money for every transaction, and your balance after every transaction.

- Change your e-mail.

- Change your password.

#### Saftey Standars

- All the passwords are encrypted in the database by werkzeug hash generator

- All the user data verification is done on the server-side

- The App won't allow you to withdraw more money than you have in your account.

- The App won't allow you to transfer more money than you have in your account.

- You can't change your e-mail until you type in your password.

- You can't change your password unless you type in your old password.
