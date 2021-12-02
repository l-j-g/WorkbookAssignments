# Written Report/Proposal - Research and Improve an Application Stack 

## Brief



* Provide and Application Stack Diagram for one product or service of the application you are considering. 

    * Mark down which technologies fall into:
        *  The Presentation Layer of the stack 
        *  The Application Layer of the stack
        *  The Data Access Layer of the stack
    * Pick three technologies for each
        * describe in a short paragraph its role in the stack and how it relates to its neighbouring technologies.
    * Pick two technologies and for each:
        * Discuss what physical hardware this technology is most likely delivered on. 
        * Include a table comparing its features and benefits to similar alternative technologies. 

---


![Application Stack Diagram for Ebay](Ebay.ASD.drawio.svg)
Figure 1: Application Stack Diagram for Ebay

The application stack of Ebay strongly based on Java and Javascript, utilising a partial J2EE technology stack in order to streamline development and prioritise latency and scalability.

What is this technology doing and how does it relate. 

Marko is a package that is used for rendering HTML views for clients. Marko is an open-source project 


Node JS is a Java(script) Runtime Environment (JRE), that is used to execute Javacript code at the application layer. `

 **Presentation Layer:**
 
- Javascript 


- Marko: Marko is an open-source HTML Rendering, templating engine that was designed by Ebay. It operates in conjunction with functionality of node.js to allow progressive rendering of pages that update the view to the client as the data for the page is received. 

**Application Layer:**

- Node.js

- Apache Tomcat

**Data Access Layer**

- Oracle RDS: RDS databases from Oracle are used to store and process ordered transactions where reliability, consistency and availability a priority - such as user login details and auction bid orders.

- Cassandra: NoSQL distributed databases are used for processing large datasets at high speed. Data stored in these databases are accessed by time critical processes such as search queries.

- Hadoop: Non time-critical, processing of historical big data is preformed offline on hadoop databases to preform process such as data analytics and machine learning optimization.



* Examine the application’s developer API and:

    * Describe TWO processes for the input and output of data based on the company's API and how they achieve organisational objectives.
---


    * Describe the functions of the API that facilitate your chosen feature or service

    * Create an entity relationship diagram to depict the database tables that you believe are likely to be employed by the system you are investigating in order to provide your chosen service or product. You are free to speculate on the properties of entities and the relationships between entities.
    * Supplementary to this diagram, suggest a way in which these entities might be altered in order to add an extra piece of functionality to the product or service. Explain how you think this would improve the service.
        * Explain what technologies or app functionality would need to be added to support this. Would this be difficult or expensive to implement?
        * Create a modified entity relationship diagram that depicts your planned change.
        
REST stands for REpresentational State Transfer, which probably doesn't help you that much in understanding what it is. Pragmatically, it means that you or your program communicates with a remotely-run service using standard web commands and protocols such as HTTP requests and responses. You send the service an API command wrapped in an HTTP request, and it responds with a success or failure indicator and any results data, all wrapped in an HTTP response.

This means the REST API itself is stateless. State is maintained on either the client side or the service side, but not within the API. Thus the full name; Representational State Transfer. REST APIs transfer state from client to server or vice versa.

REST architecture emphasizes that interactions between clients and services are enhanced by having a limited number of operations with which it acts. Specifically, there are four common HTTP methods that give you full "CRUD" capabilities: Create, Retrieve, Update, and Delete. Each of the main HTTP methods (GET, POST, PUT, and DELETE) has a specific meaning in the REST architecture, and in this way REST avoids ambiguity. You can think of the HTTP methods as the verbs in a rest operation.

Follows the OpenAPI specification, generates APIs in multiple programing langauges including; Javascript, Java and Python, Bash, Ruby ect.
