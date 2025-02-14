With serverless, a user can simply create and upload code, 
and then define the triggers or events that will execute the code.
------------

created Azure Functions in Java
https://docs.google.com/document/d/1PSanqd0Pj59WOfX9jqNdeY7RYUtrFEMi/edit
1) create azure storage account
2) Initialize a Java Azure Functions Project
3) mvn clean package
4) to run the azure function in local in windows machine you need azure function tools msi 
    -- Please go to https://aka.ms/azfunc-install to install Azure Functions Core Tools first
    -- download the windows msi and install it 
5) mvn azure-functions:run
6) go to browser test1: http://localhost:7071/api/HttpExample  test2: http://localhost:7071/api/HttpExample?name=Ramesh
7) curl http://localhost:7071/api/HttpExample?name="Ramesh"
8) deploy the azure function using azure core tools in azure portal
9) az login
10) mvn azure-functions:deploy
11) once deployement is success --> HTTP Trigger Urls:
[INFO]   HttpExample : https://azfuncdev-20250214222923307.azurewebsites.net/api/httpexample
12) test the azure function hosted in remote  https://azfuncdev-20250214222923307.azurewebsites.net/api/httpexample?name=Ramesh
