---
title: Checkpoints
---

#Checkpoints

Checkpoints are a validation point that is used to compare the current value of specified properties with the expected value. It's a good way to double check that your script is getting or doing the right thing. 

There are several different kinds of checkpoints:
-----------------------------------------------------------
-Standard Checkpoint (Objects)

-Bitmap Checkpoint

-File Content Checkpoint

-Table Checkpoint

-Text Checkpoint

-Text Area Checkpoint

-Accessibility Checkpoint

-Page Checkpoint

-Database Checkpoint

-XML Checkpoint

For our example we are going to use a standard checkpoint which just checks the current object's propterty/value pairs with the expected property/value pairs. We are going to use our checkpoint to make sure that after we log in that the Flight application window opens. So log into Flight, click Record on QTP and then click on Insert -> Checkpoint -> Standard Object.

![alt text](https://cloud.githubusercontent.com/assets/10998057/10372617/446b1fa6-6dae-11e5-9817-76ed7c72c64b.png "InsertCheckpoint")

Once you do that, your mouse will be a pointer so that whatever you next click on will be the object it chooses for the checkpoint. I clicked on the Flight Reservation Window.

Make sure if got the element you wanted and then click ok.

![alt text](https://cloud.githubusercontent.com/assets/10998057/10376499/c29c6082-6dc3-11e5-99b2-6e6ac9b3467d.PNG "Selection")

This then shows you the captured property/value pairs it will use as the expected values that it will compare against runtime values. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10376498/c297cf2c-6dc3-11e5-93fa-155331b42790.PNG "Properties")

This then shows you the captured property/value pairs it will use as the expected values that it will compare against runtime values. 

QTP will then generate a line of code to your test script:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10376524/e4fc1320-6dc3-11e5-83e2-7c1f666fd769.PNG "Checkpoint")

Now when your test script runs it will check to make sure the Flight Window is there. If for some reason, the login fails and the Flight Window does not open up then your script will error our when it hits the checkpoint. 






