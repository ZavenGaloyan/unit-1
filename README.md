# Crypto Wallet

![](22ROOSE-master768.gif)  
<sub>Illustration for Glenn Harvey</sub>

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

## Proposed Solution

Design statement:
I will to design and make a electronic ledger for Ms. Sato. The digital crypto ledger will use ETH or ethernium crypto currency and is constructed using the software Python . It will take a few weeks to make and will be evaluated according to the criteria listed below.

Eth or etherium is a popular cryptocurrency in the modern crypto market. It is one of the leading technologies in Defi or decentralized finance. 
Its speed for transactions, Dis-inflationary supply, and scalability to various aspects in fiance and tech make it so wanted
https://ethereum.org/en/


Justify the tools/structure of your solution

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger will display past transactions within a given month and year
5. The electronic ledger will show a graph on the total balence in a the ledger for every month of the year.
6. The electronic ledger will have password to enter this 
## Record of Test Plan
| Description | test type                                                |                                                                                                 | Inputs | Outputs | |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| Login & Menu       | Unit test                                         |                         | Input correct password to login        | It will move the user to a the menu of options when the correct password is enters                 |          |
| Basic description of crypto currency       | Unit test                                         |                         | Input the number 1 in menu        |When number 1 is entered a basic description of the crypto currency is displayed                  |          |
| To enter, withdraw and record transactions       | Unit test                                         |                         | Input the number 2 in the menu then choose wheter to enter or withdraw a transaction by choosing 1 or 2        |Once 2 is selected a a menu for transactions pops up from which the user can choose to enter or withdraw a transation. Each of these options will present a date and amount which is then transfered to a csv file taht keeps the data                 |          |
| Display past transactions within a given month and year       | Unit test                                         |                         | Input the number 3 in menu       |The user will fill in the month and year from which they would like to see past transactions from. When these are entered, All the transactions within these parameters will be printed in the terminal                 |          |
| Display a graph on the total balence in a the ledger for every month of the year      | Unit test                                         |                         | Input the number 4 into the menu        |When the number 4 is entered into the menu a graph on the total balence in a the ledger for every month of the year will be printed in the terminal                |          |
| Password validation       | Usability test                                         |                         | Input correct password to login        |If the inputed password matches what is stored in the password.csv file. It will move the user to the menu of options: if the passoword is incorrect it will allow another antempt to login                  |          |
| Date validation       | Usability test                                         |                         | Input a date in a given format (month/day/year)        |This will check if the given values are eligable and if the month and days written math. For example if the 31 of Feb is written the terminal will explain the issue and allow for another attempt. Once the nessisary requirements are met.It will then proceeds to the next stage                  |          |
| Numerical validation       | Usability test                                         |                         | Input a integer with in a given range       |If a letter,symbol, or number that is not a posative integer is entered it will allow for antempts to be made until the nessisary requirements are met.It will then proceeds                 |          |
# Criteria B: Design

## System Diagram 
![](https://github.com/ZavenGaloyan/unit-1/blob/main/Untitled%20Diagram.jpg)
## Flow Diagrams:Password protection
![](https://github.com/ZavenGaloyan/unit-1/blob/main/PasswordFlowchart.jpg)
## Flow Diagrams:Numerical validation 
![](https://github.com/ZavenGaloyan/unit-1/blob/main/Transaction.jpg)
## Flow Diagrams:Past Transaction with Validation
![](https://github.com/ZavenGaloyan/unit-1/blob/main/Displaying_past_transactions.jpg)
## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Discuss with Ms Sato about the nessiray requirements                                         | To have a clear understanding of the clients needs                        | 15min         | Sep 24                 | A         |
| 2       | Create Success Criteria                                         | To have a clear idea of what is needed for to have a successful project                        | 30min         | Sep 25                 | A         |
| 3       | Code Login system to have it password protected                                         | To complete one of the criteria by having the digital ledger password protected                        | 45min         | Sep 28                 | C         |
| 4       | Code menu                                         | So the digital ledger has differant options Ms Sato can choose to do a function as she wishes                       | 1 hr         | Sep 30                 | C         |
| 5       | Code main functions                                         | To have all the nessisary functions to show every criteria given                      | 4 hr         | Oct 2                 | C         |
| 6       | Code the validations for functions                                         | To reduce the risk of errors and the digital ledger not functining properly.                        | 3 hr         | Oct  7                  | C         |
| 7       | Create a test plan                                         | To have a clear display of the nessisary tests needs to see the functionality and usability of the digital ledger                        | 30min         | Oct 8                  | B         |
| 8       |Make Systems diagram                                        | To show how the digital ledger was made and functions on the computer in the form of a system diagram                        | 10min         | Oct 8                 | B         |
| 9       | Creating Flow diagrams                                         | To show how certain functions in the code work in the form of a flow chart                       | 1 hr min         | Oct 9                  | B         |
| 10       | Record the using of Program                                         | To show how the digital ledger actully works                    | 15min         | Oct 9                  | B         |
                    
# Criteria C: Development
## Specific techniques used
Functions
For and while loops
Input Validation in various circumstances
If/else statements
Password encryption
List Comprehension
## Examples of when Techniques were used
```.py
#password validation
print("Login below to begin :)")

with open("Unit1_PROJECT_pass.csv") as file:
    stored_data = file.readlines()
    line1 = stored_data[0].split(":")
    password = line1[1]
    password = password.strip()


pass_stat = False
new_pass = input("Enter a password:")
while not pass_stat:
    if new_pass == password:
        pass_stat = True
    elif new_pass != password:
         new_pass = input("Incorrect password try again:")
```.py
##hello
 
