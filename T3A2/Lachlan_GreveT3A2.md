# Written Report/Proposal - Research and Improve an Application Stack 

## Brief




    * Pick three technologies for each
        * describe in a short paragraph its role in the stack and how it relates to its neighbouring technologies.
    * Pick two technologies and for each:
        * Discuss what physical hardware this technology is most likely delivered on. 
        * Include a table comparing its features and benefits to similar alternative technologies. 

---

* Provide an Application Stack Diagram for one product or service of the application you are considering. 

![Application Stack Diagram for eBay](./Ebay_ASD.svg)

Figure 1: Application Stack Diagram for eBay

* Mark down which technologies fall into:
  * The Presentation Layer of the stack
  * The Application Layer of the stack
  * The Data Access Layer of the stack

The application stack of eBay strongly based on Java and Javascript, utilising a partial Enterprise Edition of the Java technology stack in order to streamline development and prioritise latency and scalability.




Node JS is a Java(script) Runtime Environment (JRE), that is used to execute Javacript code at the application layer. `

 **Presentation Layer:**
 
- Javascript: Is a programing for the presentation layer that can update and change both HTML and CSS.


- Marko: Marko is an open-source HTML Rendering, templating engine that was designed by eBay. It operates in conjunction with functionality of node.js to allow progressive rendering of pages that update the view to the client as the data for the page is received. 

Marko is a package that is used for rendering HTML views for clients. Marko is an open-source project 
**Application Layer:**

- Node.js

- Apache Tomcat

**Data Access Layer**

- Oracle RDS: RDS databases from Oracle are used to store and process ordered transactions where reliability, consistency and availability a priority - such as user login details and auction bid orders.

- Cassandra: NoSQL distributed databases are used for processing large datasets at high speed. Data stored in these databases are accessed by time critical processes such as search queries.

- Hadoop: Non time-critical, processing of historical big data is preformed offline on hadoop databases to preform process such as data analytics and machine learning optimization.



* Examine the application’s developer API and:
    * Describe TWO processes for the input and output of data based on the company's API and how they achieve organisational objectives.
    * Create an entity relationship diagram to depict the database tables that you believe are likely to be employed by the system you are investigating in order to provide your chosen service or product. You are free to speculate on the properties of entities and the relationships between entities.
    * Supplementary to this diagram, suggest a way in which these entities might be altered in order to add an extra piece of functionality to the product or service. Explain how you think this would improve the service.
        * Explain what technologies or app functionality would need to be added to support this. Would this be difficult or expensive to implement?
        * Create a modified entity relationship diagram that depicts your planned change.

**eBay Sell API**

The eBay developer API are all RESTful. RESTful API's allow a developers program to communicate directly with the service providers technology stack using standardised commands through HTTP method (GET, POST, PUT and, DELETE) requests and responses.

eBay provide seperate developer API's for user features such as: Sell API, Buy API, Commerce API and Analytics API.

Before 

1. Getting category information and other metadata:



The following processes are derived specifically from t

    * Describe the functions of the API that facilitate your chosen feature or service



Follows the OpenAPI specification, generates APIs in multiple programing langauges including; Javascript, Java and Python, Bash, Ruby ect.

        
