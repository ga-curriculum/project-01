# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Banking With Python

![gif](https://media2.giphy.com/media/y3B74VeWI2QQE/giphy.gif)

| Language | Type      | Date       | Due        | Author               |
|----------|-----------|------------|------------|----------------------|
| Python   | Project 1 | XX/XX/XXXX | XX/XX/XXXX | Suresh Melvin Sigera |

## Prompt

ACME Bank uses a file structure called `bank.csv`. The cashiers will use this brand-new software to manage transactions, and you have been tasked with developing it.

```text
10001;suresh;sigera;juagw362;1000,10000
10002;james;taylor;idh36%@#FGd;10000,10000
10003;melvin;gordon;uYWE732g4ga1;2000,20000
10004;stacey;abrams;DEU8_qw3y72$;2000,20000
10005;jake;paul;d^dg23g)@;100000,100000
```

| account_id | frst_name | last_name | password    | balance_checking | balance_savings |
|------------|-----------|-----------|-------------|------------------|-----------------|
| 10001      | suresh    | sigera    | juagw362    | 1000             | 10000           | 
| 10002      | james     | taylor    | idh36%@#FGd | 10000            | 10000           |
| ...        | ...       | ...       | ...         | ...              | ...             |

Given the above file structure for the ACME Bank, write the entire Python program using classes, methods, file handling,
and exception handling to meet the functional requirements below:

## Requirements

You should have **a minimum of**:

* 4 classes;
* 1 file (`bank.csv` given to you);
* You're allowed to add more classes base on the OOP design
* The entire project should be carried out using a **test-driven development (TDD)** approach

### Your app should have the following functionality:

1. Add New Customer
    * customer can have a checking account
    * customer can have a savings account
    * customer can have both a checking and a savings account

2. Withdraw Money from Account (required login)
    * withdraw from savings
    * withdraw from checking
3. Deposit Money into Account (required login)
    * can deposit into savings
    * can deposit into checking
4. Transfer Money Between Accounts (required login)
    * can transfer from savings to checking
    * can transfer from checking to savings
    * can transfer from checking or savings to another customer's account

5. Build Overdraft Protection
    * charge customer ACME overdraft protection fee of $35 when overdraft
    * prevent customer from withdrawing more than $100 USD if account is currently negative
        * _the account cannot have a resulting balance of less than -$100_
          OR
        * _the customer cannot make a withdrawal of greater than $100_
    * deactivate the account after 2 overdrafts
        * reactivate the account if the customer brings the account current, paying both the overdraft amount and the
          resulting overdraft fees
          
### (Bonus)

- Display Transaction Data (You need to create another file to store the transaction history, required login)
  - index all transactions for a customer account
  - show one transaction details
  - show historical data of transactions (date and time of transaction, type of transaction, resulting balance, etc.)

### Planning requirements

As you've discovered, a project consists of more than just code.

This project requires planning organized within the **GitHub projects** with the following lists:

- **Icebox**: Holds user stories that have yet to be moved to the Current/MVP list. All user stories are originally put into
  the Icebox, including both MVP and wish list stories.
- **Current/MVP**: Holds user stories that must be completed to meet the minimum project requirements (MVP). Once the MVP
  has been met, additional user stories may be moved to this list from the Icebox.
- **Completed**: Holds completed user stories.

Important: User stories need to be formed properly using this template: 
```
    As a <role>, I want <feature> so that <reason>.
```

As an example : 

```
- As a user, I want to open a checking account so that I can deposit money into my checking
- As a user, I want to open a savings account so that I can deposit money into my savings
- As a user, I want to open both a savings and checking account

```


### Version control requirements

- The project's source code must be hosted on a GHE account.
- The repo is to contain **frequent commits dated from the beginning of the project through its completion**.
- Do not **start over** by _replacing the repository_ with a different one.
- Overall project must have at least **60 commits**

### Self-sufficiency / Project assistance

- At this stage being able to find the answers to development issues is of paramount importance.
- Use all resources available to solve the issue on your own before seeking assistance.
- If you do seek assistance in Slack, use the support channel and explain the issue as clearly and detailed as you can,
  include screenshots when possible, and be prepared to explain what you've done to solve the issue on your own.

## Get started!

![gif](https://media.giphy.com/media/ADgfsbHcS62Jy/giphy.gif)

## Additional resources:

- [Pretty-print tabular data in Python, a library and a command-line utility](https://pypi.org/project/tabulate/)
- [Command line colors](https://pypi.org/project/termcolor/)
- [Command line menu](https://pypi.org/project/simple-term-menu/)
