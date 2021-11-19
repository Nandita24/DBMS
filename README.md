                                         PART A 
                                         
1. Consider the following schema for a Library Database: 
  BOOK(Book_id, Title, Publisher_Name, Pub_Year) 
  BOOK_AUTHORS(Book_id, Author_Name) 
  PUBLISHER(Name, Address, Phone) 
  BOOK_COPIES(Book_id, Programme_id, No-of_Copies) 
  BOOK_LENDING(Book_id, Programme_id, Card_No, Date_Out, Due_Date) 
  LIBRARY_PROGRAMME(Programme_id, Programme_Name, Address) 
  
   Write SQL queries to 
   
(i). Retrieve details of all books in the library – id, title, name of publisher, authors, 
   number of copies in each Programme, etc.
   
(ii). Get the particulars of borrowers who have borrowed more than 3 books, but 
   from Jan 2017 to Jun 2017. 
   
(iii). Delete a book in BOOK table. Update the contents of other tables to reflect this 
   data manipulation operation. 
   
(iv). Partition the BOOK table based on year of publication. Demonstrate its working 
   with a simple query. 
   
(v). Create a view of all books and its number of copies that are currently available 
   in the Library.
   
2. Consider the following schema for Order Database: 
  SALESMAN(Salesman_id, Name, City, Commission) 
  CUSTOMER(Customer_id, Cust_Name, City, Grade, Salesman_id) 
  ORDERS(Ord_No, Purchase_Amt, Ord_Date, Customer_id, Salesman_id)
  
  Write SQL queries to 
  
(i). Count the customers with grades above Bangalore’s average. 

(ii). Find the name and numbers of all salesman who had more than one customer. 

(iii). List all the salesman and indicate those who have and don’t have customers in 
   their cities (Use UNION operation.) 
   
(iv). Create a view that finds the salesman who has the customer with the highest order 
   of a day. 
   
(v). Demonstrate the DELETE operation by removing salesman with id 1000. All 
   his orders must also be deleted. 
   
3. Consider the schema for Movie Database: 
  ACTOR(Act_id, Act_Name, Act_Gender) 
  DIRECTOR(Dir_id, Dir_Name, Dir_Phone) 
  MOVIES(Mov_id, Mov_Title, Mov_Year, Mov_Lang, Dir_id) 
  MOVIE_CAST(Act_id, Mov_id, Role) 
  RATING(Mov_id, Rev_Stars) 
  
  Write SQL queries to 
  
(i). List the titles of all movies directed by ‘Hitchcock’. 

(ii). Find the movie names where one or more actors acted in two or more movies.

(iii). List all actors who acted in a movie before 2000 and also in a movie after 2015 
   (use JOIN operation).
   
(iv). Find the title of movies and number of stars for each movie that has at least one 
     rating and find the highest number of stars that movie received. Sort the result by 
      movie title. 

(v). Update rating of all movies directed by ‘Steven Spielberg’ to 5. 

4. Consider the schema for College Database: 
  STUDENT(USN, SName, Address, Phone, Gender) 
  SEMSEC(SSID, Sem, Sec) 
  CLASS(USN, SSID) 
  COURSE(Subcode, Title, Sem, Credits) 
  IAMARKS(USN, Subcode, SSID, Test1, Test2, Test3, FinalIA) 
  
 Write SQL queries to 
 
(i). List all the student details studying in fourth semester ‘C’ section. 

(ii). Compute the total number of male and female students in each semester and in each section.
   
(iii). Create a view of Test1 marks of student USN ‘1BI15CS101’ in all Courses. 

(iv). Calculate the FinalIA (average of best two test marks) and update the 
   corresponding table for all students. 
   
(v). Categorize students based on the following criterion: 
     If FinalIA = 17 to 20 then CAT = ‘Outstanding’ 
     If FinalIA = 12 to 16 then CAT = ‘Average’ 
     If FinalIA< 12 then CAT = ‘Weak’ 
     Give these details only for 8th semester A, B, and C section students. 
  
  
5. Consider the schema for Company Database: 
  EMPLOYEE(SSN, Name, Address, Sex, Salary, SuperSSN, DNo) 
  DEPARTMENT(DNo, DName, MgrSSN, MgrStartDate) 
  DLOCATION(DNo,DLoc) 
  PROJECT(PNo, PName, PLocation, DNo) 
  WORKS_ON(SSN, PNo, Hours) 
  
  Write SQL queries to 
  
(i). Make a list of all project numbers for projects that involve an employee whose 
   last name is ‘Scott’, either as a worker or as a manager of the department that 
   controls the project. 
   
(ii). Show the resulting salaries if every employee working on the ‘IoT’ project is 
      given a 10 percent raise. 
   
(iii). Find the sum of the salaries of all employees of the ‘Accounts’ department, as 
       well as the maximum salary, the minimum salary, and the average salary in this 
       department 
   
(iv). Retrieve the name of each employee who works on all the projects controlledby 
      department number 5 (use NOT EXISTS operator). 
   
(v). For each department that has more than five employees, retrieve the department 
     number and the number of its employees who are making more than Rs. 
     6,00,000.
