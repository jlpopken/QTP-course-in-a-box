---
title: Descriptive Programming
---

#Descriptive Programming

<iframe width="560" height="315" src="https://www.youtube.com/embed/IemykLK0xZw" frameborder="0" allowfullscreen></iframe>

So far we've relied heavily on the Object Repository. If our test tries to run using an object that does not exist in the Object Repository then our test fails. But this is not our only option, if we use descriptive programming to reference the object then the object does not need to be present in the Object Repository. 

So let's change the way we are clicking on the Insert Order button. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10459339/bee3557a-7194-11e5-97d6-ff4d44bdbc30.PNG "InsertOrderButton")

(You can even delete the Insert Order button out of the object repository if you want. We won't need it anymore.)

So let's click on the object spy and then the pointer and then click on the Insert Order Button. 
We want to find a unique property/value pair:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10459340/bee3f12e-7194-11e5-875c-18a026371885.PNG "PropertyValuePair")

Ok. We'll use the property value pair text and &InsertOrder.

So instead of using the object's name from the object hierarchy (i.e. WinButton("Insert Order").Click) we will use a property/value pair instead. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10459341/bee3fd36-7194-11e5-8949-6e620683e457.PNG "DesriptivePrograming")

You can actually use multiple property/value pairs if you run into a situation where one pair isn't unique enough. 
