---
title: Object Models
---

There are various Object Models that help VBScript interact with a certain group of objects. This can be exetremely useful in your test scripts.


#COM - Component Object Model

COM is used to help interact with Microsoft objects. COM  objects includes Microsoft technologies like: OLE, OLE Automation, ActiveX, COM+, DCOM, the Windows shell, DirectX, and Windows Runtime. COM helps us interact with Microsoft Objects like Word, Access, Excel, Outlook, Internet Explorer, and the Windows File System Object.

First we must create an instance of the object we want to use:

Here are some examples:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10581159/e05a3adc-7646-11e5-9c5e-a79825b82359.PNG "EXCEL")
![alt text](https://cloud.githubusercontent.com/assets/10998057/10380818/d9121a92-6ddb-11e5-8388-8ff1453ed118.PNG "WORD")

Once you have created the object you can always type the name and then a period (I.E. "myExcel.") and then the list of available methods will pop up.

![alt text](https://cloud.githubusercontent.com/assets/10998057/10581161/e05cb370-7646-11e5-96a3-ea5547da4ae0.PNG "Methods")

Here is an example of what you can do with the Excel object:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10581158/e054d3da-7646-11e5-810c-27e52e633eb4.PNG "Methods")

#WSH - Windows Script Host Object Model

![alt text](https://cloud.githubusercontent.com/assets/10998057/10581160/e05a411c-7646-11e5-97e6-5400a0f43c08.PNG "WSH")

You can use WSH to run applications, manipulate the contents of the registry, or send keyboard input.

Here is an example of using the WSH object model to send keyboard input:

![alt text](https://cloud.githubusercontent.com/assets/10998057/10581157/e048f2fe-7646-11e5-9377-3bca811df5dc.PNG "SendKeys")

#DOM - Document Object Model
You can use DOM to interact with objects in HTML, XHTML, and XML documents. So think web applications. 

#AOM - Automation Object Model

You can use AOM to load all the required add-ins for a test, make QTP visible while execution, opens the test using the specified location, associates function libraries, setting the common object sync time out, start and end iteration, enable/disable smart identification, on error settings, data table path, recovery scenario settings, and log tracking settings. So you can use AOM objects to help automate configurations for your test script. 


