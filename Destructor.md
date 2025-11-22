# Ex.No:5B Destructor
# AIM
To Add the destructor in the following python code to delete the instance of the class.

# ALGORITHM
Begin the program.
Define a class Student with:
An init() method that initializes name and age attributes.
A printDetail() method that prints the student's name and age.
A del() method that prints a message indicating the student object is deleted.
Create an object s1 of the Student class, passing "Vishvajit Rao" as the name and 22 as the age.
Call the printDetail() method on s1 to print the student's details.
Delete the s1 object using del s1, triggering the del() method.
Terminate the program.
# PROGRAM
```
#REGNO:- 212222060229
# Name:-sarvesan lathika
class Student:
	def __init__(self, name, age):
		self.name = name
		self.age = age

	def printDetail(self):
		print(f"My name is {self.name} and I am {self.age} years old.")

	def __del__(self):
	    print(f"{self.name} student is deleted.")


s1 = Student("Vishvajit Rao", 22)
s1.printDetail()
del s1
```
# OUTPUT
<img width="1151" height="244" alt="image" src="https://github.com/user-attachments/assets/a54ddb70-713a-4a67-a24c-6c1d45c999fb" />


# RESULT
Thus Add the destructor in the following python code to delete the instance of the class has been successfully implemented.
