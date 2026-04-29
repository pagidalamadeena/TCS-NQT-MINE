✅MySQL:

* MySQL is an open‑source relational database management system (RDBMS).
* It uses SQL (Structured Query Language) to store, manage, and retrieve data.
* A database is an organized collection of data stored so it can be easily accessed and managed.



✅Types of Databases:
1 . Relational (MySQL, PostgreSQL)
2 . Non‑relational (MongoDB)



✅SQL commands are grouped as:
DQL (Data Query Language): Retrieves data.
SELECT
DML (Data Manipulation Language): Inserts, updates, deletes records.
INSERT, UPDATE, DELETE
DDL (Data Definition Language): Defines database structure.
CREATE, ALTER, DROP
DCL (Data Control Language): Controls access.
GRANT, REVOKE
TCL (Transaction Control Language): Manages transactions
COMMIT, ROLLBACK, SAVEPOINT



✅Normalization: Process of organizing data to reduce redundancy.
Common forms:
1NF: No repeating groups.
2NF: No partial dependency.
3NF: No transitive dependency.



✅Indexes: Improve the speed of selecting data. Like an index in a book.
Types:
Primary index
Unique index
Composite index



✅Constraints:-
NOT NULL – field can’t be empty
UNIQUE – unique values only
PRIMARY KEY
FOREIGN KEY
CHECK – validates condition
DEFAULT – auto value if not provided



✅Transactions:- Group multiple queries as a single unit.
Properties (ACID):

* Atomicity
* Consistency
* Isolation
* Durability



✅Aggregate functions:
count()
sum()
avg()
max()
min()



✅ Stored Procedures
Pre‑compiled SQL code reused multiple times.
Definition:
Stored procedures are SQL scripts stored in the DB that can perform operations like insert, update, delete, and complex logic.
CREATE PROCEDURE getAllEmployees()
BEGIN
SELECT  \* FROM employees;
END;



✅ Cursors
Used to process rows one at a time.
Definition:
Cursor is a database object used for row‑by‑row operations when set‑based operations are not possible (but generally discouraged).



✅ Triggers
Triggers run automatically when an event occurs (INSERT/UPDATE/DELETE events).
Definition:
A trigger is a stored program in SQL that is executed automatically when a specified event occurs.
CREATE TRIGGER before\_insert\_emp
BEFORE INSERT ON employees
FOR EACH ROW
SET NEW.created\_at = NOW();



✅ Views
A virtual table created using a SELECT query. Virtual table based on query results. Does not store data physically.
Definition:
View does not store data; it presents data from one or more tables for simplification and security.



✅ Indexes
Improve read performance.
Definition:
An index is a database object that speeds up searches by creating a pointer structure (like an index in a book).



Delete table + data: DROP TABLE table\_name;

"Delete": only rows/data is removed
"Drop": table + data is removed
"Alter": change table structure

RENAME TABLE NAME: ALTER TABLE old\_table\_name RENAME TO new\_table\_name;
RENAME COUMN NAME: ALTER TABLE employees RENAME COLUMN old\_column TO new\_column;
ADD NEW COLUMN: ALTER TABLE employees ADD salary INT;



🔄Sample code/syntax:

create database school\_db;

use school\_db;



create table students (

student\_id int primary key,

student\_name varchar(30),

age int,

teacher\_id int

);

create table teacher(

teacher\_id int primary key,

teacher\_name varchar(30),

subject varchar(20)

);



insert into teacher values

(1, 'Ravi', 'Maths'),

(2,'Meena','Science'),

(3,'John','English');



insert into students values

(101,'Arun',18,1),

(102,'Divya',17,2),

(103,'Kiran',18,1),

(104,'Priya',17,NULL);



select  \* from students;

select  \* from teacher;



select  \* from students order by age desc;



select student\_name,age from students where age=18;



update students set age=19 where student\_id=101;



delete from students where student\_id=104;



alter table students add foreign key (teacher\_id) references teacher(teacher\_id);



select avg(age) as average\_age from students;



select teacher\_id, count(\*) as total\_students from student group by teacher\_id; \[Counts students per teacher]



select teacher\_id, count(*) as total\_students from student group by teacher\_id having count(*)>1; \[Show only teachers who have more than 1 student]



🔄JOINS:
INNER JOIN → Matching rows only
LEFT JOIN → All left + matching right
RIGHT JOIN → All right + matching left
FULL JOIN → Everything from both
CROSS JOIN → All combinations
SELF JOIN → Same table joined to itself

1 . Inner join:(Shows only matching records in both tables)

select students.student\_name, teacher.teacher\_name

from students

inner join teacher

on students.teacher\_id=teacher.teacher\_id;



2.Left join: (Shows all students + matching teachers)->(gives all students details even if there is no teacher)

select students.student\_name, teacher.teacher\_name

from students

left join teacher

on students.teacher\_id=teacher.teacher\_id;



3 . Right join: (Shows all teachers + matching students)->(gives all teachers even there are no students)

select students.student\_name, teacher.teacher\_name

from students

right join teacher

on students.teacher\_id=teacher.teacher\_id;



4 . FULL join: MySQL doesn't support FULL JOIN directly, so use:

select students.student\_name, teacher.teacher\_name

from students

left join teacher

on students.teacher\_id=teacher.teacher\_id;

union

select students.student\_name, teacher.teacher\_name

from students

right join teacher

on students.teacher\_id=teacher.teacher\_id;

\------------------------------------------------------------

🔄Copilot gave this as examples for each join:

SELECT s.student\_name, t.teacher\_name

FROM students s

INNER JOIN teacher t

ON s.teacher\_id = t.teacher\_id;



SELECT s.student\_name, t.teacher\_name

FROM students s

LEFT JOIN teacher t

ON s.teacher\_id = t.teacher\_id;



SELECT s.student\_name, t.teacher\_name

FROM students s

RIGHT JOIN teacher t

ON s.teacher\_id = t.teacher\_id;



SELECT s.student\_name, t.teacher\_name

FROM students s

FULL OUTER JOIN teacher t

ON s.teacher\_id = t.teacher\_id;

(Not supported in MySQL — needs UNION workaround)



SELECT s.student\_name, t.teacher\_name

FROM students s

CROSS JOIN teacher t;

\---

