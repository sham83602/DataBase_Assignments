## **\*\*# DataBase_Assignments\*\***

##

## **\*\*# Assignments 1\*\***

##

## **create table orders ( onum int (4),amt float (7,2),odate date , cnum int**

## **(4),snum int (4));**

##

## **insert into orders values (3001,18.69,'1990-10-03',2008,1007);**

##

## **insert into orders values (3003,767.19,'1990-10-03',2001,1001);**

##

## **insert into orders values (3002,1900.10,'1990-10-03',2007,1004);**

##

## **insert into orders values (3005,5160.45,'1990-10-03',2003,1002);**

##

## **insert into orders values (3006,1098.16,'1990-10-03',2008,1007);**

##

## **insert into orders values (3009,1713.23,'1990-10-04',2002,1003);**

##

## **insert into orders values (3007,75.75,'1990-10-04',2004,1002);**

##

## **insert into orders values (3008,4723.00,'1990-10-05',2006,1001);**

##

## **insert into orders values (3010,1309.95,'1990-10-06',2004,1002);**

##

## **insert into orders values (3011,9891.88,'1990-10-06',2006,1001);**

##

## **select\*from orders;**

##

## **create table customers ( cnum int (4),cname varchar (10),city varchar**

## **(10),rating int (4),snum int (4));**

##

## **insert into customers values (2001,'hoffman','london',100,1001);**

##

## **insert into customers values (2002,'giovanni','rome',200,1003);**

##

## **insert into customers values (2003,'liu','san jose',200,1002);**

##

## **insert into customers values (2004,'grass','berlin',300,1002);**

##

## **insert into customers values (2006,'clemens','london',100,1001);**

##

## **insert into customers values (2008,'cisneros','san jose',300,1007);**

##

## **insert into customers values (2007,'pereira','rome',100,1004);**

##

## **selec**from customers;\*\*

##

## **create table salespeople ( snum int (4), sname varchar (10),city varchar**

## **(10),comm float (3,2));**

##

## **insert into salespeople values (1001,'peel','london',.12);**

##

## **insert into salespeople values (1002,'serres','san joes',.13);**

##

## **insert into salespeople values (1004,'motika','london',.11);**

##

## **insert into salespeople values (1007,'rifkin','barcelona',.15);**

##

## **insert into salespeople values (1003,'axelrod','new york',.10);**

##

## **selec** from salespeople;\*\*

##

## **\*\*# Answer of Assignments 1\*\***

##

## **KD3_SHAM_83602>create table orders ( onum int (4),amt float**

## **(7,2),odate date , cnum int (4),snum int (4));**

##

## **Query OK, 0 rows affected, 4 warnings (0.04 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3001,18.69,'1990-10-03',2008,1007);**

##

## **Query OK, 1 row affected (0.01 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3003,767.19,'1990-10-03',2001,1001);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3002,1900.10,'1990-10-03',2007,1004);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3005,5160.45,'1990-10-03',2003,1002);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3006,1098.16,'1990-10-03',2008,1007);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3009,1713.23,'1990-10-04',2002,1003);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3007,75.75,'1990-10-04',2004,1002);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3008,4723.00,'1990-10-05',2006,1001);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3010,1309.95,'1990-10-06',2004,1002);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into orders values**

## **(3011,9891.88,'1990-10-06',2006,1001);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>selec**\*from orders;\*\*

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt     | odate      | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3001 |   18.69 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3003 |  767.19 | 1990-10-03 | 2001 | 1001 |**

##

## **| 3002 | 1900.10 | 1990-10-03 | 2007 | 1004 |**

##

## **| 3005 | 5160.45 | 1990-10-03 | 2003 | 1002 |**

##

## **| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3007 |   75.75 | 1990-10-04 | 2004 | 1002 |**

##

## **| 3008 | 4723.00 | 1990-10-05 | 2006 | 1001 |**

##

## **| 3010 | 1309.95 | 1990-10-06 | 2004 | 1002 |**

##

## **| 3011 | 9891.88 | 1990-10-06 | 2006 | 1001 |**

##

## **+------+---------+------------+------+------+**

##

## **10 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>create table customers ( cnum int (4),cname varchar**

## **(10),city varchar (10),rating int (4),snum int (4));**

##

## **Query OK, 0 rows affected, 3 warnings (0.03 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>insert into customers values**

## **(2001,'hoffman','london',100,1001);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into customers values**

## **(2002,'giovanni','rome',200,1003);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into customers values (2003,'liu','san**

## **jose',200,1002);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into customers values**

## **(2004,'grass','berlin',300,1002);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into customers values**

## **(2006,'clemens','london',100,1001);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into customers values (2008,'cisneros','san**

## **jose',300,1007);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into customers values**

## **(2007,'pereira','rome',100,1004);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>selec**from customers;\*\*

##

## **+------+----------+----------+--------+------+**

##

## **| cnum | cname    | city     | rating | snum |**

##

## **+------+----------+----------+--------+------+**

##

## **| 2001 | hoffman  | london   |    100 | 1001 |**

##

## **| 2002 | giovanni | rome     |    200 | 1003 |**

##

## **| 2003 | liu      | san jose |    200 | 1002 |**

##

## **| 2004 | grass    | berlin   |    300 | 1002 |**

##

## **| 2006 | clemens  | london   |    100 | 1001 |**

##

## **| 2008 | cisneros | san jose |    300 | 1007 |**

##

## **| 2007 | pereira  | rome     |    100 | 1004 |**

##

## **+------+----------+----------+--------+------+**

##

## **7 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>create table salespeople ( snum int (4), sname varchar**

## **(10),city varchar (10),comm float (3,2));**

##

## **Query OK, 0 rows affected, 2 warnings (0.03 sec)**

##

## **KD3_SHAM_83602>**

##

## **KD3_SHAM_83602>insert into salespeople values**

## **(1001,'peel','london',.12);**

##

## **Query OK, 1 row affected (0.01 sec)**

##

## **KD3_SHAM_83602>insert into salespeople values (1002,'serres','san**

## **joes',.13);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into salespeople values**

## **(1004,'motika','london',.11);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into salespeople values**

## **(1007,'rifkin','barcelona',.15);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>insert into salespeople values (1003,'axelrod','new**

## **york',.10);**

##

## **Query OK, 1 row affected (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from salespeople;\*\*

##

## **+------+---------+-----------+------+**

##

## **| snum | sname   | city      | comm |**

##

## **+------+---------+-----------+------+**

##

## **| 1001 | peel    | london    | 0.12 |**

##

## **| 1002 | serres  | san joes  | 0.13 |**

##

## **| 1004 | motika  | london    | 0.11 |**

##

## **| 1007 | rifkin  | barcelona | 0.15 |**

##

## **| 1003 | axelrod | new york  | 0.10 |**

##

## **+------+---------+-----------+------+**

##

## **5 rows in set (0.00 sec)**

##

## **\*\*# Assignments 2\*\***

##

## **Q.1 Which field of the customer table is primary key ?**

##

## **Q.2 What is the 4th column of customer table?**

##

## **Ans. Rating**

##

## **Q.3 What is another word for row and column?**

##

## **Ans. Row is also called as tuple, entity, opportinity Column is also**

## **called as attributes, methods , keys**

##

## **Q.4 Why isnt it possible to see 1st 5 rows of a table?**

##

## **Ans. The rows are stored at diffrent places in a server HDD in a file**

## **format. And they**

##

## **are called sequentially as per there address. No specific location is**

## **given to the rows.**

##

## **Thats why it is not possible to see 1st 5 rows of the table.**

##

## **\*\*# Assignments 3\*\***

##

## **Q.1 Does ANSI recognise the data type DATE?**

##

## **Ans : ANSI dosent recognise the date datatype.**

##

## **Q.2 Which subdivison of SQL is used to insert values in tables?**

##

## **Ans : INSERT into is used**

##

## **It is a DML command**

##

## **\*\*# Assignments 4\*\***

##

## **select onum,amt,odate from orders;**

##

## **selec**from customers where snum = 1001;\*\*

##

## **select city,sname,snum,comm from salespeople;**

##

## **select rating,cname from customers where city='san jose';**

##

## **\*\*# Answer of Assignments 4\*\***

##

## **KD3_SHAM_83602>select onum,amt,odate from orders;**

##

## **+------+---------+------------+**

##

## **| onum | amt | odate |**

##

## **+------+---------+------------+**

##

## **| 3001 | 18.69 | 1990-10-03 |**

##

## **| 3003 | 767.19 | 1990-10-03 |**

##

## **| 3002 | 1900.10 | 1990-10-03 |**

##

## **| 3005 | 5160.45 | 1990-10-03 |**

##

## **| 3006 | 1098.16 | 1990-10-03 |**

##

## **| 3009 | 1713.23 | 1990-10-04 |**

##

## **| 3007 | 75.75 | 1990-10-04 |**

##

## **| 3008 | 4723.00 | 1990-10-05 |**

##

## **| 3010 | 1309.95 | 1990-10-06 |**

##

## **| 3011 | 9891.88 | 1990-10-06 |**

##

## **+------+---------+------------+**

##

## **10 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from customers where snum = 1001;\*\*

##

## **+------+---------+--------+--------+------+**

##

## **| cnum | cname | city | rating | snum |**

##

## **+------+---------+--------+--------+------+**

##

## **| 2001 | hoffman | london | 100 | 1001 |**

##

## **| 2006 | clemens | london | 100 | 1001 |**

##

## **+------+---------+--------+--------+------+**

##

## **2 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select city,sname,snum,comm from salespeople;**

##

## **+-----------+---------+------+------+**

##

## **| city | sname | snum | comm |**

##

## **+-----------+---------+------+------+**

##

## **| london | peel | 1001 | 0.12 |**

##

## **| san joes | serres | 1002 | 0.13 |**

##

## **| london | motika | 1004 | 0.11 |**

##

## **| barcelona | rifkin | 1007 | 0.15 |**

##

## **| new york | axelrod | 1003 | 0.10 |**

##

## **+-----------+---------+------+------+**

##

## **5 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select rating,cname from customers where city='san**

## **jose';**

##

## **+--------+----------+**

##

## **| rating | cname |**

##

## **+--------+----------+**

##

## **| 200 | liu |**

##

## **| 300 | cisneros |**

##

## **+--------+----------+**

##

## **2 rows in set (0.00 sec)**

##

## **\*\*# Assignments 5\*\***

##

## **selec**from orders where amt > 1000;\*\*

##

## **select sname , city from salespeople where comm > .10 and city =**

## **'london';**

##

## **selec**from customers where rating <= 100 and city != 'rome';\*\*

##

## **selec**from orders where (amt < 1000 or not (odate = '1990-10-03'\*\*

## **and cnum > 2003));**

##

## **selec**from orders where not ((odate = '1990-10-03' or snum>1006)\*\*

## **and amt >= 1500);**

##

## **select snum , sname , city , comm from salespeople where (comm > .12 or**

## **comm < .14);**

##

## **\*\*# Answer of Assignments 5\*\***

##

## **KD3_SHAM_83602>selec**from orders where amt > 1000;\*\*

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt | odate | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3002 | 1900.10 | 1990-10-03 | 2007 | 1004 |**

##

## **| 3005 | 5160.45 | 1990-10-03 | 2003 | 1002 |**

##

## **| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3008 | 4723.00 | 1990-10-05 | 2006 | 1001 |**

##

## **| 3010 | 1309.95 | 1990-10-06 | 2004 | 1002 |**

##

## **| 3011 | 9891.88 | 1990-10-06 | 2006 | 1001 |**

##

## **+------+---------+------------+------+------+**

##

## **7 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select sname , city from salespeople where comm > .10**

## **and city = 'london';**

##

## **+--------+--------+**

##

## **| sname | city |**

##

## **+--------+--------+**

##

## **| peel | london |**

##

## **| motika | london |**

##

## **+--------+--------+**

##

## **2 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from customers where rating <= 100 and city\*\*

## **!= 'rome';**

##

## **+------+---------+--------+--------+------+**

##

## **| cnum | cname | city | rating | snum |**

##

## **+------+---------+--------+--------+------+**

##

## **| 2001 | hoffman | london | 100 | 1001 |**

##

## **| 2006 | clemens | london | 100 | 1001 |**

##

## **+------+---------+--------+--------+------+**

##

## **2 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from orders where (amt < 1000 or not (odate\*\*

## **= '1990-10-03' and cnum > 2003));**

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt | odate | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3001 | 18.69 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3003 | 767.19 | 1990-10-03 | 2001 | 1001 |**

##

## **| 3005 | 5160.45 | 1990-10-03 | 2003 | 1002 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3007 | 75.75 | 1990-10-04 | 2004 | 1002 |**

##

## **| 3008 | 4723.00 | 1990-10-05 | 2006 | 1001 |**

##

## **| 3010 | 1309.95 | 1990-10-06 | 2004 | 1002 |**

##

## **| 3011 | 9891.88 | 1990-10-06 | 2006 | 1001 |**

##

## **+------+---------+------------+------+------+**

##

## **8 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from orders where not ((odate =\*\*

## **'1990-10-03' or snum>1006) and amt >= 1500);**

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt | odate | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3001 | 18.69 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3003 | 767.19 | 1990-10-03 | 2001 | 1001 |**

##

## **| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3007 | 75.75 | 1990-10-04 | 2004 | 1002 |**

##

## **| 3008 | 4723.00 | 1990-10-05 | 2006 | 1001 |**

##

## **| 3010 | 1309.95 | 1990-10-06 | 2004 | 1002 |**

##

## **| 3011 | 9891.88 | 1990-10-06 | 2006 | 1001 |**

##

## **+------+---------+------------+------+------+**

##

## **8 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select snum , sname , city , comm from salespeople where**

## **(comm > .12 or comm < .14);**

##

## **+------+---------+-----------+------+**

##

## **| snum | sname | city | comm |**

##

## **+------+---------+-----------+------+**

##

## **| 1001 | peel | london | 0.12 |**

##

## **| 1002 | serres | san joes | 0.13 |**

##

## **| 1004 | motika | london | 0.11 |**

##

## **| 1007 | rifkin | barcelona | 0.15 |**

##

## **| 1003 | axelrod | new york | 0.10 |**

##

## **+------+---------+-----------+------+**

##

## **5 rows in set (0.01 sec)**

##

## **\*\*# Assignments 6\*\***

##

## **selec**\\\_ from orders where odate between '1990-10-03' and\*\*

## **'1990-10-04';**

##

## **selec**\\\_ from orders where odate >= '1990-10-03' and odate <=\*\*

## **'1990-10-04';**

##

## **selec**\\\_ from customers where snum in (select snum from salespeople\*\*

## **where sname in ('peel' , 'motika'));**

##

## **select cname,sname from salespeople,customers where salespeople.snum**

## **=customers.snum having sname='peel' or sname='motika';**

##

## **selec**\\\_ from customers where cname >= 'A' and cname <= 'H';\*\*

##

## **selec**\\\_ from customers where cname like 'C%';\*\*

##

## **selec**\\\_ from orders where amt != '0' OR amt != NULL ;\*\*

##

## **\*\*# Answer of Assignments 6\*\***

##

## **KD3_SHAM_83602>selec**from orders where odate between\*\*

## **'1990-10-03' and '1990-10-04';**

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt | odate | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3001 | 18.69 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3003 | 767.19 | 1990-10-03 | 2001 | 1001 |**

##

## **| 3002 | 1900.10 | 1990-10-03 | 2007 | 1004 |**

##

## **| 3005 | 5160.45 | 1990-10-03 | 2003 | 1002 |**

##

## **| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3007 | 75.75 | 1990-10-04 | 2004 | 1002 |**

##

## **+------+---------+------------+------+------+**

##

## **7 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from orders where odate >= '1990-10-03'\*\*

## **and odate <= '1990-10-04';**

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt | odate | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3001 | 18.69 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3003 | 767.19 | 1990-10-03 | 2001 | 1001 |**

##

## **| 3002 | 1900.10 | 1990-10-03 | 2007 | 1004 |**

##

## **| 3005 | 5160.45 | 1990-10-03 | 2003 | 1002 |**

##

## **| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3007 | 75.75 | 1990-10-04 | 2004 | 1002 |**

##

## **+------+---------+------------+------+------+**

##

## **7 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from customers where snum in (select snum\*\*

## **from salespeople where sname in ('peel' , 'motika'));**

##

## **+------+---------+--------+--------+------+**

##

## **| cnum | cname | city | rating | snum |**

##

## **+------+---------+--------+--------+------+**

##

## **| 2001 | hoffman | london | 100 | 1001 |**

##

## **| 2006 | clemens | london | 100 | 1001 |**

##

## **| 2007 | pereira | rome | 100 | 1004 |**

##

## **+------+---------+--------+--------+------+**

##

## **3 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select cname,sname from salespeople,customers where**

## **salespeople.snum =customers.snum having sname='peel' or**

## **sname='motika';**

##

## **+---------+--------+**

##

## **| cname | sname |**

##

## **+---------+--------+**

##

## **| hoffman | peel |**

##

## **| clemens | peel |**

##

## **| pereira | motika |**

##

## **+---------+--------+**

##

## **3 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from customers where cname >= 'A' and\*\*

## **cname <= 'H';**

##

## **+------+----------+----------+--------+------+**

##

## **| cnum | cname | city | rating | snum |**

##

## **+------+----------+----------+--------+------+**

##

## **| 2002 | giovanni | rome | 200 | 1003 |**

##

## **| 2004 | grass | berlin | 300 | 1002 |**

##

## **| 2006 | clemens | london | 100 | 1001 |**

##

## **| 2008 | cisneros | san jose | 300 | 1007 |**

##

## **+------+----------+----------+--------+------+**

##

## **4 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from customers where cname like 'C%';\*\*

##

## **+------+----------+----------+--------+------+**

##

## **| cnum | cname | city | rating | snum |**

##

## **+------+----------+----------+--------+------+**

##

## **| 2006 | clemens | london | 100 | 1001 |**

##

## **| 2008 | cisneros | san jose | 300 | 1007 |**

##

## **+------+----------+----------+--------+------+**

##

## **2 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>selec**from orders where amt != '0' OR amt !=\*\*

## **NULL ;**

##

## **+------+---------+------------+------+------+**

##

## **| onum | amt | odate | cnum | snum |**

##

## **+------+---------+------------+------+------+**

##

## **| 3001 | 18.69 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3003 | 767.19 | 1990-10-03 | 2001 | 1001 |**

##

## **| 3002 | 1900.10 | 1990-10-03 | 2007 | 1004 |**

##

## **| 3005 | 5160.45 | 1990-10-03 | 2003 | 1002 |**

##

## **| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |**

##

## **| 3009 | 1713.23 | 1990-10-04 | 2002 | 1003 |**

##

## **| 3007 | 75.75 | 1990-10-04 | 2004 | 1002 |**

##

## **| 3008 | 4723.00 | 1990-10-05 | 2006 | 1001 |**

##

## **| 3010 | 1309.95 | 1990-10-06 | 2004 | 1002 |**

##

## **| 3011 | 9891.88 | 1990-10-06 | 2006 | 1001 |**

##

## **+------+---------+------------+------+------+**

##

## **10 rows in set (0.00 sec)**

##

## **\*\*# Assignments 7\*\***

##

## **select count(odate) from orders where odate='1990-10-03';**

##

## **select count(city) from customers where city is not null;**

##

## **select min(amt),cname from customers,orders where**

## **customers.snum=orders.snum group by cname;**

##

## **select cname from customers where cname like 'g%' limit 1;**

##

## **select max(rating) from customers group by city;**

##

## **select odate, count(distinct snum) from orders group by odate;**

##

## **select odate, count(distinct o.snum) from orders o, salespeople S where**

## **o.snum=S.snum group by odate;**

##

## **\*\*# Answer of Assignments 7\*\***

##

## **KD3_SHAM_83602>select count(odate) from orders where**

## **odate='1990-10-03';**

##

## **+--------------+**

##

## **| count(odate) |**

##

## **+--------------+**

##

## **| 5 |**

##

## **+--------------+**

##

## **1 row in set (0.00 sec)**

##

## **KD3_SHAM_83602>select count(city) from customers where city is not**

## **null;**

##

## **+-------------+**

##

## **| count(city) |**

##

## **+-------------+**

##

## **| 7 |**

##

## **+-------------+**

##

## **1 row in set (0.00 sec)**

##

## **KD3_SHAM_83602>select min(amt),cname from customers,orders where**

## **customers.snum=orders.snum group by cname;**

##

## **+----------+----------+**

##

## **| min(amt) | cname |**

##

## **+----------+----------+**

##

## **| 18.69 | cisneros |**

##

## **| 767.19 | clemens |**

##

## **| 767.19 | hoffman |**

##

## **| 1900.10 | pereira |**

##

## **| 75.75 | grass |**

##

## **| 75.75 | liu |**

##

## **| 1713.23 | giovanni |**

##

## **+----------+----------+**

##

## **7 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select cname from customers where cname like 'g%'**

## **limit 1;**

##

## **+----------+**

##

## **| cname |**

##

## **+----------+**

##

## **| giovanni |**

##

## **+----------+**

##

## **1 row in set (0.00 sec)**

##

## **KD3_SHAM_83602>select max(rating) from customers group by city;**

##

## **+-------------+**

##

## **| max(rating) |**

##

## **+-------------+**

##

## **| 100 |**

##

## **| 200 |**

##

## **| 300 |**

##

## **| 300 |**

##

## **+-------------+**

##

## **4 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select odate, count(distinct snum) from orders group by**

## **odate;**

##

## **+------------+----------------------+**

##

## **| odate | count(distinct snum) |**

##

## **+------------+----------------------+**

##

## **| 1990-10-03 | 4 |**

##

## **| 1990-10-04 | 2 |**

##

## **| 1990-10-05 | 1 |**

##

## **| 1990-10-06 | 2 |**

##

## **+------------+----------------------+**

##

## **4 rows in set (0.00 sec)**

##

## **KD3_SHAM_83602>select odate, count(distinct o.snum) from orders o,**

## **salespeople S where o.snum=S.snum group by odate;**

##

## **+------------+------------------------+**

##

## **| odate | count(distinct o.snum) |**

##

## **+------------+------------------------+**

##

## **| 1990-10-03 | 4 |**

##

## **| 1990-10-04 | 2 |**

##

## **| 1990-10-05 | 1 |**

##

## **| 1990-10-06 | 2 |**

##

## **+------------+------------------------+**

##

## **4 rows in set (0.00 sec)**

##

##
