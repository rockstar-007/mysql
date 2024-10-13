# mysql
sql>
Create table Department(
dept_id Number (10) primary key,
department_name varchar(10)
);
op
SQL query successfully executed. However, the result set is empty.
----------------------------------------------------------------------------
sql>
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
query--> inserting values into department
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
Query--Insert values into employee table 50 rows
INSERT INTO employee (employee_id, employee_name, salary, Joindate, dept_id) VALUES
(1, 'Alice Johnson', 55000, '2022-01-15', 1),
(2, 'Bob Smith', 60000, '2021-03-22', 2),
(3, 'Charlie Brown', 75000, '2019-07-30', 3),
(4, 'David Wilson', 80000, '2018-05-14', 4),
(5, 'Eve Davis', 72000, '2020-09-10', 5),
(6, 'Frank Martin', 67000, '2023-02-19', 6),
(7, 'Grace Lee', 85000, '2022-06-08', 7),
(8, 'Hank Green', 90000, '2017-11-25', 8),
(9, 'Ivy White', 95000, '2016-12-03', 9),
(10, 'Jack Black', 65000, '2021-04-18', 10),
(11, 'Laura White', 56000, '2019-02-20', 1),
(12, 'Tom Harris', 61000, '2020-06-15', 2),
(13, 'Sandra Adams', 74000, '2021-01-05', 3),
(14, 'Alex Carter', 78000, '2018-03-30', 4),
(15, 'Linda Moore', 72000, '2019-07-25', 5),
(16, 'Walter Scott', 68000, '2023-05-10', 6),
(17, 'Barbara Clark', 86000, '2022-08-12', 7),
(18, 'Daniel Lewis', 93000, '2017-09-14', 8),
(19, 'Nancy Allen', 95000, '2016-05-22', 9),
(20, 'Patrick Turner', 67000, '2020-02-28', 10),
(21, 'Rebecca Nelson', 54000, '2018-12-10', 1),
(22, 'Keith Wright', 62000, '2019-04-18', 2),
(23, 'Jennifer Hill', 76000, '2020-09-07', 3),
(24, 'Andrew King', 81000, '2021-06-14', 4),
(25, 'Megan Baker', 73000, '2019-11-20', 5),
(26, 'Zachary Campbell', 69000, '2023-03-23', 6),
(27, 'Melissa Young', 87000, '2022-02-01', 7),
(28, 'Philip Perez', 91000, '2018-04-29', 8),
(29, 'Emily Hall', 96000, '2017-10-03', 9),
(30, 'Richard Allen', 65000, '2021-08-21', 10),
(31, 'Deborah Rodriguez', 53000, '2018-01-30', 1),
(32, 'Harold Stewart', 64000, '2020-05-18', 2),
(33, 'Diana Sanchez', 78000, '2021-11-05', 3),
(34, 'Jackie Bell', 80000, '2018-06-06', 4),
(35, 'Vincent Mitchell', 71000, '2019-08-10', 5),
(36, 'Katherine Collins', 67000, '2023-07-19', 6),
(37, 'Betty Reed', 86000, '2022-10-28', 7),
(38, 'Arthur Morgan', 89000, '2017-05-01', 8),
(39, 'Gloria Rivera', 95000, '2016-07-13', 9),
(40, 'Bruce Cooper', 62000, '2020-12-25', 10),
(41, 'Sara Morris', 55000, '2019-01-20', 1),
(42, 'Ethan Jenkins', 61000, '2020-03-25', 2),
(43, 'Sophia Foster', 74000, '2021-05-10', 3),
(44, 'Brian Cook', 82000, '2018-09-15', 4),
(45, 'Olivia Brooks', 71000, '2019-04-05', 5),
(46, 'Lucas Sanders', 69000, '2023-01-30', 6),
(47, 'Lily Ross', 88000, '2022-04-17', 7),
(48, 'Benjamin Ramirez', 92000, '2018-07-22', 8),
(49, 'Anna Butler', 94000, '2017-12-09', 9),
(50, 'Henry Torres', 66000, '2021-03-11', 10);
output
successfully inserted.
----------------------------------------------------------------------------
query--> do operation on select, where, like, between, and is null, not nullm, exists
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
 query --> select salary between 50000 and 65000
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
for droping table 
sql>
drop table employee;
drop table department;
