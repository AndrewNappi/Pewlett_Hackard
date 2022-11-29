# Challenge 7 Written Report

## Overview:
   
    In this challenge I am using SQL queries and schema to put together a database of employees to 
answer important questions for this company. primarily the answers I 
am providing are which employees are more likely to retire soon, 
what departments are they a part of, and which employees are young 
enough to apply for a mentor program.

##Results:

- Our first list is a list of all retiring employees:
    - This list was creted by using the employee number, first name, and last name of the employee from the Employees table and the title, to date, and from date in the Titles table.
    - This tables purpose is to create a list of employees who based on age are getting ready to retire within the next few years.
    - This table is long and part of the reason for that is that there are duplicate employees because each employee has the potential to appear multiple times due to a promotion.
    
- The second list will filter out the duplicates:
    - This list was created using the Distinct On function in SQL. This function filters out all the duplicate occurrances of the individual employee numbers.
    - Much like the last table we have all the employees that may retire in the next few years but this is cut down to only the employees most recent role.
    
- Our next list list shows us numbers of who is retiring:
    - This list is informational it shows based on the title itself how many people they are going to need to replace based souly on what role they had in the company.
    
- The last table shows employees that may be elidgabele for the mentour program:
    - This table has the employee number, first name, last name, and birth date from the employee table joined with the to date, from date, and title from the title table.
    - This table is much shorter than the retiring employees table.
    
    
## Summary

- How many roles will need to be filled as the "silver tsunami" begins to make an impact?
    - The retirement table has all the info for the. To get the number of positions that need filled in the next four years I created queries that show how many people retire in each department.
    
- Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
    - We can tell from the chart how many retirement ready employees we have at the company. In this chart i used queries to return how many employees are in high enough positions to be mentors.
