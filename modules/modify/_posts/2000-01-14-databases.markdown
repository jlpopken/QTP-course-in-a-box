---
title: Databases
---

#Databases

You can use QTP to interact with databases using ADODB or the Active X Database Object model. This way you can interact with SQLServer, MySQL, Oracle, Excel, Access, and Sybase.

There are four methods that we need to use when interacting with databases:

ADODB.Connection - Connects you to a database

ADODB.Command - Executes  SQL commands, queries, or stored procedures

ADODB.Fields - get a specific column from a record set after executing a query or stored procedure

ADODB.Recordset - get data from a database

You will want to specify a Provider when using the connection method. Here is a list of Provider codes:

ADSDSOObject -	Active Directory Services <br />
Microsoft.Jet.OLEDB.4.0	- Microsoft Jet databases <br />
MSDAIPP.DSO.1	- Microsoft Internet Publishing <br />
MSDAORA	- Oracle databases <br />
MSDAOSP	- Simple text files <br />
MSDASQL	- Microsoft OLE DB provider for ODBC <br />
MSDataShape	- Microsoft Data Shape <br />
MSPersist	- Locally saved files <br />
SQLOLEDB	- Microsoft SQL Server <br />

Example:
Dim myConnection 
'Create and Set Connection Object
Set myConnection = CreateObject("ADODB.Connection")     
Dim myRecordSet 
 
'Create and Set RecordSet Object
Set myRecordSet = CreateObject("ADODB.Recordset")     
 
 'Set up Query
Dim myQuery 
myQuery = "Select NAME from dbo.EMPLOYEE where AGE = 29"
 
'Connecting to database
myConnection.Open "Provider=providercode;Server=servername;User Id=userid;Password=password;Database=databasename"
 
'Run the Query
myRecordSet.Open myQuery,myConnection
 
'Return the Result Set
Value = myRecordSet.fields.item(0)				
msgbox Value
 
'Close and Release
myRecordSet.Close        
myConnection.Close		
 
Set myConnection = Nothing
Set myRecordSet = Nothing
