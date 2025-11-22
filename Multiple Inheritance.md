# Exp.No:23
Multiple Inheritance
# AIM
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

# ALGORITHM
1.Define the Student class.

2.Inside the Student class, define the __init__ method (constructor). The __init__ method accepts two parameters: name and student_id.
   Inside the __init__ method: Assign the value of name to self.name and student_id to self.student_id.
   
3.Define the get_student_info method inside the Student class

4.This method should return a string formatted with self.name and self.student_id.

5.Define the Attendance class, which inherits from the Student class.

6.Inside the Attendance class, define the __init__ method (constructor).

7.The __init__ method accepts three parameters: name, student_id, and attendance.

8.Inside the __init__ method: Call the parent class constructor super().__init__(name, student_id) to initialize name and student_id. Assign the value of attendance to self.attendance.

9.Define the check_eligibility method inside the Attendance class:

10.Terminate the program.
# PROGRAM
```
# Reg.No-212222060229
# Name-sarvesan lathika
class Demo:
    def __init__(self):
        self.status = "Alive"
    
    def __del__(self):
        print('The object no longer exists')

obj = Demo()
print(obj.status)
```
# OUTPUT
<img width="443" height="118" alt="image" src="https://github.com/user-attachments/assets/730ca834-1fcf-4b70-9d99-7760c7464cef" />


# RESULT
Thus the program that demonstrates the use of a destructor method (del) in a class to indicate when an object is destroyed has been implemented and executed successfully.
