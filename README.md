# legalnamechanges
Find duplicates in databases to merge or investigate


##Simple code snippet to edit to work with your database
##Reduce duplicates in database to speed up transctional or lookup speed
##Used with existing SQL will help find employees using same SSN for further investigation
##I had my name legally changed, but my SSN, personality, ethics and morality character didn't change (for the worse, just better)
##Note: Someone named Donnajay is competing for my identity, as programmer, technology manager and WGU graduate, but isn't suthentic
##Reducing identity fraud in your database and community can be very good thing
##Popular or wealthy people aren't neceessary using true identity

SELECT First_Name, Last_Name, Address, City, State, Phone_Number
##Change names to fit columns in your database to assist with planning further research
FROM Employees
##Change name of table to fit your data
GROUP BY Employee_SSN
HAVING COUNT (Employee_SSN) > 1
