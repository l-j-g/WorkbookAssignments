# Written Report/Proposal - Research and Improve an Application Stack 

## Brief





--- 
    * Provide an Application Stack Diagram for one product or service of the application you are considering.

![Application Stack Diagram for eBay](./Ebay_ASD.svg)

Figure 1: *Application Stack Diagram for eBay*

---

    * Mark down which technologies fall into:
      * The Presentation Layer of the stack
      * The Application Layer of the stack
      * The Data Access Layer of the stack

In order to prioritise latency and scalability of their platform the eBay application stack utilises Java for the backend and Javascript for the frontend. This technology stack allows eBay developers to streamline development and prioritise latency and scalability.

 **Presentation Layer:**
 
- Javascript: A client side programing language for the presentation layer that can update and change both HTML and CSS.

- Marko: Marko is an open-source HTML rendering and templating engine that was designed by eBay.

**Application Layer:**

- Node.js: A Java(script) Runtime Environment (JRE), that is used to execute Javascript code at the application layer. 

- Apache Tomcat: Is a Java based webserver that uses concurrent execution threads and provides clustering and load balancing capabilities 

**Data Access Layer**

- Oracle RDS: Java based RDS databases from Oracle are used to store and process ordered transactions where reliability, consistency and availability a priority - such as user login details and auction bid orders.

- Cassandra: Java based NoSQL distributed databases are used for processing large datasets at high speed. Data stored in these databases are accessed by time critical processes such as search queries.

- Hadoop: Java based database format for storage and processing of big data that is highly scalable, cost effective, fast and resistant to failure.

---
>* Pick three technologies for each
>   * describe in a short paragraph its role in the stack and how it relates to its neighbouring technologies.

1. Marko: Marko is a component in the presentation layer that can render HTML from Javascript. As a response to a client side request is received from the application layer through the node.js runtime, the received data is dynamically rendered by the Marko engine. The Marko engine takes advantage of the data streaming capabilities of the node.js by rendering pages asynchronously as the data of the page is streamed to the client.  This functionality is advantageous for applications with high-scale traffic because hardware infrastructure is used more efficiently with less downtime spent waiting for partial or incomplete processes. For the client this also improves user experience by providing a low latency and more responsive website.

2. Node.js: Is an application layer Java runtime environment that allows the use of Javascript as the development language in both the client and server side of an applications architecture - for an enterprise this improves the efficiency and performance of applications whilst reducing development and maintenance costs. Node.js provides the backbone of the eBay architechture by processing client requests and passing them to templating and webserver architechture to request the necessary resources to serve the request.  Node.js utilise single thread processing with non-blocking asynchronous operations, when enables high performance, low latency operation.

3. Apache Tomcat: Is a Java based webserver that creates containerized instances of web applications that can scale horizontally and operate independently. When requests for data are received from node.js, Tomcat will distribute the request across its containerized applications and make requests for the necessary data from the data access layer. Tomcat serves as an interface (known as middleware) between eBays application layer (Javascript) and data access layer (primarily Java). Because Tomcat can scale horizontally with containerized clusters, the single thread limitations of node.js can be overcome, providing a highly scalable solution that is optimised for performance high amounts of traffic with low latency.

>* Pick two technologies and for each:
>   * Discuss what physical hardware this technology is most likely delivered on. 
>   * Include a table comparing its features and benefits to similar alternative technologies. 



>* Examine the application’s developer API and:
>   * Describe TWO processes for the input and output of data based on the company's API and how they achieve organisational objectives.


**eBay API's**

The eBay developer API are all RESTful. RESTful API's allow a developers program to communicate directly with the service providers technology stack using standardised HTTP methods (GET, POST, PUT and, DELETE) that provide full Create, Retrieve, Update and Delete (CRUD) capabilities. 

eBay provide seperate developer API's for user features such as: Sell API, Buy API, Commerce API and Analytics API. The following two procceses are facilitated through eBays Sell API:

**1. Matching inventory to catalog products**

For sellers wanting to list items for sale, eBay provide a catalog of item listings templates for various categories of different products. The eBay product catalog allows sellers to quickly create or revise product sale listings. 

Each product in the catalog is uniquely identified by a eBay product ID (ePID) that is provided by the item seller. Alternatively, many products can be identified by common industry standard product indentifiers such as UPC, EAN, ISBN or brand / manufacture part number(s) (MPN).

For each item that can be found in the eBay catalog the following fields can be returned:

- Product title
- Product identifier(s)
- Product aspects (aka "item specifics")
- Stock photo(s) (not available for every catalog product)
- Product Category (incl. required category specific product aspects e.g. brand, operating system, color, storage capacity.)

The process of matching sellings inventory to catalog products achieves organisational objectives by automating the processes of listing items for sale.  Sellers who automate the listing of their products by matching inventory to catalog products reduce the amount of manual data entry needed and create more consistent and reliable listings which increases the overall efficiency of the platform. By aligning their products with pre-existing templates sellers are more likely to use common terminology to describe their prducts - for example: a 'red' mobile phone could also be listed as 'scarlet', 'crimson' or 'ruby' in appearance, the eBay product catalog assists sellers in selecting the appropriate color description for their product which in turn help connect more buyers with the products that they are looking for. 

The process also provides tools that assist sellers in aligning 

statistical analysis 

Inventory API > call to createOrReplaceInventory > product.epid field

Category API >  call to search > query paramameters (q, gtin and/or mpn)


**Marketing Seller Inventory**

eBay assist sellers in marketing their inventory by providing the Negotiation and Marketing API.

The Negotiation API allows sellers to discover buyers who are interested in their products (who have have added the sellers products to their Watch list or shopping card).

The Marketing API allows sellers to attract buyers to their items by creating Promoted Listings ad campaigns and discount promotion with the Promotions Manager

https://developer.ebay.com/api-docs/sell/static/marketing/promoted-listings.html

Describe the Fields you need - JSON, Key Values Pairs. 
Listing an Item for Sale: 

The Inventory API is used to create and mange offers on eBay marketplaces. In order to create a listing on thjThe major components of this API include:

- Location: The sellers inventory location must be registered with the API.
- Inventory Item: An inventory record that details; a seller-defined SKU, product details (description, title, images), quantity avalibile, means of delivery and product condition.


The following processes are derived specifically from t

    * Describe the functions of the API that facilitate your chosen feature or service





    * Create an entity relationship diagram to depict the database tables that you believe are likely to be employed by the system you are investigating in order to provide your chosen service or product. You are free to speculate on the properties of entities and the relationships between entities.
    * Supplementary to this diagram, suggest a way in which these entities might be altered in order to add an extra piece of functionality to the product or service. Explain how you think this would improve the service.
        * Explain what technologies or app functionality would need to be added to support this. Would this be difficult or expensive to implement?
        * Create a modified entity relationship diagram that depicts your planned change.