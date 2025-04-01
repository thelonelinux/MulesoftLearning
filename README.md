# MulesoftLearning
* Mulesoft Technology Learning and Stuffs
* Other Mulesoft Learning suggested by Vishaksha
  * TechZone :  https://www.youtube.com/playlist?list=PL61bQcdxsK6_1tb0BbAtAOX_SdtvgQlxV
  * Developer Guide : https://www.youtube.com/playlist?list=PL2LUDEomJp_jNB4v-rFn6GmpbOZqkhIlR


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
* API Designing steps in mulesoft Anypoint Web IDE
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

#### AGENDA
* RECAP OF PREVIOUS SESSION
  * API Specification
  * Design Center
  * Creating an API Spec using RAML
  * Resource, Request, Respionsem Statuscides etc.
  * Publish to exchange
* API Designing Plus Resource Types and Trait, For reusable methods
* RAML Json type prepared
  
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
            description: Get <<resourcePathName | !uppercase>>   # this will give api name where it is going to be used in UpperCase.
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
        type: 
          healthcheck
  * So now when you go and check this API name in console, you will see it will be in Upper case as "get HEALTH".
  * So for any kind of description, you can make use of this angular braces.
  * You can deep dive this topic in raml.org
  * so this is just kind of reusing things.

* IN CODE DEFINING MULTIPLE RESOURCE TYPES IN SAME
  * Here in this below code we have two resourceTypes in same. healthCheck and sravan
    * resourceTypes:
        healthCheck 
          get:
            description: Get <<resourcePathName | !uppercase>> #this will give api name where it is going to be used in UpperCase.
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
  * After here mostly learn via code only. By watching videos.
  * Purpose of doing this resourceType and Traits : to identify repeated stuffs and eliminate it using this.

* DEFINING SCHEMA USING DATA TYPES (HANDS ON WITH CODE)
  * JSON object, which is key value pair.
  * { "key" : "value" }   (this is a JSON object or say object)
  * JSON Array is anything which is closed in [] brackets
  * { "key" : "value" , array : ["1" , "2", "3"] }  (As array example in json object)
  * In www.jsonlint.com
    * Here you can go and write json objects
  * So here we are just learning to define our JSON Schema, how it should be and it's properties data types.
  * See in video, just defining in new file.

* USING !include, type, types, Resource types Vs Traits, small validations, etc
  * See in video for use of !include
  * Creating JSON type object item in our code.
    * Create a new file in anypoint website. 
    * API Format : RAML 1.0
    * File type chose : Data Type
    * File name : yourFileName.raml
    * And then click create
  * So we are just doing this to create a data schema in json type.
  * Here we learn use of !include and how to create example json and use in our api for response. 
  * We create response - JSON class. And example of JSON object.
  * And how to use this as response we use in api
  * We also added constraints like min max when creating JSON class. So this is how it works. 
  * When creating the example select filetype as example.
  
* HOW TO USE MOCK URL?
* PUBLISH TO EXCHANGE
* raml.org

### VIDEO 5 - 59 mins (Developing APIS - Part 1 - MULE 2 - MESSAGE STRUCTURE and Anypoint studio) (https://www.youtube.com/watch?v=HG2mdaw1_Ak&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=5&ab_channel=SalesforceApexHours)
* NO NEED TO WRITE DEVELOPMENT
  * ANYPOINT STUDIO IDE Download
#### AGENDA
##### 1. Developing APIs
##### 2. Mule 4 Message Structure
* MESSAGE STRUCTURE
  * Mule Event
    * Mule Message (PayLoad + Attributes)
    * Variables
    * Error Information
  * Mule Event = Mule Message + Variables + (Error Information) 
  * Mule Message = Payload + Attributes 
  * In Simple terms :
    * A Mule 4 messge is like an envelope that contains a letter (payload), some informatin on the outside (attributes), 
      * sticky notes (variables) you can attach, and a place to write down any problems that might occur (error information). 
      * All of these components work together to help you process and manage data in your Mle 4 application.
  * Mule Event & Message Structure
    * Payload : It's the actual message content. Payload can be over ridden.
    * Attributes: These provides metadata information such as queryParams, urParams, file size etc. These are immutable (cannot be changed)
    * Variables: These are which you can store some kind of data or information and can be used across the application as long as you connect the flows the flow-ref.
    * Error Information: In case any error occurs in the application, an error object is produced which contains all the information related to the error.
* ANYPOINT STUDIO TOOL TO RUN CODE (SEE BELOW)

##### 3.Anypoint Studio (Download and install and get started with the IDE)
* DOWNLOAD AND INSTALL ANYPOINT STUDIO (See in video only)
  * It comes with inbuilt maven and java
  * https://www.mulesoft.com/lp/dl/anypoint-mule-studio
  * In the download section - You have to select this things.
    * Product Selection : Mule and Studio
    * Select Version : Latest
    * Select OS : Windows (A/To your computer)
    * Rest of the details you add, you can remove company name and mobile and just download at the end.
    * You will get the download link in your gmail.
    * You can also watch this yt video : https://www.youtube.com/watch?v=caL_2HAIZ5I&ab_channel=Sayeed
    * Also remember, better put your download and then extract in D:// Location only, As lengthy path name was also causing issue.

* CODE PART
  * Layout of your IDE.
  * It looks similar like our SSIS. But different from that of Web Mulesoft
  * There is Canvas (Plane area), File/Package Area, Tools Pallete/Mule Pallte, Console. Similarly like in any other ide or like in SSIS ide.

* CREATE A NEW PROJECT
  * Step see in video only
* CONNECTORS - Here tool or mule pallets which we drag and drop are called as connectors
* FOR GK -
  * If you want to reset views then in anypoint studio, go in widow » perspective » reset perspective

##### 4. MuleSoft Project Structure
* MULE PROJECT STRUCTURE
  * Every Project in Mule 4 is Mavenized Project (pom. xmi)
  * All Mule xml's are placed under src/main/mule
  * Other files can be placed under : src/main/resources or src/test/resources
  * mule-artifact.json (We will discuss more about it later)
  * Each Mule app xml has
    * Message flow (Graphical View)
      * This is main part where you drag and drop your tool / mule pallets like in ssis.
        * when you open the src/main/mule app.xml there you make this project drag drop in this section.
    * Global elements (contains all config details)
      * Here you create global variable, DB connection details. Similarly you know you had in sSIS.
    * Configuration xml (xml version of graphical view)
      * So here in Message Flow tab whatever tool/mule pallets you drag and drop, it is converted into its xmi in configuration xml.
        * These things you can see in IDE code plane bottom only. If you open src/main/mule app-ml file, there it is.
    * More details see in code always. in video

##### 5. Flow, Sub Flow & Private flow
* FLOW, SUB-FLOW AND PRIVATE FLOW (This is like same arrow flow you did in ssis)
  * An App can consists of a single flow !
  * Or it can break up processing into discrete (private) flows and sub flows that you add to the app and connect together.
  * Private and sub-flows can be triggered by Flow-reference or by DataWeave lookup! (We will look more about this in code on hands on)
* FLOW
  * A flow has "Source" , "Process" and "Error Handling" Part
  * You should definitely keep something in Source
  * Image you can see in YT. It contains all those three parts mentioned.
* PRIVATE FLOW
  * A private flow has "Source", "Process" and "Error Handling" Part
  * It's called a private flow when we don't keep anything in Source Part
* How to use this flow in our project.
  * Open src/main/mule app-xml
  * Go in Mule Pallete (Tools), Search for flow
  * You will get there options for Flow and Sub Flow, but not private flow
  * Private flow are self attributed by developer.
  * So now drag and drop flow, there you will see we have source, process and error handling.
  * Since our is RESTApi which used HTTP protocol,
  * We will add listener in our Source, So that we will know which is calling our API, as you know.
  * Check in video only for about how it is dragging and dropping, Good explained.
  * So if we remove listener from source, then our flow will be called as private flow, as now we don't have anyone to listen our https, so this is what we call private flow.
  * So all this tools you are adding from mule pallete are called CONNECTORS. This connector you are adding in either source or process or error handling section of the flow.

##### 6.Connectors
* You have already seen some connectors (tools) which we drag and drop from above part
* There are thousands of connectors in mulesoft
* Remember like SSIS, here also we are not writing any code, We are just dragging and dropping the connector/tools and doing our configuration and job task.
* So now we will start with our API DEVELOPMENT
  * We will start with HTTP Listener connector/tool, see below part now.

##### 7. Http Listener, Set Payload connectors
* HTTP Listener (Connector/tool)(Present in HTTP in Mule Pallete)
  * Listens to the request which client/user sends.
  * Mandatory Config Details required: host, port, path
  * Default: Accepts all kind of Methods if nothing is specified. Method like verb etc.
  
* Set Payload (Connector/tool) (Present in Core in Mule Pallete)
  * The Set Payload component lets you update the payload of the message.
  * The payload can be a literal string or a Dataweave expression
  * Mandatory config Details Required :
    * value eg:
      * #["Hello World"] or #[payload]    or #[attributes.queryParams.name]
  * Default: #[payload]
  * Set Payload connects to the client when drag and drop and put in process
  
* Hands on with code
  * HTTP Listener
  * Set PayLoad
  * Building Simple Rest Application
  * Debugging an application

* See in next part for hands on

##### 8. Building a simple REST API - Hands-on
* STEPS
  * Drag and drop a flow
  * Add (Drag and drop) HTTP Listener connector in Source
  * Add (drag and drop) Set Payload connector in process
  * Double click on the HTTP Listener to do the configuration in it.
    * In the General Tab
      * Make Display name as you wish
      * Other host details you can add and test connection. See video only and do when practising code.
  * It's all about click, drag, drop, configure, so just check video and develop a simple REST API.
   
* To run the project. right click on the project canvas plane, and then click on Run Project "projectName",
  * So now in console you can see project is running,
  * In the console when you see the status is Deployed, means you project has successfully run.
  * Now open the browser. Whaterver you configured in host just search that port
    * http://localhost:8080/test
* To stop the application, click on stop red button in ide only

* Deploying via sandbox the jar file which you have created in Anypoint IDE Projects (See video)
  * Deploying via web browser mulesoft only
  * Click on Runtime manager.
    * (However for now sir is just showing it to us. but in future we will go deep dive in deplopyment)
  * Chose Design environment (Not sandbox)
  * Click on Deploy Application
  * Before deploying, first stop the application from Anydesk studio
  * Some other step check in video only. we will see in detail in later videos for deployment. So that's it.
  * use port as  : ${http.port}    for deploying
  * we use : 8080 usually.
* Jar file deploy in sandbox, just check video for step. but later do more.
  * Jar file you can get from your app project. Right click and see the steps.
  * You can also open in your browser as he has deployed in cloud sandbox.
  * So this is all about it.
  * After deployment is done, it will give you app url
    * Go in settings, once deployment is done to get the app url.
      * https://vicky-sandbox-deploy-3ustpy.5sc6y6-4.usa-e2.cloudhub.io/display

##### 9. Debugging application in Anypoint Studio - Hands-on
* We will learn about this in next video class.

### VIDEO 6 - 61 mins (Debugging application in Anypoint Studio) (https://www.youtube.com/watch?v=rebYIty04mI&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=6&ab_channel=SalesforceApexHours)
#### AGENDA
##### 1. Debugging application in Anypoint Studio - Hands-on

##### 2. Flow - Reference - Hands-On
* Flow Reference (Connector)
  * As we discussed in our previous class, we have normal, private flow and sub-flow.
  * So to connect these private flows and sub-flows we need Flow-reference connector.
  * Use to call a sub-flow/private flow.
  * Mandatory Config Details required: flow name to be called. All names are present in drop-down list.
  * Default: empty but it fails to deploy if you don't give any flow name from drop down.
* Hands-on
  * Watch video - To connect flow with private flow.
  * Also download postman - for testing our APIS
  * To check the flow how request is being processed step by step we need debugging
* Debugging
  * This time instead of run the project, choose debug the project,
  * See video on how to do debugging.
  * You can also set debug configuration, in menu of run » Debug configuration
  * So run the api in postman, you will see the breakpoint will get hit,
  * During debug we can see in Mule Debugger, it contains
  * For debugging put yor cursor on flow-reference connector, right click and put break point.
* Attributes (In Mule Debugger tab during debugging)
  * This contains meta data, you can check here during debugging.
  * example like listener path, method, requestPath etc.
  * You can get attribute details with #[attribute.requestPath] or #[attribute headers] when debugging by click on evaluate.
  * Check in video about how it is doing evaluate and getting attributes values. host values ete.
  * Use attribute name with case sensitive only.
  * {# and [] } are automatically added in evaluate even you don't add it. You can just write attribute.requestPath
  * So this is all about flow-reference, debug and attributes.
  * Now checking with variables. (See in next part below)

##### 3. Attributes and Variables
* Attributes
  * We know that attributes is part of Mule Message
  * Attributes are nothing but the meta-data coming from the system which we are connecting.
  * Accessed as #[attributes.requestPath]
    #[attributes.queryParams.name]
  * Attributes are replaced with new or no values whenever we connect to any external systems.
* Variables (Lies in Mule Event Hierarchy only)
  * Mule 4 has only one kind of variable called "variable" whereas in Mule 3 we used to have 3 kinds of variables (flow, session and record) - Now deprecated.
  * They are used to preserve information which you think might be useful to any point of flow.
  * Accesses as #[vars.id]
  * IMP - Vars are carried as long as the flow is connected. If you think that you no longer need the variable, you can use "remove variable" to remove it.
* Hands-on Variables
  * Search Set Variable tool from mule palette. and drag and drop and put in. Check in video.
  * You can give id and value for this Set variable mule palette.
  * Mostly you have to do here is see video and do code practise only more to understand.
  * Further check in below part

##### 4. SET VARIABLE and Attributes - Hands-On
* Set Variable (Connector/tool)
  * Here also after adding Set variable and doing debug and check in evaluate to check your variable value attributes.
  * Also you can see here that wars are carried as long as connector are connected.
  * You can add as many as Set Variable connector in your app.
  * Now we will check with logger component/connector in next part, see below

##### 5. LOGGER
* Logger (Connector/Tool)
  * Log the information for tracking purpose, Logs appear in the console.
  * Mandatory Config Details required:
    * Nothing is mandatory here. You can set anything in "message" field.
* Hands-on
  * Anything you see in console. when running or debugging the code. those are loggers only.
  * So last time we set apple value in our Set Variable.
    * So how to know what is this value is. We can do this by the use of logger.
  * So search for "logger" tool in the mule pallete. Drag and drop and do the configuration
  * Code it and practise and see in video you know how to do.
  * You can add as much as logger as you want to log after every tools you want to log
  * Just start the api, clear the console, call the api, you will see apple log displayed in console.
  * We will also check how to pass queryParameters in this project
  * Adding logger after flow-reference, then after going to set Payload only, it will hit last logger.
* Query Parameter (Adding query parameter)
  * localhost:8080/students?id=123
  * check more in video
  * http://localhost:8383/setpayload?name=mulesoft
  * Name you can add as dynamic attribute
* So for now our next concept "Scope of Attributes, Payload and variable" logger can help us to understand the scopes. Check in next part below

##### 6. SCOPE OF ATTRIBUTES, PAYLOAD AND VARIABLES - Hands-On
* XML view of your payloads and attributes check in Configuration XML as well.
  * Check in video only, when debugging, what value will be there for that syntax
  * to know the scope of values while going from different connectors.

### VIDEO 7 - 15 mins (Scope of Variable attributes and payload) (https://www.youtube.com/watch?v=_26LGlyj-Do&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=7&ab_channel=SalesforceApexHours)
* Some previous continue code with request connector
#### AGENDA
##### JUST CONTINUE CODE PART 

### VIDEO 8 - 47 mins (Mulesoft Dataweave Part 1) (https://www.youtube.com/watch?v=GLpXQvyobvA&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=8&ab_channel=SalesforceApexHours)
#### AGENDA
##### 1. RECAP OF PREVIOUS SESSION
* Flow-reference, Attributes and Variables, Set variables and attributes
* Transform Message, Logger, Scope of attributes, Payload and variables - Hands-on

##### 2. CONFIGURATION PROPERTIES
* Configuration Properties
  * Property values are used for best practices to extract some values from property files using corresponding to avoid Hardcoding values.
  * We can extract property values from property file by two ways, either by ${} or p('')
  * ${} can be used anywhere at any place, either in configuration or in dataweave etc.
  * p('') can only be used in DataWeave expression Language scope. i.e. within #[]
  * Remember : Either of the cases, we have to restart the application if there are any changes made in property file to get the new values reflected.
* Hands On
  * How we made ${http.port} when deploying, Now also we will do and add the property of http port in test.properties file in src/main/resources
  * So this way we reduce hardcoding.
  * add this test.properties file attach with your tool canvas from Global Elements, Create Configuration. Select Configuratoin Properties, upload your test.properties file.
  * Now you can make use of your properties file in coding. see video for more.
  * In Properties code as : 
    * http.port : 8484
    * message : Apex Hours
  * In Transform Message connector code as 
    * output application/json
    * ---
    * {
    * "value using dollar " : '${message}',
    * "value using p " : p('message')
    * }

##### 3. DATAWEAVE 2.0 INTRODUCTION (Both in same)
##### 4. DATAWEAVE - THE POWER PF PREVIEW AND ONLINE DATAWEAVE PLAYGROUND FEATURE (Both in same)
* Dataweave - the power of preview feature
  * Dataweave : Transform some data from database
  * Are you not sure the syntax you want to write?
  * Are you struggling to deploy your application always, to check whther your syntax or DW is correct or not?
  * DataWeave Preview & Playground helps us to overcome it!
  * Please make sure that your Tooling instance is running properly. or else this feature won't be available.
    * Go in window >> preferences >> Search Tooling >> Below status,if it is not running then click on restart studio
    * Now your tooling services will start, which will give you preview options in your transfrom message whenever you write.
      * Preview option is there in side up right hand side, click on it. and you can see the preview of your code.
  * This is online Dataweave Palyground feature - You can learn from here.
    * https://dataweave.mulesoft.com/learn/dataweave

* Hands-one
  * Simple video code of preview as mentioned above

##### 5. TRANSFORMING ONE DATA TYPE TO OTHER
* Understanding object and Arrays
  * How to Identify an Object and an Array?
  * An Object is always enclosed with {} and contains key-value pair.
  * Eg:
    * {"name" : "Sravan"}                => Correct Way
    * {"name" : "Sravan" , "id" : "2" }  => Correct Way
    * {"Sravan"}                         => InCorrect
    * {"name" : "Sravan" , "2" }
  * An Array is always enclosed with [] and contains only values
  * Eg:
    * ["Sravan", "2", "Mulesoft"]     => Correct way
    * {"name" : ["Sravan", "Lingam"]}  => InCorrect
    * ["name" : "Sravan"]             => InCorrect
    * ["hello" , {"name" : "vicky"} ] => Correct way
  * Tool website where you check the correct json syntax
    * https://jsonlint.com/
    * Here you can check whether a data is valid or not. A json is valid or not here you can check.

* Transforming one data type to other
  * In Mule 3, we have separate connectors to convert from one type to other.
  * In Mule 4 we use DataWeave to achieve this.
  * Eg: 
    * JSON to XML
    * XML to JSON
    * JSON to CSV
    * And many more....
  * Here you can see example of converting from json to xml (In video)
    * https://jsonlint.com/

* Hands On - Converting JSON post you put to XML from Transform Message: 
  * Just add this in Transform message (DataWeave syntax to convert json to xml) : (Rest see in video code for converting Json to xml and vice versa using dataweave project) 
    * %dw 2.0
    * output application/xml
    * ---
    * details : payload
  * Or you can add code in this way
    * %dw 2.0
    * output application/xml
    * ---
    * {details : payload}
  * This above code will convert the JSON object to XML. This is DataWeave Syntax above
    * {
      "message": "Hello world!"   ,
      "name" :   "yik"
      }
  * to 
    * <?xml version='1.0' encoding='UTF-8'?>
     *   <details>
      *    <message>Hello world!<message></message>
      *    <name>yik</name>
      * </details>
        
* Now we will have input as xml and output as json    
  * Then add below dataweave code in Transform message. In postman add xml type post data, 
  * It will give output as json data for that posted
    * %dw 2.0
    * output application/json
    * ---
    *  payload

### VIDEO 9 - 57 mins (Dataweave Part 2) (https://www.youtube.com/watch?v=Kch-Tks3QP4&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=9&ab_channel=SalesforceApexHours)
Dataleave is basically a Mulesoft expression language. It is mainly used for accessing and transforming the data receivd through a Mule application.
* Do mostly hands-on only learn by code only to transform in Dataleave Transform message connector
* this is mosity coding practise and not much of theory. Do mostly code practise only.
* Map and Mapobject syntax learning only.
* For detailed syntax notes check : Tutorials Point Mule soft, Can learn from there rather than making notes here, here only do that much code notes only in hands-on
####  AGENDA
* MAP AND MAPOBJECT
  * map operator is ued on Arrays.
  * mapobject is used for Objects.
  * You cannot use mapobject operator for Arrays.
  * You cannot use map operator for objects.
  * $: gives the value of the particular field/key.
* HANDS-ON
  * See all in video and do coding syntax

### VIDEO 10 - 41 mins (Mostly do in code practise only - Dataweave Syntax Learning Part 2)  (https://www.youtube.com/watch?v=GB7wu1lokmg&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=11&ab_channel=SalesforceApexHours)
* You can learn from online documentation of mulesoft. Search Dataweave2.0, You can see this in video and learn
* MapObjet Mule: search this also you can check. Main website is mulsfot one only, there only all are there syntaxes.
#### AGENDA
* CONTINUE WITH DATAWEAVE SYNTAX LANGUAGE
* Map and Mapobject
* Reduce and Flatten
* Cannot coerce errors
* Reduce
* Flatten
* groupBy
* DistinctBy
* Custom functions
* Define local variables
* There are many more Dataweave syntax to learn (Mostly practise on DataWeave playground and in code we were using in Transform Messgae connector)

### VIDEO 11 - 59 mins (Developing APIs) (https://www.youtube.com/watch?v=gbgb0axNZFs&list=PLaGX-30v1lh0YPFM-RU7ddYcFNiFLj-ab&index=12&ab_channel=SalesforceApexHours)
* Some theory also to learn v ###*# AGENDA
##### Recap of Previous Session
v ##### Things to remember when connecting to external systems
* External Systems: Database, Salesforce, SFTP, any external Mebservices etc,
* Gather the configuration details that are required to connect to that particular system.
* See what is the request that particual system is accepting
* See what is the security that is required to connect to that system, v ##### HTTP Request (External System)
* Http Reqeust is use to call other web-services
 
