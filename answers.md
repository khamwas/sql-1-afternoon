/_ create table person
(id Integer primary key autoincrement,
name varchar(100) not null,
age integer,
height float,
city varchar(100),
favorite_color varchar(50));
_/

/_ insert into person
(name, age, height, city, favorite_color)
values('Jon',30,170,'Amarillo','blue'),
('Jacob',35,174,'Canyon','red'),
('Jingle',20,165,'Durango','green'),
('Heimer',40,189,'Plano','yellow'),
('Schmidt',45,250,'Clovis','orange'); _/
  
/_ select _ from person
order by height desc; _/
  
/_ select _ from person
order by height; _/
  
/_ select _ from person
order by age desc; \*/

/_ select _ from person
where age>20; \*/

/_ select _ from person;
where age=18; \*/

/_ select _ from person
where age <20
or age>30; \*/

/_ select _ from person
where age !=27; \*/

/_ select _ from person
where favorite_color='red'; \*/

/_ select _ from person
where favorite_color!='red'
and favorite_color!='blue'; \*/

/_ select _ from person
where favorite_color='orange'
or favorite_color='green'; \*/

/_ select _ from person
where favorite_color in ('green','orange','blue'); \*/

/_ select _ from person
where favorite_color in ('yellow','purple'); \*/

/_ create table orders(
personid integer,
productname varchar(100),
productprice integer,
quantity integer); _/

/_ insert into orders
(personid,productname,productprice,quantity)
values(1,'rogaine',25,15),
(2,'cologne',56,'1'),
(1,'comb',3,1),
(3,'cereal',2,16),
(3,'milk',2,4); _/

/_ select _ from orders; \*/

/_ select total(quantity) from orders; _/

/_ select total(productprice) from orders; _/

/_ select total(productprice) from orders
where personid=3; _/

/_ insert into Artist(Name)
values("T-Swift"),
("Ke$ha"),
("Eminem"); _/

/_ select _ from Artist
order by Name desc
limit 10
; \*/

/_ select _ from Artist
order by Name
limit 5; \*/

/_ select _ from Artist
where Name like 'black%'; \*/

/_ select _ from Artist
where Name like '%black%'; \*/

/_ select FirstName,LastName from employee
where city = 'Calgary'; _/

/_ select max(BirthDate),FirstName,LastName from employee; _/

/_ select min(BirthDate),FirstName,LastName from employee _/

/_ select _ from employee
where ReportsTo = 2; \*/

/_ select count() from employee
where city='Lethbridge'; _/

/_ select count() from invoice
where BillingCountry='USA'; _/

/_ select max(Total) from invoice; _/

/_ select min(Total) from invoice; _/

/_ select _ from invoice
where Total>5; \*/

/_ select count() from invoice
where Total<5; _/

/_ select count() from invoice
where BillingState in ('CA','TX','AZ'); _/

/_ select avg(Total) from invoice; _/

/_ select sum(Total) from invoice; _/
