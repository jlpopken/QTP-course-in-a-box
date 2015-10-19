---
title: Recovery Scenarios
---

#Recovery Scenarios

Your test scripts will sometimes run into unexpected problems or errors as you run them. We will use recovery scenarios so that our scripts can "recover" from these errors and continue running the script. 

Click on Resources -> Recovery Scenario Manager

![alt text](https://cloud.githubusercontent.com/assets/10998057/10376800/7ba97352-6dc5-11e5-8579-acb23a4b4f03.png "RecoveryManager")

Click on the new recovery scenario button

![alt text](https://cloud.githubusercontent.com/assets/10998057/10376839/b8536a1a-6dc5-11e5-8529-a8223a098bd9.PNG "RecoveryManagerNew")

This opens up the recovery scenario wizard:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10376887/f5c6137a-6dc5-11e5-8400-e2683473c116.PNG "RecoveryManagerNew")

For this example, we will be putting in yesterday's date and this will cause a pop-up window stating that this is an incorrect date. So we want to select the pop-up window event at our trigger. 


![alt text](https://cloud.githubusercontent.com/assets/10998057/10376972/4eabcf7a-6dc6-11e5-8e4b-0fc334c0ed4e.PNG "RecoveryManagerNew")

Then QTP gives us the option to point to the pop-up window. Click on the pointer and then click on the pop-up window that appears when you enter yesterday's date.

This is the pointer button:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379777/c8bb1f64-6dd5-11e5-8068-21aee0645eee.PNG "Pointer")

This is the initial information that it grabbed when I pointed to the pop-up window:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379776/c8b61320-6dd5-11e5-94cd-93dc73473c6c.PNG "PointerInfo")

But I changed it to be a regular expression so that is would work with any date no just 10/08/15. Regular expressions are great fun and can be very helpful. (See resources for more info about them) 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379775/c8b59954-6dd5-11e5-857e-7a03ac9658bf.PNG "PointerInfo")

Then we need to give our scenario some steps to help recover and continue. First we will need to hit Enter on the keyboard so the pop-up goes away. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379778/c8bbaa6a-6dd5-11e5-8314-ab1259539d35.PNG "Enter")

Then we need this to erase out the bad date and enter in a good date. So I created a function which we will select. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379769/c8a99c08-6dd5-11e5-8b60-e5b1a173e110.PNG "Function")

This is what the code from my function looks like:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379771/c8aa8e88-6dd5-11e5-807f-ce9005c41241.PNG "Code")

For the Post-Recovery, I will select "Re-run current step" because we fixed the date so we can re-run the step without any problems now. 

Then give it a name and a description. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379770/c8a9ce26-6dd5-11e5-972d-eb02326a00a0.PNG "Scenario")

I choose to add it to this script. And now it's part of our test. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10379774/c8ae7f02-6dd5-11e5-9c15-f5226d88c46e.PNG "Scenario")

###Exercise
Change one of the dates on your spreadsheet to a date before today's date. Then run your test sript. Does your test hit the recovery scenario? Instead of deleting the bad date and entering a new date, what else could you try to recover from this error?






