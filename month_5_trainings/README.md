# Month #5


# 0x06. Regular expression

## Regular Expression
A regular expression, commonly called a “regexp”, is a sequence of characters that define a search pattern.  It is mainly for use in pattern matching with strings, or string matching (i.e. it operates like a “find and replace” command). While it is a very powerful tool, it is also very dangerous because of its complexity.

Some people, when confronted with a problem, think “I know, I’ll use regular expressions.”   Now they have two problems. (super classic joke in the industry)

One thing you have to be careful with is that different languages use different regexp engines. That means that a regexp in Python, for example, will be interpreted differently in Javascript:

Regular expressions are everywhere and software engineers, no matter their positions, will have to use them during their careers. System administrators and DevOps are the ones using them the most because they are very handy for log parsing.

### Concepts

_For this project, we expect you to look at this concept:_

-   [Regular Expression](https://intranet.alxswe.com/concepts/29)


### Read about regexp:
- [Learn Regular Expressions (Regex) - Crash Course for Beginners](https://www.youtube.com/watch?v=ZfQFUJhPqMM)
- [Regular Expressions (RegEx Playlist) - What is RegEx?](https://www.youtube.com/watch?v=r6I-Ahc0HB4&list=PL4cUxeGkcC9g6m_6Sld9Q4jzqdqHd2HiD)
- [Regular Expression match(), fullmatch(), search(), findall(), finditer(), sub() in Python](https://www.youtube.com/watch?v=XM5zPAbFOn4)
- [Regular Expression](http://www.regular-expressions.info/)
- [Regular Expression](http://www.w3schools.com/jsref/jsref_obj_regexp.asp)
- Play with regexp (or compose them):
- [Ruby: ](http://rubular.com/)
- [PHP/Javascript/Python: ](https://regex101.com/)

## Background Context
For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties.

Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the  `//`:

```
sylvain@ubuntu$ cat example.rb
#!/usr/bin/env ruby
puts ARGV[0].scan(/127.0.0.[0-9]/).join
sylvain@ubuntu$
sylvain@ubuntu$ ./example.rb 127.0.0.2
127.0.0.2
sylvain@ubuntu$ ./example.rb 127.0.0.1
127.0.0.1
sylvain@ubuntu$ ./example.rb 127.0.0.a
```

## Resources
### Read or watch:
- [Regular expressions - basics ](https://www.slideshare.net/neha_jain/introducing-regular-expressions)
- [Regular expressions - advanced ](https://www.slideshare.net/neha_jain/advanced-regular-expressions-80296518)
- [Rubular is your best friend](https://rubular.com)
- [Use a regular expression against a problem: now you have 2 problems   ](https://blog.codinghorror.com/regular-expressions-now-you-have-two-problems/)
- [Learn Regular Expressions with simple, interactive exercises  ](https://regexone.com)


# 0x07. Networking basics #0
![enter image description here](https://www.simplilearn.com/ice9/free_resources_article_thumb/Working_And_Implementation_Of_Physical_Layer_In_The_OSI_Model_1.png)
## Resources
- [OSI](https://www.simplilearn.com/tutorials/cyber-security-tutorial/physical-layer-in-the-osi-model)
- [LAN](https://www.cisco.com/c/en/us/products/switches/what-is-a-lan-local-area-network.html)
### Read or watch:
- [Keith Baker CCNA Playlist](https://www.youtube.com/watch?v=8AX9LandYJU&list=PLQQoSBmrXmrysEaVNia7KVwf85qATIi1V)
- [OSI model](https://en.wikipedia.org/wiki/OSI_model)
- [Different types of network](https://www.lifewire.com/lans-wans-and-other-area-networks-817376)
- [LAN network   ](https://en.wikipedia.org/wiki/Local_area_network)
- [WAN network   ](https://en.wikipedia.org/wiki/Wide_area_network)
- [Internet   ](https://en.wikipedia.org/wiki/Internet)
- [MAC address   ](https://whatismyipaddress.com/mac-address)
- [What is an IP address](https://www.bleepingcomputer.com/tutorials/ip-addresses-explained/)
- [Private and public address    ](https://www.iplocation.net/public-vs-private-ip-address)
- [IPv4 and IPv6 ](https://www.webopedia.com/insights/ipv6-ipv4-difference/)
- [Localhost](https://en.wikipedia.org/wiki/Localhost)
- [TCP and UDP](https://www.howtogeek.com/190014/htg-explains-what-is-the-difference-between-tcp-and-udp/)
- [TCP/UDP ports List ](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)
- [What is ping /ICMP](https://en.wikipedia.org/wiki/Ping_%28networking_utility%29)
- [Positional parameters](https://wiki.bash-hackers.org/scripting/posparams)

### man or help:
- netstat
- ping

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## OSI Model 
- What it is  
- How many layers it has
- How it is organized
- What is a LAN
- Typical usage
- Typical geographical size
- What is a WAN
- Typical usage
- Typical geographical size
- What is the Internet
- What is an IP address
- What are the 2 types of IP address
- What is localhost
- What is a subnet
- Why IPv6 was created

## TCP/UDP
- What are the 2 mainly used data transfer protocols for IP (transfer level on the OSI schema)
- What is the main difference between TCP and UDP
- What is a port
- Memorize SSH, HTTP and HTTPS port numbers
- What tool/protocol is often used to check if a device is connected to a network

# 0x08. Networking basics #1
![enter image description here](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/285/s7kpNYq.png)


## Resources
### Read or watch:
- [CCNA Playlist](https://www.youtube.com/playlist?list=PLxbwE86jKRgMpuZuLBivzlM8s2Dk5lXBQ)
- What is localhost
- What is 0.0.0.0
- What is the hosts file
- Netcat examples

### man or help:
- ifconfig
- telnet
- nc
- cut

## Learning Objectives
### At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
## General
- What is localhost/127.0.0.1
- What is 0.0.0.0
- What is /etc/hosts
- How to display your machine’s active network interfaces


# 0x00. AirBnB clone - The console
![enter image description here](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/65f4a1dd9c51265f49d0.png)

# Background Context
## Welcome to the AirBnB clone project!
Before starting, please read the AirBnB concept page.


## First step: Write a command interpreter to manage your AirBnB objects.
This is the first step towards building your first full web application: the AirBnB clone. This first step is very important because you will use what you build during this project with all other following projects: HTML/CSS templating, database storage, API, front-end integration…

### Each task is linked and will help you to:
 - put in place a parent class (called BaseModel) to take care of the initialization, serialization and deserialization of your future instances
 - create a simple flow of serialization/deserialization:
   Instance <-> Dictionary <-> JSON string <-> file
 - create all classes used for AirBnB (User, State, City, Place…) that inherit from BaseModel
 - create the first abstracted storage engine of the project: File storage.
 - create all unittests to validate all our classes and storage engine

## What’s a command interpreter?
Do you remember the Shell? It’s exactly the same but limited to a specific use-case. In our case, we want to be able to manage the objects of our project:
 - Create a new object (ex: a new User or a new Place) 
 - Retrieve an object from a file, a database etc…
 - Do operations on objects (count, compute stats, etc…)
 - Update attributes of an object
 - Destroy an object

## Resources
### Read or watch:
- [CMD Module](https://docs.python.org/3.8/library/cmd.html)
- [cmd module in depth](http://pymotw.com/2/cmd/)
- packages concept page
- [uuid module](https://docs.python.org/3.8/library/uuid.html)
- [datetime](https://docs.python.org/3.8/library/datetime.html)
- [unittest module](https://docs.python.org/3.8/library/unittest.html#module-unittest)
- [args/kwargs](https://yasoob.me/2013/08/04/args-and-kwargs-in-python-explained/)
- [Python test cheatsheet](https://www.pythonsheets.com/notes/python-tests.html)
- [cmd module wiki page](https://wiki.python.org/moin/CmdModule)
- [python unittest](https://realpython.com/python-testing/)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General

 - How to create a Python package 
 - How to create a command interpreter in Python using the cmd module
 - What is Unit testing and how to implement it in a large project 
 - How to serialize and deserialize a Class 
 - How to write and read a JSON file 
 - How to manage datetime 
 - What is an UUID
 - What is *args and how to use it 
 - What is **kwargs and how to use it
 - How to handle named arguments in a function

# 0x0D. SQL - Introduction
![enter image description here](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/272/rtcwz.jpg)

## Resources
### Read or watch:

- [What is Database & SQL?](https://www.youtube.com/watch?v=FR4QIeZaPeM)
- [A Basic MySQL Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04)
- [Basic SQL statements: DDL and DML (no need to read the chapter “Privileges”)](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/ddldml.php)
- [Basic queries: SQL and RA](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/queries.php)
- [SQL technique: functions](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/functions.php)
- [SQL technique: subqueries ](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/subqueries.php)
- [What makes the big difference between a backtick and an apostrophe?     ](https://stackoverflow.com/questions/29402361/what-makes-the-big-difference-between-a-backtick-and-an-apostrophe/29402458)
- [MySQL Cheat Sheet](https://intellipaat.com/mediaFiles/2019/02/SQL-Commands-Cheat-Sheet.pdf?US)
- [MySQL 8.0 SQL Statement Syntax  ](https://dev.mysql.com/doc/refman/8.0/en/sql-statements.html)
- [installing MySQL in Ubuntu 20.04](https://phoenixnap.com/kb/install-mysql-ubuntu-20-04)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General
 - What’s a database 
 - What’s a relational database 
 - What does SQL stand for
 - What’s MySQL
 - How to create a database in MySQL
 - What does DDL and DML stand for
 - How to CREATE or ALTER a table
 - How to SELECT data from a table
 - How to INSERT, UPDATE or DELETE data
 - What are subqueries
 - How to use MySQL functions


# 0x0E. SQL - More queries
![enter image description here](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/274/66988091.jpg)
## Resources

**Read or watch**:

-   [How To Create a New User and Grant Permissions in MySQL](https://intranet.alxswe.com/rltoken/RniBKj48bnIN8xpXhGl1yA "How To Create a New User and Grant Permissions in MySQL")
-   [How To Use MySQL GRANT Statement To Grant Privileges To a User](https://intranet.alxswe.com/rltoken/FIiEIvA6IN_hSKM5TvgyxQ "How To Use MySQL GRANT Statement To Grant Privileges To a User")
-   [MySQL constraints](https://intranet.alxswe.com/rltoken/LrovGa6N-OE2ID_tpWZRaQ "MySQL constraints")
-   [SQL technique: subqueries](https://intranet.alxswe.com/rltoken/kR71h5zjkPtx4kBoVf7q0g "SQL technique: subqueries")
-   [Basic query operation: the join](https://intranet.alxswe.com/rltoken/rNMJeQ1jbNTCljbvCSjf6w "Basic query operation: the join")
-   [SQL technique: multiple joins and the distinct keyword](https://intranet.alxswe.com/rltoken/HhZ6TJ1q5S0aR4lhfpKdOQ "SQL technique: multiple joins and the distinct keyword")
-   [SQL technique: join types](https://intranet.alxswe.com/rltoken/T6FZUQdsMzr8hgNInBzudA "SQL technique: join types")
-   [SQL technique: union and minus](https://intranet.alxswe.com/rltoken/Nd-sdM8QUpf0YKIlXzVv4w "SQL technique: union and minus")
-   [MySQL Cheat Sheet](https://intranet.alxswe.com/rltoken/iSNyinU6SPWTGDUWMmcRkg "MySQL Cheat Sheet")
-   [The Seven Types of SQL Joins](https://intranet.alxswe.com/rltoken/-plhBsra0N7BOuFoEg--zg "The Seven Types of SQL Joins")
-   [MySQL Tutorial](https://intranet.alxswe.com/rltoken/I4Lws_eQrIrNTbkZvvk-oQ "MySQL Tutorial")
-   [SQL Style Guide](https://intranet.alxswe.com/rltoken/051eAEP_rePBU7jeh879GA "SQL Style Guide")
-   [MySQL 8.0 SQL Statement Syntax](https://intranet.alxswe.com/rltoken/YavbYiraYFr8oTukT_N6eQ "MySQL 8.0 SQL Statement Syntax")

Extra resources around relational database model design:

-   [Design](https://intranet.alxswe.com/rltoken/EWLRPeqr5sQ9AqfoG_KXxw "Design")
-   [Normalization](https://intranet.alxswe.com/rltoken/mqBhYoSYbhH5ZZrhDcY0kA "Normalization")
-   [ER Modeling](https://intranet.alxswe.com/rltoken/R0exkJmf-2ddKjGfa8D0dA "ER Modeling")

## Learning Objectives

At the end of this project, you are expected to be able to  [explain to anyone](https://intranet.alxswe.com/rltoken/0qci3VdIVdKJXldEZ6zAjA "explain to anyone"),  **without the help of Google**:

### General

-   How to create a new MySQL user
-   How to manage privileges for a user to a database or table
-   What’s a  `PRIMARY KEY`
-   What’s a  `FOREIGN KEY`
-   How to use  `NOT NULL`  and  `UNIQUE`  constraints
-   How to retrieve datas from multiple tables in one request
-   What are subqueries
-   What are  `JOIN`  and  `UNION`

# 0x01. AirBnB clone - Web static
### Concepts

_For this project, we expect you to look at these concepts:_

-   [HTML/CSS](https://intranet.alxswe.com/concepts/2)
-   [The trinity of front-end quality](https://intranet.alxswe.com/concepts/4)

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2021/9/135ef103cf7ed150c9760aadc66844113dfc3d35.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230522%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230522T185555Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6be38c378edc1e9de280d86c8abc14e73ca89e4a2c0b40f1d12f6cddfddcae99)

## Background Context

### Web static, what?

Now that you have a command interpreter for managing your AirBnB objects, it’s time to make them alive!

Before developing a big and complex web application, we will build the front end step-by-step.

The first step is to “design” / “sketch” / “prototype” each element:

-   Create simple HTML static pages
-   Style guide
-   Fake contents
-   No Javascript
-   No data loaded from anything

During this project, you will learn how to manipulate HTML and CSS languages. HTML is the structure of your page, it should be the first thing to write. CSS is the styling of your page, the design. I really encourage you to fix your HTML part before starting the styling. Indeed, without any structure, you can’t apply any design.

Before starting, please fork or clone the repository  `AirBnB_clone`  from your partner if you were not the owner of the previous project.

## Resources

**Read or watch**:

-   [Learn to Code HTML & CSS](https://intranet.alxswe.com/rltoken/T9KyiA6_Tm3Ny6oTn08S-A "Learn to Code HTML & CSS")  (_until “Creating Lists” included_)
-   [Inline Styles in HTML](https://intranet.alxswe.com/rltoken/7NdYbImFNofpB_FXXn3otg "Inline Styles in HTML")
-   [Specifics on CSS Specificity](https://intranet.alxswe.com/rltoken/z_OTPFCjmhXJJi7KJqBCbQ "Specifics on CSS Specificity")
-   [CSS SpeciFishity](https://intranet.alxswe.com/rltoken/orI812cozq-yd2769VdM_w "CSS SpeciFishity")
-   [Introduction to HTML](https://intranet.alxswe.com/rltoken/okP4V3RxFXHkEcQo19AnuQ "Introduction to HTML")
-   [CSS](https://intranet.alxswe.com/rltoken/Ir8Ka59FO6Z_vJQ-gkSG_w "CSS")
-   [MDN](https://intranet.alxswe.com/rltoken/BpSXtcWOGH0UT4XLCoQyJg "MDN")
-   [center boxes](https://intranet.alxswe.com/rltoken/Tlje4XYwyZbUfHkQWGi1WQ "center boxes")

## Learning Objectives

At the end of this project, you are expected to be able to  [explain to anyone](https://intranet.alxswe.com/rltoken/Zb9sTIct2xdhDCDLGF-RyQ "explain to anyone"),  **without the help of Google**:

### General

-   What is HTML
-   How to create an HTML page
-   What is a markup language
-   What is the DOM
-   What is an element / tag
-   What is an attribute
-   How does the browser load a webpage
-   What is CSS
-   How to add style to an element
-   What is a class
-   What is a selector
-   How to compute CSS Specificity Value
-   What are Box properties in CSS


# Authors
## **[Innocent Udo](https://www.github.com/innocentsax)**, **[Owolabi Pius](https://www.github.com/opius2017)**
