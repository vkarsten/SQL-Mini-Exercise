1. Write a SQL statement to create a simple table countries including columns country_id,country_name and region_id.
- CREATE TABLE countries (country_id int, country_name varchar(255), region_id int);
2. Write a SQL statement to create a simple table countries including columns country_id,country_name and region_id which already exist.
- CREATE TABLE countries (country_id int, country_name varchar(255), region_id int); 
3. Write a SQL statement to create the structure of a table dup_countries similar to countries.
- create table dup_countries as (select * from countries) with no data;
4. Write a SQL statement to create a duplicate copy of countries table including structure and data by name dup_countries.
- create table dup_countries as (select * from countries);
5. Write a SQL statement to create a table countries set a constraint NULL.
- CREATE TABLE countries (country_id int NOT NULL, country_name varchar(255) NOT NULL, region_id int NOT NULL);
6. Write a SQL statement to create a table named jobs including columns job_id, job_title, min_salary, max_salary and check whether the max_salary amount exceeding the upper limit 25000.
- CREATE TABLE jobs (job_id int, job_title varchar(80), min_salary float, max_salary float CHECK (max_salary < 25000));
7. Write a SQL statement to create a table named countries including columns country_id, country_name and region_id and make sure that no countries except Italy, India and China will be entered in the table.
- CREATE TABLE countries (country_id int, country_name varchar(255), region_id int CHECK (country_name IN ('Italy', 'India', 'China')));
8. Write a SQL statement to create a table named countries including columns country_id,country_name and region_id and make sure that no duplicate data against column country_id will be allowed at the time of insertion.

9. Write a SQL statement to create a table named jobs including columns job_id, job_title, min_salary and max_salary, and make sure that, the default value for job_title is blank and min_salary is 8000 and max_salary is NULL will be entered automatically at the time of insertion if no value assigned for the specified columns.

10. Write a SQL statement to create a table named countries including columns country_id, country_name and region_id and make sure that the country_id column will be a key field which will not contain any duplicate data at the time of insertion.

11. Write a SQL statement to create a table countries including columns country_id, country_name and region_id and make sure that the column country_id will be unique and store an auto-incremented value.

12. Write a SQL statement to create a table countries including columns country_id, country_name and region_id and make sure that the combination of columns country_id and region_id will be unique.
