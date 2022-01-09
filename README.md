# SNOW-Web-Services

- A Web Service is an HTTP-based communication method that lets diverse applications exchange information and talk to each other. 

## Inbound Web Services: 
- Inbound web services allow you to access and modify ServiceNow data using a client application.

## Outbound Web Services: 
- Outbound web services allow you to send SOAP and REST messages to external web service providers. 

## Publisher of Web Services (Provider/Producing)
- Publishing a web service in ServiceNow that can be consumed by a 3rd party can be accomplished by creating a new Inbound Web Service
- Publishes web services for clients to invoke (consume)

## Consumer of Web Services (Consuming)
- Consuming a 3rd party web service from ServiceNow can be accomplished by creating a new Outbound SOAP Message or Outbound Rest Message.
- Invokes / Consumes published web services.

## Web Services Components
![image](https://user-images.githubusercontent.com/12488769/148688569-69346e0f-74a3-43c6-940d-e21a31599a1c.png)

## Web Services & ServiceNow

- A method of communication between two electronic devices over a network

- ServiceNow supports both inbound (provider) and outbound (consumer) web services.
A method of communication between two electronic devices over a network

ServiceNow supports both inbound (provider) and outbound (consumer) web services.
![image](https://user-images.githubusercontent.com/12488769/148688601-ad3f39d6-61cd-4ad2-8095-7e9c534162fc.png)

## Web Services Methods
![image](https://user-images.githubusercontent.com/12488769/148688623-db539c3d-ba5d-410f-9c6b-d9f924539fb6.png)

The ServiceNow system supports access (input and query) to its tables and their data by using these below methods:

- Direct Web Services (get, insert, query)
- Web Service import sets that do data mapping using Transform Maps
- Scripted Web Services that are executed in JavaScript


## Direct Web Service:
Endpoints are accessed directly using a URL, which is integrated on  the UI level between two or more applications. It directly manipulates the data into the target tables. Therefore, there are many security considerations with this Web Service Method.
URL format: https://<instance name>.service-now.com/<table_name>.do

## Mapped Web Service:
  All Web Services import sets go through a transform map to match fields.

## Scripted Web Services: 
  Helpful when the other system requires a very specific integration that Simple Web Services cannot provide. It parses the information and determines the source.
  
## Example: 
  Servers in locations all over the world are tracked in one CMDB. The MID Server checks the server message queue and uses scripting to determine which location sent the record. If it was San Diego, the update will go to San Diego Servers table.

## Note:
  If we have a large amount of data, Mapped Web Services process data one by one and the cost of transformation is quite high. Scripted Web Services is lower cost and for large amount of data, the better choice.

## REST Web Services
-  REST (Representational State Transfer) is a simple stateless architecture that provides standards between computers systems on the web, making it easier to communicate with each other.

- The NOW platform provides various REST API’s which are active by default.

- There API provide the ability to interact with various ServiceNow functionality within your application

- Such functionality includes the ability to perform Create, Read, Update and Delete operations on existing tables (Table API)


### REST ENDPOINT:

https://myinstance.service-now.com/api/now/table/{tablename}

## SOAP  Web Services
-  SOAP (Simple Object Access Protocol) is an XML based protocol for accessing web services over HTTP.

- One can use SOAP API to perform Create, Read, Update and Delete operations on existing tables (Table API)


### WSDL:

https://myinstance.service-now.com/instance.do?WSDL





