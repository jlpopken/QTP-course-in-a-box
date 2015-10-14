---
title: Function Library
---

#Function Library

One cool thing about QTP is that you can create custom functions and then stored them in a function library so that all of your tests can call the custom functions stored in the function library. 

Example of a Function: 
 
function SumOfTwoNumbers(a,b)
Dim sum
sum=a+b
SumOfTwoNumbers=sum
End Function
 
Example Calling a Function:

result=SumOfTwoNumbers(x,y)
msgbox result


