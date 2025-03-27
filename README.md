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
* DESIGNING AN API (Coding Part) (CREATING API SPEC USING RAML)
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
    * IMP - In the Design, There just click on console on Documentation and then on summary to see all the APIs to check and run and try in console there.
    * PUBLISH TO EXCHANGE
      * Once you created this, you can click on publish right top button, then it will publish in the "Exchange".
      * One in Exchange and then you can use this API from there as well. All your created API you can store there.
      * So in Exchange, a consumer/customer will go and use this APIs without going in deep dive of that API. So this is the use of Exchange.

* BASICS OF RAML - Resource/Method/Request/Response/Mocking
* help.mulesoft.com
--


### VIDEO 4 - 52 mins (RAML and Publish to Exchange in Mulesoft) (https://www.youtube.com/watch?v=2Hom4_8IYq4&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=4&ab_channel=SalesforceApexHours)
* API Designing Plus Resource Types and Trait, For reusable methods
* RAML Json type prepared
#### AGENDA
* RECAP OF PREVIOUS SESSION
  * API Specification
  * Design Center
  * Creating an API Spec using RAML
  * Resource, Request, Respionsem Statuscides etc.
  * Publish to exchange
  
* RAML CONTINUE..
  * When and How to use ResourceTypes?
  * "resourceTypes" refers to a way to define reusable templates or blueprints for different types of resources in your API.
    * Some common functionality which we can use again, So this is some kind of reusability functionality.
    * We will see more in the code
  * It is like set of instructions that you can use to create consistent and standardised resouce definitions.
  * Used for Best practise to avoid writing code again and again.
  * The resourceTypes uses some user-defined parameters surrounded by double angle brackets (<< and »)
  * <<resourcePath» - represent the entire URI (not URL - with the host is called URL)
  * <<resourcePathName» - represents the part of URI (the oath of the URI following the right most forward slash)
  * There are some parameter functions you can use in resource types for example:
    * !singularize
    * !pluralize
    * !uppercase
    * !lowercase
    * !uppercamelcase
    * !lowercamelcase
    * !upperunderscorecase
    * !lowerunderscorecase
    * !upperhyphencase
    * !lowerhyphencase
  * for example, given the resource /health, where «resourcePathName», evaluates to "health"
    * «‹resoursePathName | Suppercase» ==> "HEALTH" (it will make all in caps letter).
* IN CODE NoW
  * Assume we are developing 10 different APIs. In all apis we have standard to follow for health check
  * Code API for health check
    * /healthCheck 
        get:
          responses:
            200: 
              body:
                application/json;
                  example:
                  {
                    time: "8;32 am" ,
                    health: "ok"
                  }
  * But in code we don't want this code to be written in all the APIs to first check the health in there API everytime.
  * Same line of code in 10 different APIs.
  * So we better define this as resourcetype
  * So Code as
    resourceTypes:
      healthcheck
        get: 
          responses:
            200: 
              body:
                  application/json:
                      example:
                          {
                            time: "8:32 am",
                            health: "ok"
                          }
  * Now we will see about how to use this resourceType in our API
  * Now we have made this "healthCheck" resource type, And now we will use this code.
  * So Code to use it
    * /health:
         type:
           healthCheck
  * So now here it will reuse the "healthCheck" resource type in /health api.
  * So now using this in second API as
    * /oneMoreHealth:
        type:
          healthCheck
  * So this way we have used our resource type in two places as in example above.
* CODE WITH HOW ANGULAR BRACKETS ARE USED
  * Note : indentation also plays a good role in how this code is or else it will give error.
  * So code as (Here we just added the description)
    * resourceTypes;
        healthCheck
          get;
            description: Get <<resourcePathName | uppercas>>   # this will give api name where it is going to be used in UpperCase.
            responses;
              200:
                body:
                  application/ json;
                    example:
                    { 
                      time: "8:32 am",
                      health: "ok"
                    }
  * Now this code will be reused as
    * /health:
        type: healthcheck
  * So now when you go and check this API name in console, you will see it will be in Upper case as "get HEALTH".
  * So for any kind of description, you can make use of this angular braces.
  * You can deep dive this topic in raml.org
  * so this is just kind of reusing things.

* IN CODE DEFINING MULTIPLE RESOURCE TYPES IN SAME
  * Here in this below code we have two resourceTypes in same. healthCheck and sravan
    * resourceTypes:
        healthCheck 
          get:
            description: Get <<resourcePathName luppercase>> #this will give api name where it is going to be used in UpperCase.
            responses:
              200: 
                body:
                  application/json:
                    example;
                      {
                        time:"8:32 am" health: "ok"
                      }
        sravan 
          get:
  * Now how to use this as below 
    * /onemoreHealth:
        type:
          sravan
  * So this is how you can define more than one resourceTypes

* TRAITS ( WHEN AND HOW TO USE TRAITS?)
  * "traits" are a kind of resourceTypes
  * Understand this way: resourceTypes are used to extract pattern from "resource" definitions (resource level),
  * Whereas, traits are used to extract patterns from "method" definitions that are common across resources.
  * In simpler tems, traits are defined to use whenever there is a common functionality needs to be implemented across more than one method at-le
  * CODE LEARNING of TRAITS - Using traits, we will make internal call to put username and password and use this in our /getAccountSummary so that
  * This time we also have to pass username and password to getAccountSummary details.
  * CODE
    * traits:
        typeOfVerification: 
          queryparameters:
            username : string 
            password : string
  * Here we have to use "is" keyword to add this Trait in our API /getAccountSummary
    * #GET API
        /getAccountSummary:
        description: "To get static bank account details of a customer with accountNumber as random input - you will get same one account details 
        get:
          queryParameters: 
            accountNumber:
              type: number
            is:
              - typeOfVerification 
            responses:
            200: 
              body: 
                application/json:
                  example;
                    {
                      "BankAccountNumber" : 1345,
                      "Name" : "Vicky",
                      "Country" : " India"
                    }
  * So now after adding this code, we also have to add username and password along with the accountNumber to call /getAccountSummary API.
  * So this is like adding the extra queryParameters 11ke Traits.
  * So this is how we make use of Traits.
  * Also we can make use of other like Body instead of queryParameters and other items. You can explore this yourself.
  * This similar trait you can also add in the /createAccount and use it other APIs as well.


* USING linclude, type, types, Resource types Vs Traits, smal validations, etc
* HOW TO USE MOCK URL?
* PUBLISH TO EXCHANGE
* raml.org
  





