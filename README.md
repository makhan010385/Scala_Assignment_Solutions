# Scala Assignments
### [SCS2204_2020](https://ugvle.ucsc.cmb.ac.lk/course/view.php?id=278)


- **Assignment 1**

Write Scala functions to solve the following problems. 
1. The temperature is 35C; convert this temperature into Fahrenheit.
ºF =ºC * 1.8000 + 32.00
2. The volume of a sphere with radius r is 4/3 Pi r3. What is the volume of a sphere with radius 5?
3. Suppose the cover price of a book is Rs. 24.95, but bookstores get a 40% discount.Shipping costs Rs. 3 for the first 50 copy and 75 cents for each additional copy. 
What is the total wholesale cost for 60 copies?


- **Assignment 2**

Write Scala functions to solve the following problems. 
1. Company XYZ & Co. pays all its employees Rs.150 per normal working hour and Rs. 75 per OT hour. A typical employee works 40 (normal) and 20(OT) hours per week has to pay 10% tax. Develop a functional program that determines the take home salary of an employee from the number of working hours and OT hours given.
2.  Imagine the owner of a movie theater who has complete freedom in setting ticket prices. The more he charges, the fewer the people who can afford tickets. In a recent experiment the owner determined a precise relationship between the price of a ticket and average attendance.  At a price of Rs 15.00 per ticket, 120 people attend a performance. Decreasing the price by  5 Rupees increases attendance by 20 and increasing the price by  5 Rupees decreases attendance by 20. Unfortunately, the increased attendance also comes at an increased cost. Every performance costs the owner Rs.500. Each attendee costs another 3 Rupees. The owner would like to know the exact relationship between profit and ticket price so that he can determine the price at which he can make the highest profit. Implement a functional program to find out the best ticket price.


- **Assignment 3**

1. Can you write a recursive function prime(n) that returns true for a prime number and false for the other? 
For example prime(5) should return true and prime(8) should return false.
2. Can you write a recursive function primeSeq(n) that prints all 	prime number which less than n?
For example prime(10) should print 2,3,5, and 7 on the terminal.
3. Can you write a recursive function returns the addition of numbers from1 to n?
For example sum(5) should print 15
4. Can you write a recursive function to determine even and odd numbers? 
5. Can you write a recursive function to get the addition of all even numbers less than given n.
6. The Fibonacci Sequence is the series of numbers: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, . . . 
Each subsequent number is the sum of the previous two. 
Write a recursive function print fist n Fibonacci numbers for given n.


- **Assignment 4**

The Caesar cipher is one of the earliest known and simplest ciphers. It is a type of substitution cipher in which each letter in the plaintext is 'shifted' a certain number of places down the alphabet. For example, with a shift of 1, A would be replaced by B, B would become C, and so on. The method is named after Julius Caesar, who apparently used it to communicate with his generals.
1. Implement Encryption and Decryption functions of Caesar cipher.
2. Then implement a Cipher function which take Encryption and Decryption functions to process the data.


- **Assignment 5**

1. Implement a Data Structure for Rational Number and create a method neg to class Rational that is used like this: x.neg // evaluates to -x
2. Create a method sub to subtract two rational numbers and find an answer  x-y-z where x=3/4, y=5/8, z=2/7.
3. Implement a Data Structure for Account and create a method transfer which transfer the money from this account to a given account.
4.  A Bank defines as List of Accounts. So implement the following functions:
4.1 List of Accounts with negative balances
4.2 Calculate the sum of all account balances
4.3 Calculate the final balances of all accounts after apply the interest function as fallows: 
If balance is positive, deposit interest is .05  and if balance is negative, overdraft interest is .1




- **Assignment 6**

Implement a case class Point(x,y) and create following methods:
1. add(+) should add two given points
2. move should move a point by a given distance dx and dy
3. distance should return the distance between two given points
4. invert should switch the x and y coordinates.


-----------------------------------------------------------------------------------------------------------------

--------------
List based assignment  :-
________________________________________________________________________________________________________
Assignemnt 1)
________________________________________________________________________________________________________


Every Student has some marks associated with it. Student details contains its id and name.
And for Marks, there are subjectId, studentId and number of marks a student scored.


Following are the requirements which is required to gain from above scenario (i.e. Student and marks)


1)
Input:- (subjectId, percentage, pass/fail)
Output:- for input pass, evaluate that how much students(id, name) are passed in the inputted subjectId
	for input fail, evaluate that how much students(id, name) are failed in the inputted subjectId
Note:- percentage is the input which defines the minimum passing criteria
e.g. 
Pass count: 15
Fail count: 10


2)
Input:- (subjectId, count, top/bottom)
Output:- based on the last input(top/bottom), output the students details who have scored max/min in that subjectId
e.g. 
input: 1 5 top
output: 
Kunal 85
Himanshu 84
Geetika 83
Anmol 82
Mahesh 81


3)
Input:-
(top/bottom, count)
OutPut:-
Overall top/least scorer based on all the subjects score, fetch students name
count- input defines that how much students name are to be printed on console
e.g.
input: top 2


output:
Himanshu 75%
Geetika 74%




4)
Input:-
(percentage, good_scholarship, normal_or_no_scholarship)
Output:- two groups of students with the amount of scholarship
e.g.
input: 85% 2000 500
output: 
Kunal 2000
Himanshu 500
Geetika 2000
Mahesh 500


5)
Input:-
(pass/fail, percentage)
count and print the number of students and all names who are passed/fail,
Pass or fail would be decided by percentage input field.
e.g.
input: fail 30
output: 
Kunal 28%
Himanshu 29%


6) Find the student(s) who have scored 95% or above and print its details.
input: 95%
output:
Kunal 95%
Himanshu 96%
Geetika 97%


7) For every student, find its marks in detail (just like detailed Report card of a student.)
Note:- must use groupBy method of List
input: reportcard
output:
Kunal 75 70 80 75 75%
Himanshu 74 70 81 75 75%
Geetika 70 70 85 75 75%




Developer Notes:


There would be two case classes
1) Student(id: Long, name: String)
2) Marks(subjectId: Int,studentId: Long, marksObtained: float)


In order to fill data in those case classes, either take inputs from a file, or take static inputs. But there must be atleast 5 subjects, and atleast 10 students.
e.g. List(Student(1, "Kunal"), Student(2, "Himanshu"), Student(3, "Geetika") ....)
List(Marks(1, 1, 95), Marks(2, 1, 75), ...)
So basically here Kunal has marks 95 and 75 for the paper 1 and 2 respectively.


______________________________________________________________________________________________________
Assignemnt 2)
______________________________________________________________________________________________________
- Find the last element of list with its index value(dont use inbuilt methods to extract last element directly)
- print the table of each element in the List
- aggregate the contents of two lists of same size into a single list
	List(1,2) and List("a", "b") results List(List(1, "a"), List(2, "b"))
- find sum and multiplication of the list (dont use inbuilt methods)
- apply quicksort and mergesort on the Lists
- implement Stack and Queue using Lists.









