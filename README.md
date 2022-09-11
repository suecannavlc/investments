# investments
Investments and taxes tracking

The goal of this project is keeping track of my stock investments, analyze the companies data and ease the process of reporting taxes.

High Level Requirements:
- Display all of my investments in an appropriate GUI
- Retrieve information regarding the companies in real time, or with a polling interval
- Keep track of all stock movements, such as buying, selling, receiving RSU, etc. 
- Calculate taxes automatically
- Keep track of all my finances, including deposits, cash, etc.

ARCHITECTURE

SHARES
All data can be thought as events in a table. These events contain all
needed information:
- date
- operation type (buy, sell, dividend, ...)
- broker
- value
- description
- currency
- currency exchange value
- number of shares

DEPOSITS
Similar to shares, but there are no number of shares

CASH
No number of shares, no broker/bank

BANK ACCOUNTS
Very similar to deposits, may even have interest rate. However, we need to
add new operations, as payments, withdrawals, ...

--------
From all the data before, I want to be able to extract different calculations,
do simulations, print reports and even generate a GUI.