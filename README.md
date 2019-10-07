# BC-Webservice-Access-by-Postman
Create Webservice And Access by Postman

As the API is simply a standard RESTful API, we can use some industry-standard tools to navigate through the API to see what's available.
This recipe will show you how to use Postman to take a look at what's available in the Business Central API.

Creating Webservice and consuming it with external tool as easy as you think.
Steps are below

Configurations Changes

To make Business Central Available in Postman first Step is to make few changes in Business central Admisitration, Open Business 
Central Administration and check mark these option

i:In General Tab enable NTML Authentication.
ii:Open Soap Service --> check Mark "Enable SOAP Service".
iii:Open OData Services --> Check Mark "Enable OData Services". 

Code
Now you need to create a XML file like I have uploaded, Publish your code in Business Central.
Run Busniess Central Search for Web Service, All web services which are available in business central, If your webservice don't have any error
it should be available there. Search it by ServiceName.
scroll to right and copy ODATA URL of you Webservice

PostMan Setting 

Create a get request and past copied ODATA URL here.
Select Authorization and chooose authentication TYPE 'NTLM Authentication'.
Give your system UserName and Password in Authorization's Username&Password.
In Header Tab key="Content-Type",value:"application/json"
In Body Table Select Raw
Now Send your Request
Here should be the result on your webservice.



