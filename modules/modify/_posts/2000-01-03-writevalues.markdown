---
title: Write values to a spreadsheet
---

#Write values to a spreadsheet

<iframe width="560" height="315" src="https://www.youtube.com/embed/FTVLNOqgF74" frameborder="0" allowfullscreen></iframe>

Now let's open up the Flight application. Let's say that we want to read in values at runtime and write them to our global spreadsheet that gets exported. For this exercise we will add some code that will capture the price of the order. 

First, we need to add a header to our spreadsheet but we won't be putting in any values, our script will do that. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10351235/0162c826-6d0e-11e5-8e42-9bf5e2576eb3.PNG "Price")

Then we will use the object spy to point to the element we want to capture the value during runtime. In this case, I selected the first box that is titled "price." 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10351229/f79cd03e-6d0d-11e5-9bb7-adc5cdb799c5.PNG "PriceBox")

First we find the Properties/Values pair that has the information we want. It looks like we want the "text" property because it has the value "$369.60" Then we switch from the properties tab to the operations tab to find the method we will be using.

The Properties/Values pair:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10351326/8c271ebc-6d0e-11e5-9347-dc136ec29558.PNG "Pair")

For the method, we are going to choose the GetROProperty because RO means RunTime. So this is saying get the value of the property you pass this method (we are going to be passing "text") at the run time of the script. 

![alt text](https://cloud.githubusercontent.com/assets/10998057/10351336/9b368618-6d0e-11e5-96c3-0529177d5d6e.PNG "Method")

Also note the Nested hierarchy of windows that the object spy shows us:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10351574/cf728d0e-6d0f-11e5-99c8-b17f2ed09c84.PNG "hierarchy")

Referring to the nested hierarchy at the top of object spy's results, we will add this line:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10367884/736f5558-6d98-11e5-9037-5b09e720c9c9.PNG "NewCode")

This line of code is writing the captured value of price (as the script is running) to our column on the global datatable called "PRICE." This then gets exported at the end with our global datatable. 

After we re-play our script, the exported spreadsheet looks like this:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10352060/7f86c2b2-6d12-11e5-8b94-5ca66e0432cb.PNG "Exported")




