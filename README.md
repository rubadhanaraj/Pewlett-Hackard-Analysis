# Pewlett-Hackard-Analysis
## Overview of the analysis
The purpose of the analysis is analyse the workforce of Pewlett-Hackard. As most of the employees are reaching their retirement age, PH needs to be ready to face the Silver Tsunami, which will result in a significant number of job openings in the company. PH is planning to handle the silver tsunami by designating a group of retirees as mentors to train the new hires of workers so that Pewlett Hackard's day-to-day activities could be handled well. Using Structured Query Language, all the csv files have been analysed by various functions and new addditional csv files were genarated which were helpful for the PH analysis 

## Results
The analysis was started with only six CSV files(Employees,Departments,Dat_emp,Dept_manager,Titles,Salaries) and no real database or data management system in place. A model of the database was created with an Entity Relationship Diagram, and with the help of ERD many queries were performed to help PH future-proof the company. 

![data-7-3-2-1-review-the-ERD-for-common-columns](https://user-images.githubusercontent.com/108298416/184467062-669511a2-3005-41bc-8955-96b181a114dd.png)

Using SQL queries, a Retirement Titles table was created that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees might have multiple titles in the database, due to promotions  DISTINCT ON statement was used to create a table that contains the most recent title of each employee. COUNT() function was used to create a table that has the number of retirement-age employees by most recent job title. 

![image](https://user-images.githubusercontent.com/108298416/184467949-b458d4ca-4deb-4587-8772-9acbd57b9d54.png)

Similarly, a mentorship-eligibility table was created that holds the current employees who were born between January 1, 1965 and December 31, 1965.

![image](https://user-images.githubusercontent.com/108298416/184467964-6608161d-f54b-4877-bdd9-98e6c533e010.png)

* The retiring_titles csv, shows that the largest retiring amount of employees are senior Engineers with the count of 25916, followed by senior staff.
* The mentorship eligibility csv result shows that there are 1549 employees are eligible for mentoring the new hires.
* The majority of retiring employees have so many years of hands on experience in Pewlett Hackard. To replace them with new hires will require lots of knowledge transfer and mentoring.
* The 'Silver Tsunami' in PH should be handled by hiring more potential engineers as soon as possible and  put them into different trainings in order to meet the percentage of workforce.

## Summary
1. As the 'Silver Tsunami' begins to make an impact on Pewlett Hackard workforce, PH needs to take quick action to recruit more employees. The retirment info csv results shows that there are 41380 employees retiring, resulting in lot of openings in PH. The recruitement process needs to be done and mentorship for new hires should start accordingly. The retirment info table was created with the following query.

![image](https://user-images.githubusercontent.com/108298416/184468401-4ef74ab7-abea-4763-a57a-6f832394f6d7.png)

2. The count of retiring employees is 41380 as per the retirement_info csv and the count of employees who have mentorship eligibility is 1549 as per the mentorship eligibility csv. With the rate of retiring employees being so high, Pewlett Hackard needs to incorporate more mentors in the concerned departments by accomodating senior current employees in the specific department,who are still not in the retirment list to mentor new hires along with the mentors from retiring list,for knowledege transfer and training. This analysis can be done by finding retiring employees count by department name, so that PH can allocate the required mentors from each department, depending on the needs. The following query will help find out the retiring employee count by department name.

![image](https://user-images.githubusercontent.com/108298416/184468788-fcb9fe07-64ba-47a3-9ffc-d2a553560c49.png)

 
