# CCC T4A1 - Developer Workbook 
## Author: Lachlan Greve
## Date: 06/02/2022

| No. | Questions                                                                                                                                                                                                           |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
D | Q1  | Provide an overview and description of a standard source control process for a large project.                                                                                                                       |
D | Q2  | What are the most important aspects of quality software?                                                                                                                                                            |
T | Q3  | Outline a standard high level structure for a full-stack application and explain the components.                                                                                                                    |
T | Q4  | A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?                                                       |
D | Q5  | With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges.                                                                    |
D | Q6  | With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature.                    |
D | Q7  | Explain control flow, using an example from a suitable programming language.                                                                                                                                        |
 D | Q8  | Explain type coercion, using examples from a suitable programming language.                                                                                                                                         |
D | Q9  | Explain data types, using examples from a suitable programming language.                                                                                                                                            |
D | Q10 | Explain how arrays can be manipulated, using examples from a suitable programming language.                                                                                                                         |
D | Q11 | Explain how objects can be manipulated, using examples from a suitable programming language                                                                                                                         |
D | Q12 | Explain how JSON can be manipulated, using examples from a suitable programming language                                                                                                                            |
D | Q13 | For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes |

# Q1

Source control management processes allow software developers to track code changes, monitor revisions and to revert changes back to previous versions when needed. The `Git` software package was originally developed by Linux Torvalds in 2005 and is now ubiquitous with modern day source control development for both small and large size projects.

A large organisation or project will often implement a specific git workflow that standardises project source control processes around conditions for branching and merging strategies, repository structure, repository ownership and access across the organization.

A common modern git workflow is called Trunk-based development (TBD). In Trunk-based development, all developers integrate their changes into a shared branch which is maintained in a production ready state on a daily basis. The benefit of this approach is that it forces developers to consider how their changes will interact with changes made by other developers working on the project.

When implementing changes or features that are too large to be completed in a single day, a technique called 'branch by abstraction' is commonly used. When branching by abstraction, a boolean logic point is utilised to switch between default and development behaviour. As the new functionality is developed, the default functionality of the application can remain unchanged. Once development of the new component is complete the programs logic is switched to utilise the component and the old component can be removed.

By forcing developers to regularly integrate their changes with a production ready code base Trunk-based development encourages collaboration between team members and is is most closely aligned with Continuous Integration / Continuous Development and DevOps best practices.

# Q2: 
https://www.silasreinagel.com/blog/2016/11/15/the-seven-aspects-of-software-quality/

The seven aspects of software quality was described by Silas Reinagel and can be summarised as follows: 

1. Reliability: Execution should be consistent and without error.
2. Understandability: Source code should be logical in structure and well organized.
3. Modifiability: Components should be loosely coupled and allow for extension in functionality.  
4. Usability: User interaction should be as simple as possible and achieve functionality with minimal configuration.
5. Testability: Functionality should be verified for all use cases.
6. Portability: Software that is operating system, hardware and deployment agnostic.
7. Efficency: Function is achieved with the least amount of resources as possible.

# Q3: 

At a high level a full stack application can be considered in three separate layers:

The 'front-end' or presentation layer of an application displays content to and interacts directly with the user. This layer defines the 'look and feel' and is typically built using a combination of HTML, CSS and JavaScript.

The 'back-end' or logic/application layer of an application processes data and interacts with the front-end layer. This layer defines the 'logic' and is typically built using a combination application frameworks written in JavaScript, C++, Python or other languages.

The data layer of an application processes data and interacts with the back-end layer. This layer defines how the data of the application is stored and is typically built using a combination of relational databases, NoSQL databases and other data stores.  

# Q4
| Q4  | A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?                                                       |

Some of the knowledge and skills needed to develop a website for a small business would include:

- Front End Design: 
The front end design is the visual design of the website. The team will need to design the and the look and feel of the website, to do this the team will need to create a development plant through consultation with the client the client to discuss their requirements and then using a design tool to create wireframes before the development of the website begins. The front end developers will be required to write code in HTML, CSS and JavaScript and may require graphic design skills to create a logo and other visual elements.

- Backend Design:
The backend design is the logic of the website. Depending on the requirements of the client little to no backend design may be required (i.e if the website serves only static content). If the requirements are more complex, the team will need no decide on a suitable web framework to use.

A web framework is a set of libraries and tools are used to build a website. A web framework is generally capable of dynamically rendering content based on the model-view-controller (MVC) pattern which modularizes code and allows for dynamic content to be rendered based on provided templates and data.

Backend Design frameworks are commonly written in JavaScript, C++, Python or other languages - popular frameworks that are currently used to develop websites include: Flask, React and Express. 

- Database Design: 

Depending on the requirements of the company, the website may also require a database to store the data. The team will need to select an appropriate database architechture for the requirements of the website, it is common that a SQL RDMS (Relational Database Management System) is database management system that is used to store and retrieve data to support various types of websites.

- Deployment: The team will need to determine how the website will be deployed and where it will be hosted. Do they need to use a hosting service such as Amazon Web Services (AWS) or a local server. 

- Maintenance: After delivery the website the team will need to determine how on-going maintenance, updating and reporting of the website be handled. Does the business have technically capable people of fulfilling this task or can the team offer a service to do this. 

# Q5

For CCC-2021 T3A3, I was required to deliver a full stack web application that included a data layer, application layer and a basic presentation layer. My project was an application that serves as an interface to a database of financial data for companies listed on the Australian Stock Exchange. The skills and knowledge required to deliver the project included:

- A working technical knowledge of the Python based web development framework and associated tools that was used.  
- An understanding of relational databases to create various database tables, relationships and queries.
- HTML and CSS knowledge to develop templated web pages that would display content based on information retrieved from a database.
- A technical understanding required to address security, data integrity as well as ethical, professional and legal concerns.

Some of the challenges that I encountered during the development of this project included:

- Limited amount of time: the project had to be delivered within a two-week time period. 
- Technical knowledge: This was the first time that I attempted to develop a full stack application and required me to learn how to properly use and debug the packages utilised as a part of the technology stack. 
- Incomplete data: The data used in the database was sourced from Yahoo Finance using public APIs. However, the data for each company was not complete and to be addressed properly required me to add error handling when expected data was not avalible. Due to time constraints, I was unable to implement this feature and instead limited the amount of data that was included in the database.  

Some of the skills I applied to address these challenges included:

- Problem solving: When encountering various issues throughout development, I applied problem solving skills to debug technical issues i encountered. This involved utilising resources that were available to me such as: reading documentation, searching online and consulting my peers / mentors.  
- Time management: I was able to complete the project on time by planning what features I wanted to implement and creating a development plan which outlined that needed to be done to deliver the project.

# Q6

With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature.                    |

The project I was assigned to was a web application that was used to manage a database of financial data for companies listed on the Australian Stock Exchange. The skills and knowledge that I required to develop the project were learnt in about 4-5 weeks prior to starting the project. Given that the project was completed within two weeks, I was able to apply my knowledge and skills in reasonably effective manor.

However, in was not able to implement all of the features that I had originally planned or aspired to implement in the project. Some of the features that I wanted to implement to improve the project were:

- Plan and organise the scope of the project better from the outset so that I could better understand what was required to be done to complete the project.
- An improved user interface that would be more visually appealing for the user.
- Better error handling and integrity checking, as well as handling these errors more gracefully when they occurred.
- Implement automated testing as a part of a CI/CD development pipeline to ensure that the application is working as expected.
- Add a feature to allow advanced queries and filters to be applied to the data, such as sorting listed companies by specific criteria such as market cap or sector. 
- Expand the scope of the application to include additional financial data about listed companies such as cash flow statements, balance sheets, income statements, and more. 
- Add functionality to visualise the data contained in the database through graphs and charts. 
- Expand the number of companies data that is included in the database and add pagination the the data displayed to the user. 


# Q7

A programs control flow is the order in which the program's source code is executed. All modern programming languages make use of three primary control flow types: sequential, selection and repetition. [^1]

1. Sequential Control:

Sequential control flow simply executes code in the order that it is written. In Python, as an interpreted languages, this is the default behaviour.  The following code snippet is an example of sequential control flow in Python:[^2]

``` python
n = 5 # The variable n is set to the value 5.
print(f"{n} is five") # >>> "5 is five"
n = 3 # The variable n is set to the value 3.
print(f"{n} is three") # >>> "3 is three"
```

2. Selection Control:

Selection control flow represents a decision making process. These statements can add a lot of functionality to code by allowing programs to interpret logic and respond conditionally.

The structure of a Selection control flow consists of a conditional statement that can be evaluated in boolean as either True or False. The code that is executed next depends on the result the evaluation.

In Python an example of the selection control flow is the `if` statement. The below following code snippet is an example of selection control flow in Python:[^2]

``` python
n = 5
if n % 2 == 0:
   print(f"{n} is even")
else:
   print(f"{n} is odd")
```

In this example, the conditional statement is defined as `n % 2 == 0`. This statement will evaluate as `True` if the variable `n` is an even number, when this occurs the indented code block will be executed.

Use of the optional `else` keyword is also demonstrated in the above example. This allows us to define which code to be executed if the conditional statement is evaluated as `False`. Upon evaluation, as `n` is defined as the odd number five, the first code block following the conditional statement will be skipped and instead the code block contained within the `else` statement is executed.

3. Repetition Control Flow

Repetition statements are known as loops and are used to repeatedly execute a block of code until a defining condition evaluates as False. 

Python has two types of loops: `for` and `while`. The difference between the two is that the `for` loop is used to iterate over a sequence of items while the `while` loop is used to iterate over an indefinite number of times. 

Repeitition control flow in Python also utilises the `break` and `continue` keywords. The `break` keyword is used to terminate the loop and the `continue` keyword is used to skip the current iteration and continue with the next iteration.

# Q8


Type coercion is the automatic or implied conversion of objects from one data type to another. It is generally used when two variables of different data types are required to operate with each other.

Type *coercion* is an implicit change in object type whilst type *conversion* can be either implicit or explicit. Technically, the Python programming language does not support type coercion but is capable of implicit type conversion in situations that will not result in data loss.[^3]

For example: Python fully supports arithmetic calculations between 'mixed' numerical data types. When a binary arithmetic operator has operands of different numeric types, the operand with the 'narrower' type is 'widened' to that of the other.[^4]

This is demonstrated in the code snippet below:

```python
x = 2 # x is of type 'int'
y = 5.5 # y is of type 'float'
z = x + y  # results in z = 5.5 (float)
```

Although int `x` and float `y` are added together without error, no type coercion occurs.

In order of execution, when python sees `x + y` it calls the `__add__` method on `x`, passing `y` :

    >>> x.__add__(y)
    NotImplemented

The result, `NotImplemented` occurs because Python can not add type `int` to type `float` without data loss. However, when Python receives the `NotImplemented` value it automatically reverses the expression with:

    >>> y.__radd__(x)
    5.5

Because the object of type float can operate with type int without data loss, the operation is completed. 

In other cases, such as `string` operations, Python is not able to manipulate objects of different data types that will result in data loss.

This is demonstrated in the following code snippet below:

```python
x = 2 # x is of type 'int'
s = "Pizza" # s is of type 'string'
y = x + s # >>> "TypeError: can only concatenate str (not "int") to str"
```

Trying to add int `x` to type string `s` results in an error because they are of different data types. For the addition to succeed we need to first explicitly convert `x` to type string. [^5]

```python
x = 2 # x is of type 'int'
s = "Pizza" # s is of type 'string'
y = str(x) + s # y = '2Pizza'
```

# Q9

All popular modern programming languages allow variables to be stored as different data types. 

In the Python programming languages, the built-in data types are: 

- Numerics: int, float, complex
- Sequences: list, tuple, range
- Mappings: dict

In Python the type of a variable can be determined using the built-in `type()` method. Any object 

**Numerics:**

Python has three numeric types: int, float and complex. Integers in Python has unlimited size and can be represented by any number of bits. Floats are represented by a single-precision floating-point number. Complex numbers are represented by a pair of numbers, one real and one imaginary.

Python fully supports arithmetic calculations between 'mixed' numerical data types. When a binary arithmetic operator has operands of different numeric types, the operand with the 'narrower' type is 'widened' to that of the other.[^4]

``` python
x = 2 # x is of type 'int'
y = 5.5 # y is of type 'float'
z = x + y  # results in z = 5.5 (float)
```

**Sequences:** 

A list in python is a type of sequence, the most basic data structure in python. Lists are used to store data in a sequential manner. Any type of data may be stored within a list and a numerical index is applied to each item of a list, which is used to reference to the data stored in that element of the list. Lists are useful for grouping data together in a known order. 

- List items are *indexed*, with the first item starting from zero. 
- List items are *ordered*, the items of a list have a defined order and that order will not change.
- Lists are *mutable*, the items of a list can be changed, added or removed after it was been created. 
- Lists can have *duplicate* values, because each item of a lists has a different numerical index. 

``` python
list = ['first', 'second', 'third']
list[1] # output is 'second'
```

**Dictionaries:**

Unlike sequences, which are always indexed by a range of numbers, a dictionary stores objects in key:value pairs.  Objects are identified by a unique key that can be any immutable type including numbers and strings. A real world example of a python dictionary is a phone book, where someone's name (unique key) is linked to an object or property (their phone number). A dictionary may hold multiple keys but only one value can be associated with each key.

Dictionaries are ordered, changeable and do not allow duplicate entries. 
The most common way to declare a dictionary is to use curly braces. The basic syntax for a dictionary is: [^14]

``` python
dict = { "key": object}  
print(dict[key])
```

# Q10

The closest built-in data type to arrays that Python includes are called Sequences. Python natively supports three types of Sequences: lists, tuple and range.

A python list is the most basic data structure in python. Lists are used to store data in a sequential manner. Any type of data may be stored within a list and a numerical index is applied to each item of a list, which is used to reference to the data stored in that element of the list. Lists are useful for grouping data together in a known order.

- List items are *indexed*, with the first item starting from zero. 
- List items are *ordered*, the items of a list have a defined order and that order will not change.
- Lists are *mutable*, the items of a list can be changed, added or removed after it was been created.
- Lists can have *duplicate* values, because each item of a lists has a different numerical index.

tuples are the same as lists but are *unmutable*. ranges are similar to tuples (also *unmuatable*) but take up a very small amount of memory - regardless of the range of numbers the sequence describes. 

Additional native support for traditional (C type) arrays is provided as `ndarray`'s in the `NumPy` package.

Creation and manipulation of Python lists is demonstrated in the example below:

```python
# create a list of length 5 containing the letters a-e
myList = ['a','b', 'c', 'd', 'e']
# print the first letter of the list -> 'a'
print(myList[0]) 
# assign the first element of the list to be 'first'
myList[0]='first'
# print the list > ['first', 'b', 'c', 'd', 'e']
print(myList) 
```

A Python list has the following built-in methods which are described below:

| Method    | Description                                                                  |
| --------- | ---------------------------------------------------------------------------- |
| append()  | Adds an element at the end of the list                                       |
| clear()   | Removes all the elements from the list                                       |
| copy()    | Returns a copy of the list                                                   |
| count()   | Returns the number of elements with the specified value                      |
| extend()  | Add the elements of a list (or any iterable), to the end of the current list |
| index()   | Returns the index of the first element with the specified value              |
| insert()  | Adds an element at the specified position                                    |
| pop()     | Removes the element at the specified position                                |
| remove()  | Removes the first item with the specified value                              |
| reverse() | Reverses the order of the list                                               |
| sort()    | Sorts the list                                                               |

# Q11 

Python is an object oriented programming language where almost all variables in Python can be considered as objects called classes. Classes combine data and functionality together and provides instructions of how to create new instances of that class. All Python `Classes` can have both `attributes` and `methods`.

+ A variable stored in an instance or class is called an attribute.
+ A function stored in an instance class is called a method.

Note: All methods are attributes, but not all attributes are methods.

The methods and attributes of a class are accessed and manipulated using dot notation. For example:

```python
# create an int object called 'number' with the value 4. 
number = int(4)
# call the __dir__() method of the int class
# returns all defined attributes of the class 
number.__dir__()
```

Class attributes can exist as either `Class Attributes` or `Instance Attributes`.

A `Class Attribute` is an attribute that is shared by all instances of the class.
A `Instance Attribute` is an attribute that is specific that the particular instance of the class.

The effect of this is demonstrated in the following code snippet:

```python

# define a new class 
class myClass():

    # set value of ClassAttribute to 1 
    ClassAttribute = 1

    # the init method is used to initialize the value of instance attributes 
    def __init__(self,data="Default Value"):
        # set the value of InstanceAttribute to the value provided during the initialisation of the class 
        self.InstanceAttribute = data
    
# create testClass with InstanceAttribute value of 'test'
testClass = myClass('test')
# create testClass with InstanceAttribute value of 'another test'
testClass2 = myClass('another test')

# >> 1
print(testClass.ClassAttribute)
# >> 'test'
print(testClass.InstanceAttribute)

# >> 1
print(testClass2.ClassAttribute)
# >> 'another_test'
print(testClass2.InstanceAttribute)
# The value of the ClassAttribute is shared across both instances
# The value of the InstanceAttribute is defined during initialisation of the instance. 
```

https://www.toptal.com/python/python-class-attributes-an-overly-thorough-guide

# Q12 

JavaScript Object Notation (JSON) is the most common format of information exchange and communication between applications. To manipulate JSON objects in Python a developer needs to be able to encode (write) and decode (read). The Python programming languages comes with built-in native support for encoding and decoding JSON data.

To add JSON support to a program written in python a developer needs to add an `import json` statement to the top of their program. The json package allows for either encoding or decoding between native Python objects and JSON formatted data files. Using the `dump()`

The `dump(input, output)` method writes (encodes) the given Python input object as a JSON file. Likewise, the `load(input)` reads (decodes) the given JSON file and translates it into a native Python object.

Python objects are translated into JSON data according to the following table:

| Python         | Java   |
| -------------- | ------ |
| dict           | object |
| list, tuple    | array  |
| str            | string |
| int,long,float | number |
| True           | true   |
| False          | false  |
| None           | null   |

Alternatively, if the the `dumps()` or `loads()` methods are used the input will be decoded / encodes as strings as opposed to native filetypes. i.e `loads()` decode a JSON object into a Python dictionary of strings, regardless of the data type.

An example of reading and writing to JSON files in Python is included below: 

```python
# import the json package 
import json

# Create a Python list of strings
cat_names = ["Garfield", "Felix", "Jerry"]

# Use Python context manager to write cat_names.json
with open("cat_names.json", 'w') as write_file:
    # encode the cat_names object to JSON format
    json.dump(cat_names, write_file)

# Use Python context manager to read cat_names.json
with open("cat_names.json", 'r') as read_file:
    # decode the cat_names object as a Python object
    cat_names = json.load(read_file)

```

# Q13

```python
# import the definitions from Pythons 'random' module package
import random

# create a class of car objects 
class Car:
    """
    A python class to represent the brand of car someone owns 

    Attributes 
    ----------
    car_name : str
        brand of the car
    
    Methods
    -------
    present():
        Prints a statement declaring the brand of car a person has
    """
    # constructor method
    def __init__(self, brand):
        '''Function that constructs all of the necessary attributes of car object'''
        self.car_name = brand

    # define a present method
    # for printing the the brand of car a person has
    def present(self):
        '''Function that prints a statement declaring the brand of a car a person has'''
        return 'I have a ' + self.car_name

# create a class of model objects as a child of car objects
# inherits methods and properties from the parent (car) class  
class Model(Car):
    '''
    A python class to represent the model of car someone owns
    
    Attributes 
    ----------
    car_name : str
        brand of the car
    
    Methods
    -------
    present():
        Prints a statement declaring the brand of car a person has
    '''

    # constructor method
    def __init__(self, brand, mod):
        # access the init method from the class parent class (car)
        super().__init__(brand)
        self.model = mod

    # define a show method for printing the brand of the car and the year that it was made
    def show(self):
        return self.present() + ', it was made in ' + str(self.model)

#  create a list of strings called `makes`, of different manufacturers of cars
makes = ["Ford", "Holden", "Toyota"]
# create an empty list called `models`, to hold the year (int) which a car was made
models = []
# for loop to populate the models list with a range of numbers between 1980 to 2020
for i in range(40):
    models.append(i+1980)

# function to select a random number between from the range of min to max
def random_int_from_interval(min,max):
    return random.randint(min, max)

# for loop which will 
# pick a random make of car from the makes list
# pick a random year of manufacture from the list of models 
# create a Model object using the randomly selected make and model
for model in models:
    # pick a random make of car from the list of makes 
    make = makes[random_int_from_interval(0, len(makes)-1)]
    # pick a random year of manufacture between 1980 to 2020 from the list of models
    model = models[random_int_from_interval(0, len(makes)-1)]
    # creates a new Model class using a randomised make and model 
    my_car = Model(make, model)
    # Print a statement to declare brand of the car and the year that it was made
    print(my_car.show())
```

# Bibliography 

[^3]: Smith, Kurt W.. Cython: A Guide for Python Programmers. United States, O'Reilly Media, 2015.
[^4]: "Built-In Types — Python 3.9.7 Documentation". 2021. Docs.Python.Org. https://docs.python.org/3/library/stdtypes.html.

[^14]: Python Dictionaries. W3schools.com. (2021). Retrieved 28 June 2021, from https://www.w3schools.com/python/python_dictionaries.asp.
https://docs.python.org/3/tutorial/datastructures.html