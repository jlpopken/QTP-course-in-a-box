---
title: Transactions
---

#Transactions

You can use transactions to see how long a particular chunk of code takes to run in your test. Or if you run your test scripts with loadrunner then you can use transactions to break up your test into pieces so loadrunner can tell you what transaction the test failed on if it fails. 

To start a transaction, click on Insert -> Start Transaction. I'm going to add this before I log in. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10583639/b0719a10-7653-11e5-802a-8df4fac6fa07.png "Start")

Give it a name. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10583660/d7387c7c-7653-11e5-9159-8ef71b241336.PNG "Name")

Then find where you want to end your transaction. I'm going to end if after the login. Click on Insert -> End Transaction. 

The now my login is encased in a transaction named "Login."

![alt text](https://cloud.githubusercontent.com/assets/10998057/10583707/18a0a996-7654-11e5-9141-1360977597cf.PNG "Transaction")
