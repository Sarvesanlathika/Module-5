# Ex.No:5C Multi-level Inheritance
## AIM
To Write a Python program to Get the name, age and location of a person and display using Multilevel inheritance.

### ALGORITHM
1.Begin the program.

2.Define a class Parent with: An init() method to initialize name. A getName() method to return the name.

3.Define a class Child that inherits from Parent with: An init() method to initialize name and age (calling the parent's constructor for name). A getAge() method to return the age.

4.Define a class Grandchild that inherits from Child with: An init() method to initialize name, age, and location (calling the child's constructor for name and age).

5.A getLocation() method to return the location.

6.Take name, age, and location as input from the user.

7.Create an object gc of the Grandchild class with the given inputs.

8.Print the name, age, and location using getName(), getAge(), and getLocation() methods.
9.Terminate the program.
### PROGRAM
```
# REGNO:-212222060229
# Name:-sarvesan lathika
class Parent:
   def __init__(self,name):
     self.name = name
   def getName(self):
     return self.name
class Child(Parent):
   def __init__(self,name,age):
     Parent.__init__(self,name)
     self.age = age
   def getAge(self):
     return self.age
class Grandchild(Child):
   def __init__(self,name,age,location):
     Child.__init__(self,name,age)
     self.location=location
   def getLocation(self):
     return self.location
name=input()
age=int(input())
loc=input()
gc = Grandchild(name,age,loc)
print(gc.getName(), gc.getAge(), gc.getLocation())
```
# OUTPUT
<img width="1158" height="264" alt="image" src="https://github.com/user-attachments/assets/aaa707b0-73cf-497b-87a1-f6791d07d805" />


# RESULT
Thus a Python program to Get the name, age and location of a person and display using Multilevel inheritance has been implemented successfully.
