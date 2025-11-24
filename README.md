# Exp.No:21 Constructors - Parameterized Constructor
# AIM
To write a Python code to create a class for a person with a parameterized constructor, which will take the name and userid of the person as parameters and print the userid of the person.

# ALGORITHM
Begin the program. Define a person class. The person class should have a parameterized init method that accepts two parameters: name and userid. Inside the init method, assign the name to self.name and the userid to self.userid. Print the self.userid. Prompt the user to enter their name (string) and userid. Create an instance s1 of the person class by passing the entered name and userid to the constructor. Terminate the program.

# PROGRAM
~~~
Reg-212222060229 Name-sarvesan lathika
class person:
def init(self,a,b):
self.a=a
self.b=b
def show(self):
print(self.b)
a=str(input())
b=str(input())
x=person(a,b)
x.show()
~~~
# OUTPUT
<img width="1091" height="285" alt="image" src="https://github.com/user-attachments/assets/e89092bc-1140-4045-916b-d8441ba74cf0" />

# RESULT 
Thus the python program was initiated and executed successfully.

# Exp.No:22 Destructor
# AIM
To create a Python class Student with a destructor.

# ALGORITHM
Begin the program. Define the student class. Inside the student class, define the init method (constructor) and the del method (destructor). Create an object s2 of the student class. When the object s2 is created, the init method is called, and its print statements are executed. Use the del statement to delete the object s2. This triggers the del method (destructor), and the respective print statements are executed. Terminate the program.

# PROGRAM
~~~
Reg-212222060229 Name-sarvesan lathika

class Awesome:
def greetings(self):
print("My name is Vishvajit Rao and I am 22 years old.")
def del(self):
print("Vishvajit Rao student is deleted.")
obj = Awesome()
obj.greetings()
~~~
# OUTPUT
<img width="1333" height="244" alt="image" src="https://github.com/user-attachments/assets/7a6e8546-ce70-477f-8ba4-eaacb932593d" />

# RESULT
Thus the python program was initialised and executed successfully.

# Exp.No:25 Multi-level Inheritance
# AIM
To write a Python program that collects a person's name, age, and salary, and displays them using multilevel inheritance in object-oriented programming.

# ALGORITHM
Start the program. Define class a (base class): In the constructor init(), get input for: x → Name (string) a → Age (integer) b → Salary (integer) Define class b inheriting from a: Define dis1() to return name. Define class c inheriting from a: Define dis2() to return age. Define class d inheriting from a: Define dis3() to return salary. Define class e inheriting from b, c, and d: Use pass since it inherits everything needed. Create an object y of class e. Print the outputs from dis1(), dis2(), and dis3(). End the program.

# PROGRAM
~~~
Reg-212222060229 Name-sarvesan lathika

class a:
def init(self):
self.x=input()
self.a=int(input())
self.b=int(input())
class b(a):
def dis1(self):
return self.x
class c(a):
def dis2(self):
return self.a
class d(a):
def dis3(self):
return self.b
class e(b,c,d):
pass
y=e()
print(y.dis1() ,y.dis2() ,y.dis3())
~~~
# OUTPUT
<img width="947" height="292" alt="image" src="https://github.com/user-attachments/assets/5895015b-3b43-4b4d-be6d-d3c4113ee76c" />

# RESULT 
Thus the python program was initiated and implemented successfully.

# Exp.No:23 Multiple Inheritance
# AIM
To write a Python program using multiple inheritance to get a student’s name, attendance, and ID (grade), and determine if the student is eligible for placement based on their grade.

# ALGORITHM
Start the program. Define class A: In the constructor init(), accept input for: n: Student's name a: Student's attendance i: Student's ID (grade) Define class B inheriting from A: Define disp1() to print the name and attendance. Define class C inheriting from A: Define disp2() to check if grade (i) is greater than 90: If yes, print “Eligible for Placement”. Else, print “Not Eligible for Placement”. Define class D that inherits from both B and C (multiple inheritance). Create an object o of class D. Call disp1() to display name and attendance. Call disp2() to check placement eligibility. End the program.

# PROGRAM
~~~
class student: def init(self,name,id,attendance): self.name=name self.id=id self.attendance=attendance def view(self): print(self.name) print(self.id) name=input() id=int(input()) attendance=int(input()) obj=student(name,id,attendance) obj.view () if attendance>=75: print("Eligible for Exam") else: print("Not Eligible for Exam")
~~~

# OUTPUT
<img width="1177" height="343" alt="image" src="https://github.com/user-attachments/assets/ad950f0a-6e12-4a54-8f5f-effae540e397" />

# RESULT
Thus the python program was initiated and executed successfully.

# Exp.No:25 Hierarchical Inheritance
# AIM
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named Details and two child (derived) classes named Employee and Doctor.

# ALGORITHM
Begin the program. Create a class Details with an init method to initialize three attributes: id, name, and gender. Define a method display_details() to print the values of id, name, and gender. Create a class Employee that inherits from the Details class. Add two additional attributes: company and department. Override the display_details() method to print the employee-specific attributes (company and department) along with the inherited details. Create a class Doctor that also inherits from the Details class. Add two additional attributes: hospital and department. Override the display_details() method to print the doctor-specific attributes (hospital and department) along with the inherited details. Accept input for employee and doctor details. Create objects of Employee and Doctor using the input. Call the display_details() method for both objects to print the details. Terminate the program.

# PROGRAM
~~~
# hierarchical inheritance

class Details:
    def __init__(self):
        self.__id="<No Id>"
        self.__name="<No Name>"
        self.__gender="<No Gender>"
    def setData(self,id,name,gender):
        self.__id=id
        self.__name=name
        self.__gender=gender
    def showData(self):
        print("Id: ",self.__id)
        print("Name: ", self.__name)
        print("Gender: ", self.__gender)

class Employee(Details): #Inheritance
    def __init__(self):
        self.__company="<No Company>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,comp,dept):
        self.setData(id,name,gender)
        self.__company=comp
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__company)
        print("Department: ", self.__dept)

class Patient(Details): #Inheritance
    def __init__(self):
        self.__hospital="<No Hospital>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,hos,dept):
        self.setData(id,name,gender)
        self.__hospital=hos
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__hospital)
        print("Department: ", self.__dept)

id=int(input())
name=input()
gender=input()
comp=input()
dept=input()
id1=int(input())
nam=input()
gen=input()
hosp=input()
dep=input()

print("Doctor Object")
e=Employee()
e.setEmployee(id,name,gender,comp,dept)
e.showEmployee()
print("\nPatient Object")
d = Patient()
d.setEmployee(id1, nam, gen, hosp, dep)
d.showEmployee()
~~~
# OUTPUT
<img width="1183" height="465" alt="image" src="https://github.com/user-attachments/assets/f0e12ffa-e023-4ac4-bb90-3f11ea7b5d94" />

# RESULT 
Thus the program to get the employee and doctor details and display them using hierarchical inheritance has been implemented and executed successfully.
