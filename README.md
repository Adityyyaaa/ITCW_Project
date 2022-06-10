# ITCW_Project - Academic Management System
## Problem Statement - 
Candidates get enrolled (registered) in Subjects. Upon registration they are 
assigned with instructors and also get their roll numbers. Achievement rewards 
students with 15 points. Punishment deducts 10 marks for students. If punished, 
the achievement grace marks are not added. Results are calculated on the basis 
of overall performance of the student during the entire course duration.

The diagram on how different classes is related to each other is as follows:
![image](https://user-images.githubusercontent.com/81140358/173026446-d76e7ffa-7f48-4c66-bc24-bd0705ffe94f.png)

## Description of the function that the classed perform:
### Abstract class Registration: 
Defines the attributes that are needed for a candidate to register also contains an abstract method which displays the information.
### Class Student: 
This class inherits the abstract class registration. Contains additional attributes such as Professor name and roll number. A method assignProf() assigns professor to the student on the basis of chosen subject. The displayStudent() method which displays the details of the student is defined here.
### Class ExamProfile: 
This class inherits Student class. Information is contained here if the student gets eligible for the grace marks, and also contains the test scores of the student. Also, the showScore() method displays the score that the student gets.
### Interface Achievement: 
Contains marks awarded as grace/penalty for the particular student during the entire course.
### Class Result: 
Inherits Examprofile class and implements Achievement. 
Constructor is put in place to initiate the class, method calculatedResult() which calculates the marks based on the conditions such as marks obtained and the grace marks. Also, method displayResult() displays the final result of the student.Upon the initiation of new object, the values of the attributes are assigned by the constructor, most of which are inherited from other classes. The method calculatedResult() uses control statements and calculates the resulting marks of the student based on the attributes. The method displayResult() uses inherited methods assignProf(), displayStudent(), showScore(), calculatedResult() to display the final result.

## Output:
![image](https://user-images.githubusercontent.com/81140358/173027993-3802fd25-dd44-42fe-852b-805a4484c4db.png)
