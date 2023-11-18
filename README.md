# legalnamechanges
Find duplicates in databases to merge or investigate


##Simple code snippet to edit to work with your database
##Reduce duplicates in database to speed up transctional or lookup speed
##Used with existing code will help find employees using same SSN for further investigation
##I had my name legall changed, but my personality, ethics and morality character didn't change for the worse


SELECT First_Name, Last_Name, Address, City, State, Phone_Number
##Change names to fit columns in your database to assist with planning further research
FROM Employees
##Change name of table to fit your data
GROUP BY Employee_SSN
HAVING COUNT (Employee_SSN) > 1
