# :rocket: ATCP SMEs API Testing Wiki :rocket: #
ATCP centralized source of information all about API Testing.
> ### Wiki Version ##

Version       | Author              | Description                           | Date
------------- | ------------------- | ------------------------------------- | -------------
0.01          | Jason C. Seguerra   | Drafted inital content                | 10/04/2021
0.02          | Geyvin D. Ediezca   | Wiki to markdown file conversion      | 12/10/2021
> ### Terminologies ###
#### XML ####
_XML stands for extensible Markup Language. It’s a mark-up language much like HTML. XML was designed to store and transport data_
#### WSDL ####
_WSDL stands for Web Services Description Language. WSDLs are an XML format that tells you how to access a web service. WSDL is used to describe web servicesWSDL is written in XML_
#### SOAP ####
_SOAP stands for Simple Object Access Protocol. It helps in exchanging structured information between computer networks. SOAP allows communication between different operating systems using XML._
#### SOA ####
_SOA (Service-oriented Architecture) is a way in which companies can organize software that can be quickly changed to respond to the requirements of the marketplace. Web Services are small units of software that run in a network. Web services can be strung together in multiple ways and used by different applications to create the desired functionality._
#### REST ####
_REST stands for Representational state transfer. These are web services that provide interoperability between computer systems over the internet._
#### JSON ####
_JSON stands for JavaScript Object Notation and was designed to be a lightweight data interchange format. JSON is definitely becoming more popular and is now replacing XML in certain situations for API data exchanging._
#### GET Method ####
_The HTTP GET method is used to retrieve data. It is a read only call and data cannot be modified. If it is a successful request, without any errors, then a status of code of 200(OK) is received along with the data requested in the particular format which is generally JSON or XML._
#### POST Method ####
_The HTTP POST method is a write method. It is mainly used to create a new resource by providing the input in Json or XML format. When a POST request is made, a new resource is created with the values provided along with it. If it is an error free call, the status returned will be 201._
#### PUT Method ####
_The HTTP PUT method is more like an update command. It is used to change the value of any resource whose original value was something else. PUT methods can also be used to create resources but only if the the request is from the client and not the server._
#### DELETE Method ####
_The HTTP DELETE method, as the name suggests, is used to delete a resource. If the request is made successfully then the status code returned is 200 (OK). These are also idempotent as if a resource is deleted once it cannot affect it._
#### Web Service ####
_Web Service is a method of communication between two electronic devices over a network. It is a software function provided at a network address over the Web with the service always-on as in the concept of utility computing._
#### Uniform Interface ####
_The uniform interface constraint defines the interface between clients and servers. In other terms, First constraint of the REST API states that the Client and server has to communicate and agree to certain rules based on resources(they should communicate with same resource like json, xml, html , txt) and with proper encoding like UTF-8 extra._
#### Stateless ####
_APIs in REST are stateless and Client and server doesn’t worry about the state of the request or response._
#### Cacheable ####
_According to the World Wide Web, clients can cache responses. Responses should therefore, implicitly or explicitly, define themselves as cacheable. Its upto server when they want the cache to expired etc._
#### Client-Server ####
_Client and Server are two different entity, It means that servers and clients may also be replaced and developed independently, as long as the interface is not altered._
#### Layered System ####
_It means that the between client and server there can be any number of layered systems it does not matter._
#### Code on Demand ####
_Server can store the Code or logic to themselves and transfer it whenever needed rather client side logic. If any API fulfill all the constraints then we can it REST API._
#### API Load Tests ####
_Load API tests, typically run in production or an equivalent system. APIs and consumers form client-server systems where multiple clients hit the same server at the same time, and the number of clients can drastically affect the behavior of the API. You specify the number of virtual users, the test script and the time to run the test and all VUs hit your API continuously during the specified time while the testing tool records the performance._
#### API Stress Tests ####
_When performing Stress Testing, you start with a low to medium number of VUs and then, step by step, increase their count. This process is also called ramping up. The idea behind this testing approach is to continuously grow the load to find the point at which your API becomes either too slow, non-responsive or throws errors._
#### API Soak Tests ####
_The idea behind Soak Testing is that sometimes a system seems to perform as expected under a particular load and then, all of a sudden, it stops working without any changes in traffic. Running out of server memory or disk space due to leaks or not cleaning up logs etc. is a common reason for it._
#### Peak and Spike Tests ####
_With Peak Testing you simulate your API at peak times. These are the times during which you expect a higher load. A peak test is typically shorter than a soak test and often includes ramping up and ramping down to a higher pressure but not as huge as within a stress test._
#### Endpoint vs. Scenario Testing ####
_When performance testing, you can call a single URL, or multiple URLs in succession.The most straightforward approach is just testing single API endpoints._
#### API Monitoring ####
_Last but not least, let’s look at API Monitoring, which is related to testing. API Monitoring typically includes simple uptime checks as well as performance or functional tests. For the latter two, you can use your existing test definitions to build your monitoring system._
#### API Endpoint ####
_This is referred to from the application point of view. The end of the communication channel of an application that allows other applications to interact with is called an API Endpoint. Endpoint is the boundary of the application which ends the responsibility of the application._
#### URI ####
_Identifier of a specific resource using both location (URL) and name (URN)._
#### URL ####
_Subset of URI, often can be identified as a string directed to an address._
#### Base URL ####
_The consistent part of a URI._
#### Path params ####
_Type of a parameter lives with the URI._
#### Query params ####
_Type of a parameter added to the end of the URI after “?”._
#### Authentication ####
_identifying the users by confirming who they are._
#### Authorization ####
_The process of assigning rights and privileges to the user._
#### OAuth ####
_Open Authorization._
> ### Training References ###

Level         | Course Name                                | Link
------------- | ------------------------------------------ | ---------------------------------------------------------------------
Beginner      | API Testing                                | https://accenture.percipio.com/courses/c9614755-e978-4ed0-8706-381cbc3969cc/videos/dfcd036a-2e02-4ac2-8734-88a777f226e7
Beginner      | API Testing and its Benefits               | https://accenture.percipio.com/courses/1f25bee1-8662-4e55-94d1-95b691512c6e/videos/16d7a540-ecfb-41c2-9206-08569a3426cd
Beginner      | API Testing using Jmeter                   | https://connectedlearning.accenture.com/learningboard/778872-api-testing-using-jmeter
Advanced      | Gherkin Scripts for API Testing            | https://accenture.percipio.com/courses/53f76cf8-c47b-4186-b19f-eeb4935bb9f2/videos/92b59ce9-c8b1-4c95-8531-9290ab25069f
Advanced      | API Management: Strategy & Monitoring      | https://accenture.percipio.com/courses/5faa25ba-eb9f-4023-ba7f-f8d1e7893c1a/videos/0236d57d-2e58-4789-ba34-bdea1dcfc078
Advanced      | CI/CD API Testing                          | https://accenture.percipio.com/courses/895e44f8-fc92-4ebf-b927-c3e57d77b292/videos/24d18e72-1aa4-47b2-a0b7-8d61054846b4
> ### API Testing Tools ###

Common API Testing Tools   | Reference Link
-------------------------- | ---------------------------------------------------------------------
Postman                    | https://www.postman.com/product/what-is-postman/
SOAP UI                    | https://www.soapui.org/
REST-Assured               | https://rest-assured.io/
Swagger.io                 | https://swagger.io/
JMeter                     | https://jmeter.apache.org/
Katalon Studio             | https://www.katalon.com/
Apigee                     | https://docs.apigee.com/api-platform/fundamentals/download-api-proxies
Assertible                 | https://assertible.com/
Karate DSL                 | https://github.com/karatelabs/karate
API Fortress               | https://rapidapi.com/products/api-testing/
Hoppscotch                 | https://hoppscotch.io/
Testim                     | https://help.testim.io/docs/api-testing
Ready API                  | https://smartbear.com/product/ready-api/overview/
Neoload                    | https://www.neotys.com/blog/executing-api-testing-with-neoload/