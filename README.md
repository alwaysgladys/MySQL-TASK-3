# Data Manipulation
# Introduction:
This very SQL data manipulation was carried out within MySQL Database.
The objective of data manipulation for this task is to replace, update, query and arrange relevant information within the tables from the database. 
From this task, I was able to retrieve data, replace data, merge data, modify data, run queries and present results within MySQL Workbench.


# Problem Statement:
1. Replace the Department ‘Communications’ with ‘Stakeholders’ and show the result of the replacement done.

2. Update the ‘Name’ column ensuring that the values are all in UPPER CASE.

3. Run a query that will show the employer's name and DOE in one column as the Employer’s brief.

4. Run a query that will remove leading spaces from the name column If exists.

# Solution:

![stakeholders department](https://github.com/alwaysgladys/MySQL-TASK-3/assets/144185133/fcfdf087-cb7c-4819-9c17-75e2006b81a7)

the Image above shows the replacement made to the 'Department'; from Communications to Stakeholders. The syntax used for this task reads;

UPDATE table_name 
SET department = 'Stakeholders'
WHERE department = 'Communications';


![UPPER NAMES](https://github.com/alwaysgladys/MySQL-TASK-3/assets/144185133/0320865e-b620-4b6b-8090-f3056b2592ef)

In this image, the name column was updated with values in Uppercase. This was achieved with the following synatx:
SELECT UPPER(Name) AS Name


![Employee's brief](https://github.com/alwaysgladys/MySQL-TASK-3/assets/144185133/23106433-8628-494b-838e-481fa0037184)


This very image displays the merged columns of the employee's name and their date of entry. This was achieved with the following syntax:
SELECT CONCAT(employee_name, '', Date_of_Entry) AS Employee's brief
FROM table_name;


There was no leading spaces in our name column For task number 4. But for the purpose of any future leading space, it will make use of TRIM to trim the leading spaces.
you can achieve that by using the syntax:
SELECT TRIM(Name) AS NAMES FROM Employee_Info;

# Conclusion:

Through the process of data manipulation in SQL for this given task, I gained valuable experience in effectively extracting and processing information from a database.
This task underscored the importance of precision and attention to detail, especially when crafting queries to filter and aggregate data.

I learned how to leverage SQL's powerful features, such as SELECT, WHERE, SET, CONCAT, TRIM, UPDATE and UPPER functions, to distill raw data into meaningful insights.

Overall, this experience has deepened my proficiency in SQL data manipulation and reinforced its pivotal role in generating actionable insights from databases. It serves as a foundation for more complex analyses and problem-solving in future endeavors.
