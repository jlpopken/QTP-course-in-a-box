---
title: Import/Export DataTables
---

#Import/Export DataTables

<iframe width="420" height="315" src="https://www.youtube.com/embed/HSkuRUSRjQg" frameborder="0" allowfullscreen></iframe>

We are going to learn how to put values that we will use in  our tests on a spreadsheet and then import that spreadsheet as the Global DataTable so that QTP can read in those values instead of using hardcoded values in the test script itself. 

Open up an excel spreadsheet.
First write the header for the column User and then put in the value
<br />
    Ex. Here you see a "USER" column with a value "jeanette" 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10349774/c0988a18-6d05-11e5-8459-856918c28747.PNG "User")

Now do the same for Password
    Ex. Here you see a "USER" column with a value "jeanette" and a "PASSWORD" column with a value "mercury"

![alt text](https://cloud.githubusercontent.com/assets/10998057/10349795/ddca614c-6d05-11e5-9a9a-5415e7f6a3c4.PNG "Password")

Save your spreadsheet so you can access it from your test script. (Note. If you are using QTP version 11 or before then you need to save it as an .xls file. If you are using UFT then you can save it with a newer format like .xlsx)

In your QTP test script, add the following line of code so that your test will import the spreadsheet as the global datatable. This means if you have several actions in your test then they all can access the global datatable.

![alt text](https://cloud.githubusercontent.com/assets/10998057/10349993/2c4dc7d6-6d07-11e5-8577-8af76de50b5a.PNG "DataTable")

At the end of your script add the following line to export the global datatable. I name it something different so it does not override the original. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10459115/b48dfcb6-7193-11e5-848d-b7d7da068073.PNG "Export")





