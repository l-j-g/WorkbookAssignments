# CCC T1A1: Workbook 
 Author: Lachlan Greve (012117)
 Date: 28/06/2021
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Assignment 1](#assignment-1)
    - [Question 1.](#question-1)
    - [Question 2.](#question-2)
    - [Question 3.](#question-3)
    - [Question 4.](#question-4)
    - [Question 5.](#question-5)
    - [Question 6.](#question-6)
    - [Question 7](#question-7)

<!-- markdown-toc end -->

## Question 1.

>**Research** the development of the internet from 1980 to today. You must **describe** at least FIVE key events in the development of the internet. You can refer to events, people of significance, or technologies and how they have changed over time.

1. Adoption of TCP/IP (1980): Transmission Control Protocol (TCP) and the Internet Protocol (IP) is a suite of technical standards that specifies and harmonises the way that data is sent and received over the internet. Prior to TCP/IP the use of different communication protocols made it difficult for systems on different networks to communicate with each other. Global adoption of the TCP/IP protocols between 1980 to 1990 established the framework for the internet that we know today. [^1]


[^1]: TCP/IP – Complete History of the TCP/IP Protocol Suite. (n.d.). History Computer. Retrieved June 20, 2021, from https://history-computer.com/tcp-ip-complete-history-of-the-tcp-ip-protocol-suite/

2. Browsers and the World Wide Web: Tim Berners-Lee created a proposal for what became the World Wide Web and developed the first web browser. Tim also wrote specifications for URIs, HTTP and HTML. These tools provided a platform where documents and other resources could easily be shared and accessed. These original tools remain in use today, only with added funcationality and features that have been added over time. [^2]

[^2]: Britannica, T. Editors of Encyclopaedia (2019, November 27). World Wide Web. Encyclopedia Britannica. https://www.britannica.com/topic/World-Wide-Web

3. Peer-to-peer file sharing (1999): Whilst peer-to-peer file sharing has existed from the conception of the internet the development of the application *Napster* fundamentally changed that way that users consumed media online. *Napster* was a file sharing application with a centralised server that became widely used to share multi-media (often pirated) files between users. In 2001 Napster was found liable for copywrite infringement and shutdown. Over time a variety of alternative services and technologies have been establish such as the Bittorrent protocol which facilitates direct peer-to-peer file transfer without the need for a centralised server that can be held liable for copywrite infringement. Online piracy and copywrite infringement over peer-to-peer networks remains as a major ethical issue that has not been resolved to this day.[^3] 

[^3]: Wikipedia contributors. (2021, April 24). Peer-to-peer file sharing. In Wikipedia, The Free Encyclopedia. Retrieved 09:51, June 28, 2021, from https://en.wikipedia.org/w/index.php?title=Peer-to-peer_file_sharing&oldid=1019635533

4. Mobile phones and the internet (1996+): The first mobile phones capable of connecting to the internet via remote cellular networks were launched in 1996. Over time rapid development has added increased functionality, increased, performance and reduction in cost. Modern mobile phones blur the lines in terms of capabilities between desktop computers and mobile devices. This has led to an exponential increase the adoption of mobile phones that are connected to the internet, which now account for the majority of internet activity in the world. [^4]

[^4]: Wikipedia contributors. (2021, June 17). History of mobile phones. In Wikipedia, The Free Encyclopedia. Retrieved 09:36, June 28, 2021, from https://en.wikipedia.org/w/index.php?title=History_of_mobile_phones&oldid=1029093651



5. Cloud Computing (~2008+): Relates to the remote delivery of computing services, typically over the internet. In recent times the availability of high-capacity networks and widespread adoption of hardware vitualization has led to a growth in cloud computing services. Cloud computing allows for the sharing of resources and can reduce IT infrastructure and maintenance costs. [^5]

[^5]: What is Cloud Computing. ITChronicles. (2021). Retrieved 28 June 2021, from https://itchronicles.com/what-is-cloud-computing/.

## Question 2.
>**Define** the features of the following technologies that are essential in terms of the development of the internet:
    * packets
    * IP addresses (IPv4 and IPv6)
    * routers and routing
    * domains and DNS
>   
>    **Explain** how each technology has contributed to the development of the internet.

**Packets**: A network packet is a formatted unit of data carried by a network. Each network packet includes information about the source and destination of the packet as well as data that is specific to the packet being transferred, known as the payload. Packets of data are generally small and are intended to ensure that data is transferred reliably and effectively. [^6]

[^6]: Christensson, P. (2016, September 21). Packet Definition . Retrieved 2021, May 22, from https://techterms.com


**IP addresses**: An ip address is a unique address that identifies a device on a network. It allows for a system to be recognised and distinguished between other systems on a network. IPv4 addresses consist of four sets of numbers ranging from 000.000.000.000 to 255.255.255.255, allowing for a total of 2^32 potential addresses. IPv4 can no longer provide enough addresses for all of the devices that are connected to the internet. IPv6 was developed to allow more devices to connect to the internet and consist of eight sets of four hexadecimal digits, allowing for maximum number of 2^128 unique addresses. [^6]

[^6]: Christensson, P. (2016, September 21). IP Address Definition. Retrieved 2021, May 22, from https://techterms.com

**Routers and Routing** Routers are an essential component of networking hardware that  connects computers and other devices to the internet by directing data from a local area network to another network connection. A router reads the network address information in the packet and ensures that it is sent / received to the appropriate destination.[^7] 

[^7]: Christensson, P. (2016, September 21). Router Definition. Retrieved 2021, May 22, from https://techterms.com

Domains and DNS: A domain name server (DNS) can be compared to an address book for websites. A DNS is a distributed database that allows browsers to connect human readable web addresses with the respective IP address where the website is hosted.[^8]

[^8]: Christensson, P. (2016, September 21). DNS Definition. Retrieved 2021, May 22, from https://techterms.com

## Question 3.

>**Define** the features of the following technologies that are essential in terms of the development of the internet:
    * TCP 
    * HTTP and HTTPS 
    * web browsers (requests, rendering and developer tools)
>    
>    **Explain** how each technology has contributed to the development of client and server communication over the internet 
    

**TCP:** The Transmission Control Protocol (TCP) is used to ensure reliable transmission of internet data packets. TCP separates data into smaller packets and identifies them with source and destination to allow for data to be transferred over the internet. Information within the header of TCP packets allows the data to be reassembled in the correct order and to check the integrity of the data that is sent and received. TCP allows for efficient and reliable transfer of data between client and server communication over the internet.[^9]

[^9]: Christensson, P. (2016, January 30). TCP Definition. Retrieved 2021, Jun 28, from https://techterms.com


**HTTP and HTTPS:** Hypertext transfer protocol (HTTP) is the network protocol invented by Tim Berners-Lee in the early 1990s. HTTP is a application layer protocol which allows for web browsers and server to communicate through the exchange of data. HTTP is not encrypted and is vulnerable to both man-in-the-middle and eavesdropping attacks. HTTPS is a more secure version of HTTP where the data that is transferred between a web browser and website is encrypted. HTTPS become more prevelent in 2016 and is now the most commonly used proctol used for web browsing. HTTPS allows for authentication, privacy and integrity and is particularly important for the transfer of sensitive data such as login details and personal data.[^10]

[^10]:Christensson, P. (2015, May 28). HTTP Definition. Retrieved 2021, Jun 28, from https://techterms.com

**Web Browsers:** The purpose of a web browser is to fetch content from hosted URLs on remote servers as requested by the user. Data received in the form of HTML documents is converted by a browsers rendering engine to display the content of the web page in an interactive visual repsentation on the users device. Web development tools are built-in to most modern web browsers and allow web developers to test and debug their code. Common tools include HTML and Document Object Model (DOM) viewers, profiling and auditing tools as well as JavaScript debuggers. [^11]

[^11]:Christensson, P. (2014, February 28). Web Browser Definition. Retrieved 2021, Jun 28, from https://techterms.com


## Question 4.

>**Identify** THREE data structures used in the Python programming language and **explain** the reasons for using each.

**Lists:** 

A list in python is a type of sequence, the most basic data structure in python. Lists are used to store data in a seqential manner. Any type of data may be stored within a list and a numerical index is applied to each item of a list, which is used to reference to the data stored in that element of the list. Lists are useful for grouping data together in a known order. 

- List items are *indexed*, with the first item starting from zero. 
- List items are *ordered*, the items of a list have a defined order and that order will not change.
- Lists are *mutable*, the items of a list can be changed, added or removed after it was been created. 
- Lists can have *duplicate* values, because each item of a lists has a different numerical index. 

The most common way to declare a list is to use square brackets. The Basic syntax for a list is as follows:[^12]

```
list = ['first', 'second', 'third']
list[1] # output is 'second'
```
[^12]: Python Lists. W3schools.com. (2021). Retrieved 28 June 2021, from https://www.w3schools.com/python/python_lists.asp.

**Tuples:**

Tuples are another type of sequence that consists of a number of values that are seperated by commas. 

Tuples are ordered, unchangeable and allows duplicates. Tuples are differentiated from lists because they are unchangable (immutable). Tuples have a fixed size because the order and content cannot change. This means that computational procedures with tuples are usually faster. Tuples should be used when the stored data should not be changed.

The most common way to declare a tuple is to use parenthesis. The basic syntax for a tuple is as follows: [^13]

```
tuple = (1,2,3,4)
tuple[1]
```
[^13]: Python Tuples. W3schools.com. (2021). Retrieved 28 June 2021, from https://www.w3schools.com/python/python_tuples.asp.

**Dictionaries:**

Unlike sequences, which are always indexed by a range of numbers, a dictionary stores objects in key:value pairs.  Objects are identified by a unique key that can be any immutable type including numbers and strings. A real world example of a python dictionary is a phone book, where someones name (unique key) is linked to an object or property (their phone number). A dictionary may hold multiple keys but only one value can be associated with each key.

Dictionaries are ordered, changeable and do not allow duplicate entries. 
The most common way to declare a dictionary is to use curly braces. The basic syntax for a dictionary is: [^14]

```
dict = { "key": object}  
print(dict[key])
```

[^14]: Python Dictionaries. W3schools.com. (2021). Retrieved 28 June 2021, from https://www.w3schools.com/python/python_dictionaries.asp.
https://docs.python.org/3/tutorial/datastructures.html

## Question 5.

>**Identify** TWO ways in which code is executed and **explain** how they are different.

Programming languages are designed for humans to be able to read and understand. Before programing languages can be executed by a computer, it must be converted into machine language (1's and 0's). The way that this is done depends on the type of programing language that the code is written in. There are two main ways that computer code is executed: 

1. Complied Languages (C, C++)
2. Interpreted Languages (Java, Python)

Compiled languages process source code through a compiler into machine code prior to execution. Compiled languages generally perform computational tasks much faster compared to interpreted languages because once compiled the code can be executed directly without any additional steps. Additionally, by producing a executable file written in machine code, the original source code is hidden which prevents people from seeing or copying the original source code. 

Interpreted languages convert source code line by line into machine code at execution. Interpreted languages offer increased portability as the source code does have to be compiled for a specific CPU architecture and allows for faster coding and development times as the source code does not need to be compiled each time before it is executed. [^15]

[^15]: Difference between Compiled and Interpreted Language - GeeksforGeeks. GeeksforGeeks. (2021). Retrieved 28 June 2021, from https://www.geeksforgeeks.org/difference-between-compiled-and-interpreted-language/#:~:text=A%20compiled%20language%20is%20a%20programming%20language%20whose%20implementations%20are,program%20into%20machine%2Dlanguage%20instructions.]
## Question 6.

>**Identify** TWO commonly used programming languages and **explain** the benefits and drawbacks of each.

Two commonly used programming languages are Python and C++. 

C++ is an object-orientated, statically typed, pre-compiled language. Variables defined in C++ must be declared as a specific data type and source code must conform to a specific syntax before it can be compiled and executed. C++ is commonly used in applications where performance is important such as embedded systems, large databases and game development. 

Python is a high-level interpreted programming language that was designed to be easy to read and understand. Python uses inbuilt indentation rules which helps to improve the readability of all source code. As an interpreted language python source code is not processed natively by the processor by rather line-by-line by an interpretor at time of execution. Python code is cross-compatible with different operating systems and does not need to be re-compiled for specific hardware or architecture. Python is now the most commonly used high-level programming language and is used for a variety of different purposes including, data analytics and application development.

Comparatively, code written in C++ generally takes more lines of code but provides faster execution speed and greater control of memory because the code has been statically defined and pre-compiled for execution. On the other hand, Python provides faster development time and greater cross-comparability. [^16]

[^16]: Difference between Compiled and Interpreted Language - GeeksforGeeks. GeeksforGeeks. (2021). Retrieved 28 June 2021, from https://www.geeksforgeeks.org/difference-between-compiled-and-interpreted-language/#:~:text=A%20compiled%20language%20is%20a%20programming%20language%20whose%20implementations%20are,program%20into%20machine%2Dlanguage%20instructions.


## Question 7
> **Identify**<span>&nbsp;TWO ethical issues from the areas below and **discuss** the extent to which an IT professional is ethically responsible in terms of the issue.
    List of topics containing ethical issues:
>  
>    * access to a user's personal information (medical, family, financial, personal attributes such as sexuality, religion, or beliefs)
>    * intellectual property, copyright, and acknowledgement.
>   * criminal acts such as theft, fraud, trafficking and distribution of prohibited substances, terrorism
>    * GPS tracking data and other types of metadata, MAC addresses, hardware fingerprints
>    * freedom of thought, conscience, speech and the media
>    * aggressive sales and marketing practices designed to mislead and deceive consumers
>    * trading of shares on the stock exchange OR crypto-currencies
>
>    For each ethical issue identify a source of legal information relating to the ethical issue and discuss whether the law is helpful in assisting a developer to act in an ethical way.
>
>    Conduct **research** into a case study of **ONE** of the ethical issues you have chosen **discuss** how an ethical IT professional should respond to the case study and how they might mitigate or prevent ethical breaches.
    
**Two Ethical Issues:**

1. The financial status of cryptocurrencies: Are cryptocurrencies currencies or investments?

Cryptocurrencies are a disruptive technology that traditional financial regulatory frameworks have struggled accommodate. Even though cryptocurrencies are traded in similar ways to traditional financial instruments (on digital exchanges and through initial public offerings), the Securities and Exchange Comission (SEC) and Commoditiy Futures Trading Commission's regulatory frameworks generally do not to cryptocurrencies. In 2017, the SEC chairman Jay Clayton issued a public statement warning of the financial risks associated with cryptocurrencies and the way that traditional security laws may not apply[^17]. The exemption of cryptocurrencies from security laws has led to various examples of unscrupulous developers that have stolen or manipulated investors assets. In the absence of a legal framework it is the responsibility for developers to act in an ethical way when developing new cryptocurrency applications. Further guidance in this regard has been provided by The Australia Securities & Investments Commission which published information sheet INFO 225 that provides guidance on the legal and ethical requirements needed for development of initial coin offerings and other crypto-assets.[^18]

[^18]: Information Sheet 225 (INFO 225) (Cth). Australian Securities and Investments Commission. https://asic.gov.au/regulatory-resources/digital-transformation/initial-coin-offerings-and-crypto-assets/

[^17]: U.S. Securities and Exchange Commission (11 Dec 2017), Statement on Cryptocurrencies and Initial Coin Offerings, Chairman Jay Clayton. https://www.sec.gov/news/public-statement/statement-clayton-2017-12-11

1. Targeted advertisement and personal data on social media sites:  

The proliferation of social media platforms like Facebook and Twitter has led to the emergence of an ethical issue that combines issues of access to user's personal information as well as targeted and aggressive advertisement. Regulation in this area is difficult as the commercial viability of major social media platforms depends on the use of user information. On the other hand, many users are unaware of what personal information is collected and what this information may be used for. The Australian Privacy Act 1988 was introduced to promote and protect the privacy of individuals. The act specifically defines key Australian Privacy Principles (APPs) that apply to the processing of personal data, individual rights in relation to the processing of their personal data and classification of what constitutes sensitive personal data.[^19][^20] Australian regulation and policy in this area assists developers in acting in an ethical way by clearly defining what is and what is not ethical behavior. 

[^19]: Privacy Act 1988 (Cth). https://www.legislation.gov.au/Details/C2018C00292
[^20]: Miralis, D., & Gibson, P. (2021). Data Protection 2020 | Laws and Regulations | Australia | ICLG. International Comparative Legal Guides International Business Reports. Retrieved 28 June 2021, from https://iclg.com/practice-areas/data-protection-laws-and-regulations/australia. 

**Case Study: *Facebook-Cambridge Analytica Data Scandal***

Social media platforms have unprecedented levels of access to user's personal information. Attention to this issue was escalated during the 2018 *Facebook-Cambridge Analytica* data scandal when whistleblower Christopher Wylie revealed that personal data of up to 87 million users of *Facebook* had been used by political consulting firm *Cambridge Analytica* to generate advanced targeted advertisements that were designed to manipulate political outcomes. This revelation came following accusations of interference in the unexpected election of Donald Trump and the United Kingdom's vote to leave the European Union and peaked the public interest in real-world implications of unethical personal data use. [^21] 

In response to this story an international political debate regarding the privacy rights of consumers online was sparked. Witness testimony before the United States Senate included expert testimony from Facebook CEO Mark Zuckerberg and concluded with the Federal Trade Commission charging Facebook with a fine of $5bn, for its violations of users privacy. Facebook responded by announcing plans to implement the EU's General Data Protection Regulation in all areas of operation and not just the EU. This event prompted major reform in many major tech companies including Apple, Facebook and Twitter. Transparancy around the use of personal data is now a prominent feature that can be found on these platforms many of which have had added features to download their own personal data from the platform and the option for users to clear all personal data from the site.[^20] 

The event of the Facebook-Cambridge Analytica Data Scandal were a catalyst to bring about change and awareness around the ethical use of personal data. In recent times large tech companies have tried to demonstrate responsible self-regulation in-order to prevent further restrictions being imposed by government agencies. The take away message for IT professionals in response to the Facebook-Cambridge Analytica data scandal is that developers must take the integrity and privacy of users personal data seriously. Best practice and regulatory guidelines have now been established through policy such as the EU's General Data Protection Regulation[^22] as well as within local jurisdictions such as the Australian Privacy Act[^19]. By ensuring that these requirements have been complied with and prioritising transparency with regard to users personal information, developers are able to find a balance between comercial viability and ethical use of personal data. 

[^20]: Nast, C. (2021). How Cambridge Analytica Sparked the Great Privacy Awakening. Wired. Retrieved 28 June 2021, from https://www.wired.com/story/cambridge-analytica-facebook-privacy-awakening/.
[https://www.wired.com/story/cambridge-analytica-facebook-privacy-awakening/]
[^21]: Wikipedia contributors. (2021, June 18). Facebook–Cambridge Analytica data scandal. In Wikipedia, The Free Encyclopedia. Retrieved 10:49, June 28, 2021, from https://en.wikipedia.org/w/index.php?title=Facebook%E2%80%93Cambridge_Analytica_data_scandal&oldid=1029165846
[^22]: Reform of EU data protection rules - European Commission. Ec.europa.eu. (2016). Retrieved 25 March 2016, from http://ec.europa.eu/justice/data-protection/reform/index_en.htm.






