# Bank tech test

### Starting up the application

1. Install node and type `node` into the command line
2. Once in node REPL. Type `Bank = require('../lib/bank')`
3. Next, type `bank = new Bank()`

### Interacting with this application

* Type `bank.deposit(amount)` to deposit funds
* Type `bank.withdraw(amount)` to withdraw funds
* Type `bank.showStatement()` to see a list of all transactions

`amount` can only be an interger value 

### Requirements

* You should be able to interact with your code via a REPL like IRB or the JavaScript console.  (You don't need to implement a command line interface that takes input from STDIN.)
* Deposits, withdrawal.
* Account statement (date, amount, balance) printing.
* Data can be kept in memory (it doesn't need to be stored to a database or anything).

### User stories 

```
As a user

I would like to deposit money into my bank account
  
I would like to withdraw money from my bank account

I would like a bank statement with a history of all transactions

I would like the bank statement to include the date, amount and final account balance of each transaction

```

### Acceptance criteria

**Given** a client makes a deposit of 1000 on 10-01-2012  
**And** a deposit of 2000 on 13-01-2012  
**And** a withdrawal of 500 on 14-01-2012  
**When** she prints her bank statement  
**Then** she would see

```
date || credit || debit || balance
14/01/2012 || || 500.00 || 2500.00
13/01/2012 || 2000.00 || || 3000.00
10/01/2012 || 1000.00 || || 1000.00
```

