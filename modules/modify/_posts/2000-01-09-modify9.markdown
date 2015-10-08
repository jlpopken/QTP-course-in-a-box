---
title: Environment Variables
---

#Environment Variables

Environment Variables are special variables that can be used by all actions, function libraries and recovery Scenarios. So they are kind of like Window's environment variables except that QTP environment variables are only available to QTP while Window's environment variables are available to any application running on the system. 

There are built in environment variables (pre-defined) and there are user-defined ones. 

In QTP click on File -> Settings 0> Environment

![alt text](https://cloud.githubusercontent.com/assets/10998057/10380233/4d0cf740-6dd8-11e5-9a97-87243e9df958.png "LoginCode")

We are going to create two user defined environment variables. One will be named "Name" with a value of "jeanette" and one will be named "Password" with a value of "mercury"

![alt text](https://cloud.githubusercontent.com/assets/10998057/10380430/641339b2-6dd9-11e5-8514-c63a13f554c8.PNG "Variables")

Then in our test script, we will switch out the login credentials to read from our environment variables and not from our datatable. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10380499/c09b5e12-6dd9-11e5-9c62-7ee1dd0f7c5a.PNG "CodeSwitch")

You can even have user defined environment variables that are stored in a external file like an .xml and can be loaded into the test or can  be loaded dynamically as the test is running. 
