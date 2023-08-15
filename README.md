# Company DataBase

## Intro to SQL
**SQL** stands for **Structured Query Language**
It is a programming language specifically designed for managing and manipulating relational databases. 
SQL allows users to define, retrieve, and manipulate data stored in a database management system (DBMS).

**CRUD** stands for Create, Read, Update, and Delete. It is a set of basic operations that can be performed on data in a database using SQL or any other database management system.

*SQL can be divided into several categories based on the types of operations it performs:*

1.**DDL** (Data Definition Language): DDL statements are used to define and manage the structure of database objects such as tables, views, indexes, and schemas. Common DDL statements include:
- CREATE: Used to create a new database object, such as a table or view.
- ALTER: Used to modify the structure of an existing database object.
- DROP: Used to remove a database object from the database.

2.**DML** (Data Manipulation Language): DML statements are used to manipulate data within the database. They are used to insert, retrieve, update, and delete records in database tables. Common DML statements include:
- SELECT: Used to retrieve data from one or more database tables.
- INSERT: Used to insert new records into a table.
- UPDATE: Used to modify existing records in a table.
- DELETE: Used to remove records from a table.

3.**DQL** (Data Query Language): DQL is a subset of DML and is specifically used for querying and retrieving data from the database. The most common DQL statement is SELECT, which allows you to retrieve data based on specified criteria.

4.**DCL** (Data Control Language): DCL statements are used to control access to the database and manage privileges. They are used to grant or revoke permissions to database users. Common DCL statements include:
- GRANT: Used to provide specific privileges to a user or role.
- REVOKE: Used to remove specific privileges from a user or role.
___
## Company DataBase Intro

Database Schema 
: refers to the structure or blueprint of a database. It defines how the data is organized, the relationships between different data elements, and the constraints and rules that govern the data.


![database_structure](database-intro.jpg)

___

**TASK 1** : creating company database.

**TASK 2** : inserting data/information.

**TASK 3** : write Queries to get the specific data mentioned below.<br>
Q1) Find all employees<br>
Q2) Find all clients<br>
Q3) Find all employees ordered by salary<br>
Q4) Find all employees ordered by sex then name<br>
Q5) Find the first 5 employees in the table<br>
Q6) Find the first and last names of all employees<br>
Q7) Find the forename and surnames names of all employees<br>
Q8) Find out all the different genders<br>
Q9) Find all male employees<br>
Q10) Find all employees at branch 2<br>
Q11) Find all employee's id's and names who were born after 1969<br>
Q12) Find all female employees at branch 2<br>
Q13) Find all employees who are female & born after 1969 or who make over 80000<br>
Q14) Find all employees born between 1970 and 1975<br>
Q15) Find all employees named Jim, Michael, Johnny or David<br>
Q16) Find the number of employees<br>
Q17) Find the average of all employee's salaries<br>
Q18) Find the sum of all employee's salaries<br>
Q19) Find out how many males and females there are<br>
Q20) Find the total sales of each salesman<br>
Q21) Find the total amount of money spent by each client<br>
Q22) Find any client's who are an LLC<br>
Q23) Find any branch suppliers who are in the label business<br>
Q24) Find any employee born on the 10th day of the month<br>
Q25) Find any clients who are schools<br>
Q26) Find a list of employee and branch names<br>
Q27) Find a list of all clients & branch suppliers' names<br>
Q28) Find all branches and the name of their managers<br>
Q29) Find names of all employees who have sold over 50,000<br>
Q30) Find all clients who are handles by the branch that Michael Scott manages<br>
Q31) Find the names of employees who work with clients handled by the scranton branch<br>
Q32) Find the names of all clients who have spent more than 100,000 dollars<br>

___

check out ![SQL code](company-database.sql)

___

![ER Diagram Template](erd-template.PNG)

**Company Data Storage Requirements**

The company is organized into branches. Each branch has a unique number, a name, and a particular employee who manages it.

The company makes it’s money by selling to clients. Each client has a name and a unique number to identify it.

The foundation of the company is it’s employees. Each employee has a name, birthday, sex, salary and a unique number.

An employee can work for one branch at a time, and each branch will be managed by one of the employees that work there. We’ll also want to keep track of when the current manager started as manager.

An employee can act as a supervisor for other employees at the branch, an employee may also act as the supervisor for employees at other branches. An employee can have at most one supervisor.

A branch may handle a number of clients, with each client having a name and a unique number to identify it. A single client may only be handled by one branch at a time.

Employees can work with clients controlled by their branch to sell them stuff. If nescessary multiple employees can work with the same client. We’ll want to keep track of how many dollars worth of stuff each employee sells to each client they work with.

Many branches will need to work with suppliers to buy inventory. For each supplier we’ll keep track of their name and the type of product they’re selling the branch. A single supplier may supply products to multiple branches.

![company ER Diagram](company-erd.PNG)

![company database schema](database-schema.PNG)