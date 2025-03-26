# MulesoftLearning
* Mulesoft Technology Learning and Stuffs


## MY LEARNING (YOUTUBE IN DETAILED LEARNING)
* Playlist of Youtube : https://www.youtube.com/watch?v=-apN1Pa1QFk&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=2&ab_channel=SalesforceApexHours

### VIDEO 1 - 25 mins (WHAT IS MULESOFT - MULESOFT FOR BEGINNERS)(https://www.youtube.com/watch?v=-apN1Pa1QFk&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=2&ab_channel=SalesforceApexHours)
* MULESOFT is an API Management Tool (Integration Tool)
#### AGENDA
* PRE-REQUISITES  AND FAQ'S BEFORE STARTING TO LEARN MULESOFT
  * No prior coding language required. But good to know Java
  * Any QA/Linux/SDE background people can learn mulesoft
  * Web-Services and APIs can be helpful
  * Practise Practise and Practise, there are no shortcuts!
* WHAT ARE WEB-SERVICES?
  * A Web Service a way for two machines to communicate with each other over a network
  * A web server running on a computer listens for request from other computers. When a request from another computer is received, over a network, 
    * the web service returns the requested resources.
  * Any software, application, or cloud technology that uses standardized web protocols (HTTP or HTTPS) to connect, inter-operate, and 
    * exchange data message across the internet is considered a web service.
  * TWO TYPES OF WEBSERVICES
    * 1. RESTful Webservice
      * Any kind of data is accepted (XML or JSON)
    * 2. SOAP Webservices
      * Legacy webservices
      * Only XML data accepted
  * EXAMPLE IN GENERAL
    * www.bbc.com
    * So click on HOME bbc/home => Then this open HOME url page. So this is we are asking for resources
    * So in this way we can see how webservices are, and url are sending or rendering that page.
    * As we have also learnd in SPRING MVC that how it works using controller to render html with url. Just to know
* WHAT ARE APIS?
  * API stands for Application Programming Interface.
  * API's allow to communicate/exchange data between two systems.
    * Client => Request => Service
    * Client <= Response <= Server
  * API acts as a broker between client and server. 
  * Like we don't directly attach with DB to Client. In between we have APIs which acts as a broker.
  * Like in Book a flight, in there we pass booking details in that api it will go in db and find that details from DB and send the 
    * available flight and flight details with the prices. So this is how API works.
* WEB-SERVICES VS APIS
  * APIs and web services are not mutually exclusive
  * Every web service is an API - but not every API is a web service.
    * Check some example
  * API's are evolution of Web Services as both purpose is information transfer.
* SOAP vs REST Services
  * SOAP
    * SOAP APIs is largely based on HTTP and XML
    * Request and Response are in XML
    * Uses WSDL
    * Complex to understand
  * REST
    * REST APIs uses multiple standards like HTTP, JSON. URL, and  XML
    * Can be of any format. XML, JSON
    * Uses RAML, Swagger etc.
    * User friendly
* WHAT IS MULESOFT
  * It is a Salesforce Company
  * An Integration Platform
  * An API Management Platform
  * Mule => the runtime engine of Anypoint Platform, is a lightweight Java based enterprise service bus (ESB) and Integration Platform
    * that allows developers to connect applications together quickly and easily, enabling them to exchange data.
  * It enables easy integration if existing system, regardless of the different technologies that the application use, 
    * including JMS, Web Services, JDBC, HTTP, and more
  * API Management Platform Means?
    * anypoint.mulesoft.com
    * Design API's
    * Develop API's
    * Deploy API's
    * Manage API's
    * Secure API's
    * Reuse API's
* 
--

### VIDEO 2 - 37 mins (API LED CONNECTIVITY - ANYPOINT PLATFORM) (https://www.youtube.com/watch?v=jRYQnF0v7_o&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=2&ab_channel=SalesforceApexHours)
* www.anypointplatform.com
#### AGENDA
* RECAP OF PREVIOUS SESSION
* API LED-CONNECTIVITY
  * API-led connectivity is an architectural approach that's closely associated with Mulesoft.
  * API-led connectivity emphasized the creation of well-defined APIs for different layers of an organization's IT infrastructure.
  * Three Layers
    * System Layer
    * Process Layer
    * Experience Layer
  * API-led connectivity follows a "bottom-up" approach, starting with the creation of APIs at the system layer, which are then resued and combined to build  higher-level APIs
    * in the process and experience layers. 
    * (Screenshot attached for better understanding of these layers - API-Led Connectivity.jpg in src folder)
  * This approach encourages resuability, modularity, and separation of concerns, making it easier to manage and update integrations as the organization's needs evolve.
  * 
* SYSTEM APIS
  * System API's are build to connect through underlying systems (Any system which contains the raw data).
  * Basically System API contains Sensitive information as it contains raw data.
  * Should never be expose for public use.
  * E.g. : APIs which connect to Databases, Salesforce, SAP Systems, Hadoop system etc.
* PROCESS APIS
  * Process API's are build to compose or combine two or more System API's
  * Usually to do any kind of transformation or to implement any kind of business logics or shape hte data our of system apis.
  * It may perform aggregation/ splitting / routing the data.
  * Process APIs must be private and should not be expose to public for use.
  * E.g : Aggregating Customer DAta nad Product DAta that comes form 2 system APIs where Actual data is originated, to prove Order Status.
* EXPERIENCE APIS
  * These are API's which are kind of wrapper either to Process API's (if present) or to System API's, so that Client/Consumer can use it.
  * Client/Consumer will not have exposure or contact with direct Raw Data.
  * We can have minimal Data Transformation like the final result to be in JSON or XML or whatever the consumer wants to have.
  * Remember, if there is any change in System API, we do not need to modify or change anything.
* API-LED Connectivity (Flight Example API)
  * See image : API-Led Connectivity.jpg
  * Here we make use of lower System APIs to make our business logic, Like Make use of Product API and Customer API to Make Order. So here making order Process APIs using two system API's. 
  * And so on.
  * Experience APIs is where you do final booking use all below level apis
* CREATING ANYPOINT PLATFORM AND TOUR TO ANYPOINT PLATFORM
  * www.anypointplatform.com
  * Produced by mulesoft company
  * Goto : www.anypoint.mulesoft.com
  * If you don't have a login account in it. Sign up and Create new account.
  * Remember : This is trial account. This Account is only free for 30 days. Only valid for 30 days.
  * After 30 days, you don't have to change the email id. Just change the username with the same email id. 
    * However, you will only lose all the data only. So you can create the backup of the data somewhere else.
  * I have created my account done.
  * From next class we start with Design APIs to Design and Develop API's
  * Exchange is the place in IDE to store your APIs and publish there.
  * Runtime Manager is to deploy APIs
  * More deep dive about this IDE we will see more later.
* ANYPOINT PLATFORM (IDE FOR API DESIGN) - One Stop Platform for APIs and Integrations 
  * Design Center - Design and Develop API's
  * Anypoint Exchange - Place where we will be able to share, discover api's and reusable assets
  * API Manager - Helps in Managing APIs by invoking policies
  * Runtime Manager - Where Applications are deployed
  * Access Management - Configures Access and permission within organization
  * Anypoint Monitoring/Visualizer - Provides Monitoring and real-time graphical representation of APIs
  * Secret Manager - Place to store and control access to private keys, passwords, certificates, etc.
* 
--

### VIDEO 3 - 40 mins (Designing APIs Using Mulesoft Part 1 - Basics of RAML) (https://www.youtube.com/watch?v=jWGHFI7i7Sw&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=3&ab_channel=SalesforceApexHours)
* API Designing steps in mulesoft Anypoint IDE
#### AGENDA
* RECAP OF PREVIOUS SESSION
* WHAT IS AN API SPECIFICATION?
  * An API specification provides an understanding of how an API behaves. (BluePrint of APIs)
    * What kind of Request it accepts?
    * What kind of Response it returns?
    * What are the mandatory fields/Data Types/Security etc.
* DESIGNING API (Using Anypoint Platform Design Center)
* DESIGN CENTER (In Anypoint Platform)
  * API Designer helps us to create API Specification in RESTful API Modeling Language (RAML)
  * It supports RAML 0.8 and 1 versions.
  * It also supports OAS 2.0 and 3.0 both YAML and JSON versions (not in our scope)
  * After creating Specification, it can be published to API Exchange so that it is available to your organization.
  * While designing APIs we need to have following stuffs in that API
    * RESOURCE : It is the unique name we give to identify a resource. It is like url u add after / in controller. Example /home, /student etc.
    * METHOD : GET, POST, PUT, DELETE, PATCH etc. You know this Verb we use.
    * REQUEST : like Body, query params, uri params (example /studentId=?), headers. So in this four way you can pass the parameters. 
    * RESPONSE : like response body and response type
    * HTTP STATUS : 200, 201, 400, 404, 500 etc. 
      * To know this response http status code meaning visit the website
      * https://http.cat/
    * Note - No two resources can have same name and method.
* START WITH API DESIGNING IN THE ANYPOINT PLATFORM
  * Open Anypoint Ide on web browser : Goto : www.anypoint.mulesoft.com
  * click on Design Center (Start Designing)
  * New page opens up, Here click on Create+ button and chose New API Specification
  * Give the project name.
  * You can there select language option either RAML or OAS, for now just chose RAML1.0 and click on create API.
  * So right now we are not developing an API, But we are in designing phase.
* DESIGNING AN API (Coding Part)
  * Using # we can comment in the ide.
  * So first we give our Resource name as "/getAccountSummary:", Also whenever you create enter, you will see it will give you option to chose PUT, DELETE, GET etc.
  * so this is like autocomplete as we have in usual Jetbrains ide. Also when writing this code you can see on right subwindow you will get for what you have made like output things.
  * ==BELOW IS THE CODE PART===
    * #%RAML 1.0
      title: my-first-api
      /getAccountSummary:
        description: "To get static bank account details of a customer with accountNumber as random input - you will get same one account details here"
          get:
            queryParameters:
              accountNumber:
              type: number
            responses:
              200:
                body:
                  application/json:
                    example:
                      {
                        "BankAccountNumber" : 1345,
                        "Name" : "Vicky",
                        "Country" : "India"
                      }
    * So once you prepare this /getAccountSummary GET Api, you can try on run on the right hand side. Just pass the account number input (Any Random number)
    * It will give output as the detail mentioned above for any number. 
    * So this is how it works.
    * For further practise, you can add code in somewhere else or download. Instead of writing here everytime.
    * Now mostly learn by coding, and add comments learn in code only

* CREATING API SPEC USING RAML
* BASICS OF RAML - Resource/Method/Request/Response/Mocking
* PUBLISH TO EXCHANGE
* help.mulesoft.com
--


### VIDEO 4
* API Designing Plus Resource Types and Trait, For reusable methods
* RAML Json type prepared
--






