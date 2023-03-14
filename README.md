# sql_fsd

Q>Car rental system - Create Table 

Refer to the given schema. 

Q>Write a query to create the Owners table with the specified columns and constraints. 

Note: Letters in bold represents the table name 

Note: Maintain the same sequence of column order, as specified in the question description 

Q>Cars not taken for rent 

Q>Write a query to display car id, car name, car type of cars which was not taken for rent. Sort the result based on car id. 

HINT: Use Cars and Rentals tables to retrieve records. 

NOTE: Maintain the same sequence of column order, as specified in the question description 

Q>Car & owner details based on car type 

Q>Write a query to display car id, car name and owner id of all the cars whose car type is 'Hatchback' or 'SUV'. Sort the result based on car id. 

(Hint: Use CARS tables to retrieve records. Data is case-sensitive. E.g: Car_type='Hatchback'. Use IN operator) 

NOTE: Maintain the same sequence of column order, as specified in the question description 

Q>Car rental system - add new column 

Q>Refer to the given schema. Assume, CARS table has been already created. Write an appropriate query for the given requirement. 
Requirement 1: Add a new column Car_Regno VARCHAR(10) to the Cars table. 

Note: Letters in the bold represents the attribute name. 

Q>Car details based on type and name 

Q>Write a query to display car id, car name and car type of Maruthi company 'Sedan' type cars. Sort the result based on car id. 

(HINT : Use Cars table to retrieve records.car name='Maruthi Swift'.car type='Sedan'.Data is case sensitive.) 

NOTE: Maintain the same sequence of column order, as specified in the question description 

Q>Maruthi car owner details 

Q>Write a query to display distinct owner id, owner name, address, and phone no of owners who owns 'Maruthi' company car. Sort the result based on owner id. 

Note: If car_name contains a string 'Maruthi' it is a Maruthi company car. 

Example: 'Maruthi swift','Maruthm nn n i 800' 

HINT: Use Owners and Cars tables to retrieve records. 

NOTE: Maintain the same sequence of column order, as specified in the question description 

Q>car rental system - Insert values 

Q>Refer to the given schema diagram. Insert the below records into Rentals Table. Assume the rentals table has been already created. 

Q>Shape table data 

Note: Letters in bold represent the attributes. 

NOTE: Maintain the same sequence of column order, as specified in the question description 

Q>Rental details based on date 

Q>Write a query to display rental id, car id, customer id and km driven of rentals taken during 'AUGUST 2019'. Sort the result based on rental id. 

(HINT : Use Rentals table to retrieve records. Eg: return date: 2019-08-12 ) 

NOTE: Maintain the same sequence of column order, as specified in the question description 

Q>No of time rented by each car 

Q>Write a query to display car id and number of times car taken for rental. Give an alias name to the number of times car taken for rental as 'NO_OF_TRIPS'. Sort the records based on car id in ascending order. 

(HINT: Use Rentals table to retrieve records.) 

Q>Shape database diagram 

 Q>1. Create a employee table and department table  

CREATE TABLE Employee ( 

    employee_id INT NOT NULL AUTO_INCREMENT, 

    first_name VARCHAR(50) NOT NULL, 

    last_name VARCHAR(50) NOT NULL, 

    email VARCHAR(100) UNIQUE NOT NULL, 

    phone VARCHAR(20), 

    hire_date DATE NOT NULL, 

    job_title VARCHAR(50) NOT NULL, 

    department_id INT NOT NULL, 

    salary DECIMAL(10,2) NOT NULL, 

    PRIMARY KEY (employee_id), 

    FOREIGN KEY (department_id) REFERENCES Department(department_id) 

); 

CREATE TABLE Department ( 

    department_id INT NOT NULL AUTO_INCREMENT, 

    department_name VARCHAR(50) NOT NULL, 

    manager_id INT, 

    location VARCHAR(100), 

    PRIMARY KEY (department_id) 

); 

2.Write a query to fetch the first_name from the Employee table in the upper case and use the ALIAS name as EmpName. 

3.Write a query to fetch the number of employees working in the department ‘HR’. 

4. Write a query to get the current date. 

5.Write a query to retrieve the first four characters of  EmpLname from the EmployeeInfo table. 

6.Write a query to fetch only the place name(string before brackets) from the Address column of EmployeeInfo table. 

7.Write a query to create a new table that consists of data and structure copied from the other table. 

8. Write q query to find all the employees whose salary is between 50000 to 100000. 

9. Write a query to find the names of employees that begin with ‘S’. 

10. Write a query to fetch top N records. 

11. Write a query to retrieve the EmpFname and EmpLname in a single column as “FullName”. The first name and the last name must be separated with space. 

