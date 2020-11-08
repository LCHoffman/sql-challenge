# sql-challenge
SQL project using Postgres

## Database Design
I used QuickDBD to design my Employee database.  I created the tables in QuickDBD in the order of the CSV files.  Once all of my tables were created, I examined the columns to determine the primary and foreign keys for each.  After determining the PK and FK for each table, I added the appropriate data types for each column.  Once I was satisfied with the results, I exported a PNG image of the database, a PDF description of the database and a PostgresSQL table schemata.

## Table Creation
I used pgAdmin 4 to create the tables and work in the database.  I used the schemata exported from QuickDBD to code each table, however I did change the order in which the tables were created.  It was important to be sure that tables were created in the appropriate order to prevent issues with foreign keys.  Since the employee number was a common foreign key, I created this table first.  Next, I created the titles and salaries tables since they only referenced the employee table.  The department table was the next table to be created, since the department number was used as a foreign key in subsequent tables.  Department employees and department managers were created last.  The table schemata file shows the code for creating these tables in the appropriate order.

## Queries
The code for all 8 queries are included in the queries.sql file.  Sample outputs are visible in the Query-result-examples.png file.  The queries required in the homework are listed below.

  1. List the following details of each employee: employee number, last name, first name, sex, and salary.
  2. List first name, last name, and hire date for employees who were hired in 1986.
  3. List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.
  4. List the department of each employee with the following information: employee number, last name, first name, and department name.
  5. List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."
  6. List all employees in the Sales department, including their employee number, last name, first name, and department name.
  7. List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.
  8. In descending order, list the frequency count of employee last names, i.e., how many employees share each last name.
