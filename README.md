for droping table 
drop table employee;
drop table department;



----------------------------------------------------------------------------
sql>
Create table Department(
dept_id Number (10) primary key,
department_name varchar(10)
);
op
SQL query successfully executed. However, the result set is empty.

----------------------------------------------------------------------------
Create table employee(
employee_id number(10) primary key,
employee_name varchar(20) not null,
salary number(20),
Joindate date,
dept_id number(10),
foreign key(dept_id) references department(dept_id)
);
op
table created.
----------------------------------------------------------------------------
query inserting values into department
Insert values into department table 10 rows
sql>
INSERT INTO department(dept_id, department_name) VALUES
(1, 'HR'),
(2, 'Finance'),
(3, 'Sales'),
(4, 'IT'),
(5, 'Marketing'),
(6, 'Operations'),
(7, 'Legal'),
(8, 'Customer Service'),
(9, 'R&D'),
(10, 'Procurement');
output 
inserted successfully.
----------------------------------------------------------------------------
Query Insert values into employee table 50 rows
INSERT ALL 
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(1, 'Alice Johnson', 55000, TO_DATE('2022-01-15', 'YYYY-MM-DD'), 1)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(2, 'Bob Smith', 60000, TO_DATE('2021-03-22', 'YYYY-MM-DD'), 2)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(3, 'Charlie Brown', 75000, TO_DATE('2019-07-30', 'YYYY-MM-DD'), 3)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(4, 'David Wilson', 80000, TO_DATE('2018-05-14', 'YYYY-MM-DD'), 4)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(5, 'Eve Davis', 72000, TO_DATE('2020-09-10', 'YYYY-MM-DD'), 5)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(6, 'Frank Martin', 67000, TO_DATE('2023-02-19', 'YYYY-MM-DD'), 6)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(7, 'Grace Lee', 85000, TO_DATE('2022-06-08', 'YYYY-MM-DD'), 7)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(8, 'Hank Green', 90000, TO_DATE('2017-11-25', 'YYYY-MM-DD'), 8)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(9, 'Ivy White', 95000, TO_DATE('2016-12-03', 'YYYY-MM-DD'), 9)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(10, 'Jack Black', 65000, TO_DATE('2021-04-18', 'YYYY-MM-DD'), 10)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(11, 'Laura White', 56000, TO_DATE('2019-02-20', 'YYYY-MM-DD'), 1)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(12, 'Tom Harris', 61000, TO_DATE('2020-06-15', 'YYYY-MM-DD'), 2)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(13, 'Sandra Adams', 74000, TO_DATE('2021-01-05', 'YYYY-MM-DD'), 3)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(14, 'Alex Carter', 78000, TO_DATE('2018-03-30', 'YYYY-MM-DD'), 4)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(15, 'Linda Moore', 72000, TO_DATE('2019-07-25', 'YYYY-MM-DD'), 5)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(16, 'Walter Scott', 68000, TO_DATE('2023-05-10', 'YYYY-MM-DD'), 6)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(17, 'Barbara Clark', 86000, TO_DATE('2022-08-12', 'YYYY-MM-DD'), 7)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(18, 'Daniel Lewis', 93000, TO_DATE('2017-09-14', 'YYYY-MM-DD'), 8)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(19, 'Nancy Allen', 95000, TO_DATE('2016-05-22', 'YYYY-MM-DD'), 9)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(20, 'Patrick Turner', 67000, TO_DATE('2020-02-28', 'YYYY-MM-DD'), 10)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(21, 'Rebecca Nelson', 54000, TO_DATE('2018-12-10', 'YYYY-MM-DD'), 1)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(22, 'Keith Wright', 62000, TO_DATE('2019-04-18', 'YYYY-MM-DD'), 2)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(23, 'Jennifer Hill', 76000, TO_DATE('2020-09-07', 'YYYY-MM-DD'), 3)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(24, 'Andrew King', 81000, TO_DATE('2021-06-14', 'YYYY-MM-DD'), 4)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(25, 'Megan Baker', 73000, TO_DATE('2019-11-20', 'YYYY-MM-DD'), 5)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(26, 'Zachary Campbell', 69000, TO_DATE('2023-03-23', 'YYYY-MM-DD'), 6)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(27, 'Melissa Young', 87000, TO_DATE('2022-02-01', 'YYYY-MM-DD'), 7)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(28, 'Philip Perez', 91000, TO_DATE('2018-04-29', 'YYYY-MM-DD'), 8)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(29, 'Emily Hall', 96000, TO_DATE('2017-10-03', 'YYYY-MM-DD'), 9)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(30, 'Richard Allen', 65000, TO_DATE('2021-08-21', 'YYYY-MM-DD'), 10)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(31, 'Deborah Rodriguez', 53000, TO_DATE('2018-01-30', 'YYYY-MM-DD'), 1)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(32, 'Harold Stewart', 64000, TO_DATE('2020-05-18', 'YYYY-MM-DD'), 2)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(33, 'Diana Sanchez', 78000, TO_DATE('2021-11-05', 'YYYY-MM-DD'), 3)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(34, 'Jackie Bell', 80000, TO_DATE('2018-06-06', 'YYYY-MM-DD'), 4)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(35, 'Vincent Mitchell', 71000, TO_DATE('2019-08-10', 'YYYY-MM-DD'), 5)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(36, 'Katherine Collins', 67000, TO_DATE('2023-07-19', 'YYYY-MM-DD'), 6)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(37, 'Betty Reed', 86000, TO_DATE('2022-10-28', 'YYYY-MM-DD'), 7)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(38, 'Arthur Morgan', 89000, TO_DATE('2017-05-01', 'YYYY-MM-DD'), 8)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(39, 'Gloria Rivera', 95000, TO_DATE('2016-07-13', 'YYYY-MM-DD'), 9)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(40, 'Bruce Cooper', 62000, TO_DATE('2020-12-25', 'YYYY-MM-DD'), 10)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(41, 'Sara Morris', 55000, TO_DATE('2019-01-20', 'YYYY-MM-DD'), 1)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(42, 'Ethan Jenkins', 61000, TO_DATE('2020-03-25', 'YYYY-MM-DD'), 2)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(43, 'Sophia Foster', 74000, TO_DATE('2021-05-10', 'YYYY-MM-DD'), 3)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(44, 'Brian Cook', 82000, TO_DATE('2018-09-15', 'YYYY-MM-DD'), 4)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(45, 'Olivia Brooks', 71000, TO_DATE('2019-04-05', 'YYYY-MM-DD'), 5)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(46, 'Lucas Sanders', 69000, TO_DATE('2023-01-30', 'YYYY-MM-DD'), 6)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(47, 'Lily Ross', 88000, TO_DATE('2022-04-17', 'YYYY-MM-DD'), 7)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(48, 'Adam Perez', 91000, TO_DATE('2021-03-08', 'YYYY-MM-DD'), 8)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(49, 'Emma Clark', 74000, TO_DATE('2023-02-21', 'YYYY-MM-DD'), 9)
INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES(50, 'Oliver Scott', 68000, TO_DATE('2020-05-11', 'YYYY-MM-DD'), 10)
SELECT * FROM dual;
output
successfully inserted.

----------------------------------------------------------------------------

query   do operation on select, where, like, between, and is null, not nullm, exists
1] where operation
select * from employee
where salary<=55000;
output -
employee_id	employee_name	salary	Joindate	dept_id
1	Alice Johnson	55000	2022-01-15		1
21	Rebecca Nelson	54000	2018-12-10		1
31	Deborah 	53000	2018-01-30		1
41	Sara Morris	55000	2019-01-20		1

----------------------------------------------------------------------------
 query   select salary between 50000 and 65000
sql> 
SELECT * FROM employee
 where salary BETWEEN 50000 AND 65000;
 output
employee_id	employee_name	salary	Joindate	dept_id
1	Alice Johnson	55000	2022-01-15		1
2	Bob Smith	60000	2021-03-22		2
10	Jack Black	65000	2021-04-18		10
11	Laura White	56000	2019-02-20		1
12	Tom Harris	61000	2020-06-15		2
21	Rebecca Nelson	54000	2018-12-10		1
22	Keith Wright	62000	2019-04-18		2
30	Richard Allen	65000	2021-08-21		10
31	Deborah Rodriguez	53000	2018-01-30	1
32	Harold Stewart	64000	2020-05-18		2
40	Bruce Cooper	62000	2020-12-25		10
----------------------------------------------------------------------------
query->
operation on like 
sql>
SELECT * FROM employee
    WHERE employee_name LIKE 'A%';
output 
employee_id	employee_name	salary	Joindate	dept_id
1	Alice Johnson	55000	2022-01-15	1
14	Alex Carter	78000	2018-03-30	4
24	Andrew King	81000	2021-06-14	4
38	Arthur Morgan	89000	2017-05-01	8
49	Anna Butler	94000	2017-12-09	9
----------------------------------------------------------------------------
query usin 'and' operation and using two operations

sql>
SELECT * FROM employee
WHERE salary = 55000 AND employee_name LIKE 'A%';
output
employee_id	employee_name	salary	Joindate	dept_id
1	Alice Johnson	55000	2022-01-15	1
----------------------------------------------------------------------------
Query to use.in operation 
sql>
SELECT employee_id,employee_name
FROM employee
WHERE salary IN (55000,60000,75000);

o/p
"1"	"Alice Johnson"
"2"	"Bob Smith"
"3"	"Charlie Brown"
"41"	"Sara Morris"
----------------------------------------------------------------------------
Query. Using alter operation. 
 sql>
ALTER TABLE employees
ADD age INT;

o/p inserted.
 2.
sql>
alter table abhi 
drop column address;
o/p
deleted .
   ...modify....
..rename ->
sql>
ALTER TABLE abhi
RENAME abhi_salary to salary;
o/p 
renamed>
QUERY: CHANGING TABLE NAME :
SQL>
ALTER TABLE FOR_ALTER
RENAME TO ABHI;
O.P-
CHANGED SUCESSFULLY
----------------------------------------------------------------------------

TO USE UPDATE AND SET 
QUERY : TO CHANE THE VALUE AS NULL
SQL>
UPDATE  XYZ 
SET salary = NULL
WHERE employee_id= 50;
O/P: "50"	"null"
-- WITHOUT UPDATE WE CANT USE SET
query: now changing value gain  to value
SELECT * from xyz
where employee_id = 50;
o/p:
"50"	"Henry Torres"	"55000"	"2021-03-11"	"10"
----------------------------------------------------------------------------
QUERY : TO SHOW ONLY TOTAL SALARY OF ALL EMPLOYEE
SQL>
SELECT  sum(salary)
FROM employee
ORDER BY salary DESC
LIMIT 1;
O/P
"3745000"
----------------------------------------------------------------------------
QUERY : TO SHOW WHO HAS MAX SALARY 
SQL>
SELECT  employee_id,employee_name,MAX(salary)
FROM employee
ORDER BY salary DESC
LIMIT 1;
O/P-
"29"	"Emily Hall"	"96000".
----------------------------------------------------------------------------
query : using order by 
sql>
 select EMPLOYEE_ID,EMPLOYEE_NAME from xyz
  2  where salary <=55000
  3  order by salary;
  o/p
  EMPLOYEE_ID EMPLOYEE_NAME
----------- --------------------
         31 Deborah Rodriguez
         21 Rebecca Nelson
          1 Alice Johnson
         41 Sara Morris
----------- -------------------- 
SQL> create table products(
  2  product_id number(20) primary key ,
  3  product_name varchar(20) not null,
  4  prize number(20),
  5  category varchar2(20));

Table created.
----------- -------------------- 
SQL> INSERT ALL
  2      INTO products (product_id, product_name, prize, category) VALUES (1, 'Laptop', 1500, 'Electronics')
  3      INTO products (product_id, product_name, prize, category) VALUES (2, 'Smartphone', 800, 'Electronics')
  4      INTO products (product_id, product_name, prize, category) VALUES (3, 'Washing Machine', 600, 'Home Appliances')
  5      INTO products (product_id, product_name, prize, category) VALUES (4, 'Refrigerator', 1000, 'Home Appliances')
  6      INTO products (product_id, product_name, prize, category) VALUES (5, 'Headphones', 150, 'Accessories')
  7      INTO products (product_id, product_name, prize, category) VALUES (6, 'Smartwatch', 250, 'Accessories')
  8      INTO products (product_id, product_name, prize, category) VALUES (7, 'Microwave', 200, 'Home Appliances')
  9      INTO products (product_id, product_name, prize, category) VALUES (8, 'Coffee Maker', 120, 'Home Appliances')
 10      INTO products (product_id, product_name, prize, category) VALUES (9, 'TV', 500, 'Electronics')
 11      INTO products (product_id, product_name, prize, category) VALUES (10, 'Camera', 350, 'Electronics')
 12  SELECT * FROM dual;

10 rows created.
----------- -------------------- 
SQL> create table departments(
  2    dept_id number(20) primary key,
  3    dept_name varchar(20) not NULL,
  4    location varchar(20));

Table created.
----------- --------------------
SQL> insert all
  2   INTO departments (dept_id, dept_name, location) VALUES (1, 'HR', 'New York')
  3   INTO departments (dept_id, dept_name, location) VALUES (2, 'IT', 'San Francisco')
  4   INTO departments (dept_id, dept_name, location) VALUES (3, 'Finance', 'London')
  5   INTO departments (dept_id, dept_name, location) VALUES (4, 'Marketing', 'Los Angeles')
  6   INTO departments (dept_id, dept_name, location) VALUES (5, 'Sales', 'Chicago')
  7   INTO departments (dept_id, dept_name, location) VALUES (6, 'R&D', 'Berlin')
  8   INTO departments (dept_id, dept_name, location) VALUES (7, 'Customer Support', 'Toronto')
  9   INTO departments (dept_id, dept_name, location) VALUES (8, 'Legal', 'Paris')
 10   INTO departments (dept_id, dept_name, location) VALUES (9, 'Operations', 'Tokyo')
 11   INTO departments (dept_id, dept_name, location) VALUES (10, 'Product Management', 'Sydney')
 12  select * from dual;
10 rows created.
----------- --------------------
  select product_name,category from products
  2    where prize > 1000;

PRODUCT_NAME         CATEGORY
-------------------- --------------------
Laptop               Electronics
----------- --------------------
CREATE table works(
  employee_id number(20) PRIMARY key,
  company_name varchar(20) not null,
  salary number(20));
  
Table created.
----------- --------------------
SQL> insert all
  2   INTO works (employee_id, company_name, salary) VALUES (2, 'HealthInc', 75000)
  3   INTO works (employee_id, company_name, salary) VALUES (3, 'FinGlobal', 90000)
  4   INTO works (employee_id, company_name, salary) VALUES (4, 'EduSolutions', 65000)
  5   INTO works (employee_id, company_name, salary) VALUES (5, 'RetailPlus', 55000)
  6   INTO works (employee_id, company_name, salary) VALUES (6, 'AutoMotives', 70000)
  7   INTO works (employee_id, company_name, salary) VALUES (7, 'TechCorp', 85000)
  8   INTO works (employee_id, company_name, salary) VALUES (8, 'RetailPlus', 60000)
  9   INTO works (employee_id, company_name, salary) VALUES (9, 'HealthInc', 77000)
 10   INTO works (employee_id, company_name, salary) VALUES (10, 'FinGlobal', 95000)
 11  select * from dual;

9 rows created.
----------- --------------------
--INSERT INTO works (employee_id, company_name, salary) VALUES (1, 'TechCorp', 80000);
sql>select avg(salary) as avg_salary from works;
avg_salary
"75200"
----------- --------------------
sql>select dept_name,location from departments
where location like 's%';
"IT"	"San Francisco"
"Product Management"	"Sydney"
----------- --------------------
sql>SELECT DISTINCT(company_name) from works;
"TechCorp"
"HealthInc"
"FinGlobal"
"EduSolutions"
"RetailPlus"
"AutoMotives"

----------- --------------------
--29|11|24
create table employe_09(
   employee_id number(10) primary key,
   employee_name varchar2(20),
    dob date,
    salary number(10),
    doj date,
    qualification varchar(20));
o/p : table created
----------- --------------------
INSERT
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(1, 'John Doe', TO_DATE('1990-05-15', 'YYYY-MM-DD'), 50000, TO_DATE('2015-06-01', 'YYYY-MM-DD'), 'MBA'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(2, 'Jane Smith', TO_DATE('1985-11-22', 'YYYY-MM-DD'), 55000, TO_DATE('2016-08-20', 'YYYY-MM-DD'), 'B.Tech'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(3, 'Emily Clark', TO_DATE('1992-03-30', 'YYYY-MM-DD'), 48000, TO_DATE('2017-01-10', 'YYYY-MM-DD'), 'M.Sc'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(4, 'Michael Johnson', TO_DATE('1988-07-14', 'YYYY-MM-DD'), 60000, TO_DATE('2014-09-15', 'YYYY-MM-DD'), 'BBA'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(5, 'Sarah Brown', TO_DATE('1995-02-01', 'YYYY-MM-DD'), 45000, TO_DATE('2019-03-25', 'YYYY-MM-DD'), 'BCA'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(6, 'David Wilson', TO_DATE('1987-12-10', 'YYYY-MM-DD'), 65000, TO_DATE('2013-07-22', 'YYYY-MM-DD'), 'M.Tech'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(7, 'Olivia Martin', TO_DATE('1994-06-18', 'YYYY-MM-DD'), 70000, TO_DATE('2020-01-01', 'YYYY-MM-DD'), 'MCA'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(8, 'James Anderson', TO_DATE('1983-10-25', 'YYYY-MM-DD'), 75000, TO_DATE('2012-04-10', 'YYYY-MM-DD'), 'PhD'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(9, 'Sophia Lee', TO_DATE('1990-08-05', 'YYYY-MM-DD'), 52000, TO_DATE('2018-05-30', 'YYYY-MM-DD'), 'B.Com'),
INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES(10, 'William Taylor', TO_DATE('1986-01-12', 'YYYY-MM-DD'), 56000, TO_DATE('2011-11-05', 'YYYY-MM-DD'), 'M.A');
o/p :
rows inserted
----------- --------------------
 q) creating view
 sql>create view e.info as 
select employee_id,employee_name,salary 
from employe_09;
o/p: view created
-- to vieew 
sql> select * from einfo
----------- --------------------
q)pl/sql query
sql>
set serveroutputon :
create or replace procedure greet_user(p_name in varchar2) AS
begin 
  DBMS_OUTPUT.PUT_LINE('HELLO,'||p_name||'!');
end; 
/ 
--1stpart end

--excuting the program
sql>
begin 
  greet_user('john');
end;
/
-- 2 nd part end
----------- --------------------
-- trigger
create or replace trigger etriger
after insert on employe_09
for each row 
begin 
   DBMS_OUTPUT.PUT_LINE('new employee added:'||:new.employee_name);
end;
/
-- then add a new row
INSERT INTO employe_09 (employee_id, employee_name, dob, salary, doj, qualification) VALUES
(7, 'Olivia Martin', TO_DATE('1994-06-18', 'YYYY-MM-DD'), 70000, TO_DATE('2020-01-01', 'YYYY-MM-DD'), 'MCA');

----------- --------------------
q) a function to return the current the current system date
 sql>
create or replace function get_sydate
return date as 
begin 
  return get_sydate;
end get_sydate;
o/p: function created .
select sydate from dual;

A FUNCTON TO CALCULATE THESQUARE OF A NUMBER
sql>
create or replace function calculate_square(
 pnumber in number 
) return number as 
begin 
  return pnumber*pnumber;
end calculate_square;
a set of code to add code in sql ,
-------------------------------------

COMMIT;
