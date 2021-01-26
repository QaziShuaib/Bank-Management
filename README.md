# Draft for Bank-Management software
                              
  ## Welcome Screen
  
1.	Add new account
2.	Login to existing account
on Display, after login: showing name, acc no, address, phone no

        a)	Edit info: change name, address, phone

        b)	Deposit money

        c)	Withdraw money

        d)	Check balance

        e)	Check fixed deposits

        f)	Make a Fixed Deposit.

        g)	Request account closing

        h)	exit

3.	Administrator check up: 

        a) check account closing requests 

        b) show ALL the info stored

4.	Help

5.	About

6.	exit

                                                     
  ## Functions

1.	Welcome_Screen () which will display above functions as a list and take corresponding number as choice.
2.	Interest (int principal, int rate, int time)
3.	new_acc(): first, it outputs the name of needed docs and an amount of 1000 INR as security charges, 1000 INR for debit card, passbook, cheque book, and an optional 1000 INR for General Insurance. Then, it takes input from user for the following:- name, age address, DOB, sex, phone number, total amount to be submitted including fees, nominee name, nominee acc no. At last, it should ask user to create a password. Then, it should ask for a security question, for this, display 5 questions and then ask user to enter customised answer of anyone question. After successful creation of account, it should allot an acc number and it should save all the information in a file.
4.	login(): it should ask the user to enter acc number and then password. If correct password is entered, it should pass the control to main. If false password is entered, then it should display two choices 1. Re-enter password for this account. 2. Forgot password. Use goto for 1 and if prompted for second, then display security question and ask answer from user, if answer is correct then, allow user to enter a new password. Update the password in directory., then again take the control to login()
5.	  login_welcome(): displays name, acc no, phone number, address of phone number after logging in.
6.	Edit(): edits personal info of user, like address, name, phone. Presents all of the options as a switch case and ask user’s choice. Allow user to re-enter any entry and then update that in directory
7.	del_bal(int m, int *user_balance_amount): deletes m INR from user’s  balance amount.
8.	Add_bal(int m, int *user_balance_amount)
9.	Deposit(): Ask user for the amount to be deposited, update in directory after entering amount. Use add_bal(). Call check_balance() function to display updated balance.
10.	Withdraw(): Ask amount to be withdrawn, update in directory after entering amount. Use del_bal(). Call check_balance() function to display updated balance.
11.	Check balance(): prints balance after calculating proper interest. Use interest()
12.	Fd(): enter amount to create an fd. call del_bal() to lessen the balance amount of user. 
13.	Check_fd(): shows existing fds of customer
14.	req_acc_closing(): writes acc no and name of customer in a file called close_requests
15.	admin(): asks the following: accounts closing  request, show directory.
16.	Close_requests: asks for: print requests, Execute request.
17.	Delete_acc(): a sub function of admin. Deletes account.
18.	print_dir(): prints whole file directory in proper format
19.	Help(): prints the functioning of all the external functions in good English
20.	About(): prints the readme type of file but in a brief manner.
