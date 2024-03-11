## DataBase_Assignments

# Assignments 1

```
create table orders ( onum int (4),amt float (7,2),odate date , cnum int (4),snum int (4));
insert into orders values (3001,18.69,'1990-10-03',2008,1007);
insert into orders values (3003,767.19,'1990-10-03',2001,1001);
insert into orders values (3002,1900.10,'1990-10-03',2007,1004);
insert into orders values (3005,5160.45,'1990-10-03',2003,1002);
insert into orders values (3006,1098.16,'1990-10-03',2008,1007);
insert into orders values (3009,1713.23,'1990-10-04',2002,1003);
insert into orders values (3007,75.75,'1990-10-04',2004,1002);
insert into orders values (3008,4723.00,'1990-10-05',2006,1001);
insert into orders values (3010,1309.95,'1990-10-06',2004,1002);
insert into orders values (3011,9891.88,'1990-10-06',2006,1001);

select \*from orders;

create table customers ( cnum int (4),cname varchar (10),city varchar (10),rating int (4),snum int (4));

insert into customers values (2001,'hoffman','london',100,1001);
insert into customers values (2002,'giovanni','rome',200,1003);
insert into customers values (2003,'liu','san jose',200,1002);
insert into customers values (2004,'grass','berlin',300,1002);
insert into customers values (2006,'clemens','london',100,1001);
insert into customers values (2008,'cisneros','san jose',300,1007);
insert into customers values (2007,'pereira','rome',100,1004);

select \*from customers;

create table salespeople ( snum int (4), sname varchar (10),city varchar (10),comm float (3,2));

insert into salespeople values (1001,'peel','london',.12);
insert into salespeople values (1002,'serres','san joes',.13);
insert into salespeople values (1004,'motika','london',.11);
insert into salespeople values (1007,'rifkin','barcelona',.15);
insert into salespeople values (1003,'axelrod','new york',.10);
select \* from salespeople;
```

# Assignments 2

```
Q.1 Which field of the customer table is primary key ?

Q.2 What is the 4th column of customer table?
Ans. Rating

Q.3 What is another word for row and column?
Ans. Row is also called as tuple, entity, opportinity Column is also called as attributes, methods , keys

Q.4 Why isnt it possible to see 1st 5 rows of a table?
Ans. The rows are stored at diffrent places in a server HDD in a file format. And they
are called sequentially as per there address. No specific location is given to the rows.
Thats why it is not possible to see 1st 5 rows of the table.
```

# Assignments 3

```
Q.1 Does ANSI recognise the data type DATE?
Ans : ANSI dosent recognise the date datatype.

Q.2 Which subdivison of SQL is used to insert values in tables?
Ans : INSERT into is used
It is a DML command
```

# Assignments 4

```
select onum,amt,odate from orders;
select \* from customers where snum = 1001;
select city,sname,snum,comm from salespeople;
select rating,cname from customers where city='san jose';
```

# Assignments 5

```
select * from orders where amt > 1000;
select sname , city from salespeople where comm > .10 and city = 'london';
select *from customers where rating <= 100 and city != 'rome';
select *from orders where (amt < 1000 or not (odate = '1990-10-03' and cnum > 2003));
select *from orders where not ((odate = '1990-10-03' or snum>1006) and amt >= 1500);
select snum , sname , city , comm from salespeople where (comm > .12 or comm < .14);
```

# Assignments 6

```
select _ from orders where odate between '1990-10-03' and '1990-10-04';
select _ from orders where odate >= '1990-10-03' and odate <= '1990-10-04';
select _ from customers where snum in (select snum from salespeople where sname in ('peel' , 'motika'));
select cname,sname from salespeople,customers where salespeople.snum =customers.snum having sname='peel' or sname='motika';
select _ from customers where cname >= 'A' and cname <= 'H';
select _ from customers where cname like 'C%';
select _ from orders where amt != '0' OR amt != NULL ;
```

# Assignments 7

```
select count(odate) from orders where odate='1990-10-03';
select count(city) from customers where city is not null;
select min(amt),cname from customers,orders where customers.snum=orders.snum group by cname;
select cname from customers where cname like 'g%' limit 1;
select max(rating) from customers group by city;
select odate, count(distinct snum) from orders group by odate;
select odate, count(distinct o.snum) from orders o, salespeople S where o.snum=S.snum group by odate;
```

# Assignments 8

```
select onum, s.snum, amt+amt\*0.12 as commission from salespeople s, orders o where s.snum=o.snum;
select concat('for the ',city,' the heightest rating is : ',max(rating)) as 'Highest Rating' from customers group by city;
select rating ,cname,cnum from customers order by rating desc;
select odate , count(onum) from orders group by odate order by 2 desc;
```

# Assignments 9

```
select onum,cname from orders o, customers c where c.cnum = o.cnum;
select sname , cname , onum from orders o,
customers c, salespeople p
where o.snum = p.snum and o.cnum = c.cnum;
select cname, sname,comm from salespeople s , customers c
where c.snum = s.snum
having comm >0.12;
select amt * comm ,rating commissions
from salespeople s , customers c , orders o
where o.snum=c.snum and o.snum=s.snum
having rating>100;
```

# Assignments 10

```
select s.sname , s.city , sp.sname from salespeople s , salespeople sp
 where sp.city=s.city and s.snum< sp.snum;

select cname , city from customers
where rating = (
select rating from customers where
cname = 'hoffman'
);
select c.cname, c.city from customers c, customers d
 where d.rating = c.rating
 having cname = 'hoffman';
```
# answers
``` 
 KD3_SHAM_83602>select s.sname , s.city , sp.sname from salespeople s , salespeople sp
    ->  where sp.city=s.city and s.snum< sp.snum;
+-------+--------+--------+
| sname | city   | sname  |
+-------+--------+--------+
| peel  | london | motika |
+-------+--------+--------+
1 row in set (0.00 sec)

KD3_SHAM_83602>
KD3_SHAM_83602>select cname , city from customers
    -> where rating = (
    -> select rating from customers where
    -> cname = 'hoffman'
    -> );
+---------+--------+
| cname   | city   |
+---------+--------+
| hoffman | london |
| clemens | london |
| pereira | rome   |
+---------+--------+
3 rows in set (0.00 sec)

KD3_SHAM_83602>select c.cname, c.city from customers c, customers d
    ->  where d.rating = c.rating
    ->  having cname = 'hoffman';
+---------+--------+
| cname   | city   |
+---------+--------+
| hoffman | london |
| hoffman | london |
| hoffman | london |
+---------+--------+
3 rows in set (0.00 sec)

KD3_SHAM_83602>
```

# Assignments 11

```
select * from orders
 where cnum = (
 select cnum from customers where cname = 'cisneros');

 SELECT c.cname, c.rating
FROM customers c
WHERE c.cnum IN (
    SELECT o.cnum
    FROM orders o
    GROUP BY o.cnum
    HAVING AVG(o.amt) > (
        SELECT AVG(amt)
        FROM orders
    )
);
 ```
 # Answers
 ```
select total from (select snum , sum(amt) as total from orders group by snum) as totals
where total > (select max(amt) from orders);
KD3_SHAM_83602>select * from orders
    ->  where cnum = (
    ->  select cnum from customers where cname = 'cisneros');
+------+---------+------------+------+------+
| onum | amt     | odate      | cnum | snum |
+------+---------+------------+------+------+
| 3001 |   18.69 | 1990-10-03 | 2008 | 1007 |
| 3006 | 1098.16 | 1990-10-03 | 2008 | 1007 |
+------+---------+------------+------+------+
2 rows in set (0.00 sec)

KD3_SHAM_83602>
KD3_SHAM_83602> SELECT c.cname, c.rating
    -> FROM customers c
    -> WHERE c.cnum IN (
    ->     SELECT o.cnum
    ->     FROM orders o
    ->     GROUP BY o.cnum
    ->     HAVING AVG(o.amt) > (
    ->         SELECT AVG(amt)
    ->         FROM orders
    ->     )
    -> );
+---------+--------+
| cname   | rating |
+---------+--------+
| liu     |    200 |
| clemens |    100 |
+---------+--------+
2 rows in set (0.00 sec)

KD3_SHAM_83602>
KD3_SHAM_83602>select total from (select snum , sum(amt) as total from orders group by snum) as totals
    -> where total > (select max(amt) from orders);
+----------+
| total    |
+----------+
| 15382.07 |
+----------+
1 row in set (0.00 sec)
```
