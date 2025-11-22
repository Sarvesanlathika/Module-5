# Exp.No:24
Multi-level Inheritance
# AIM
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

# ALGORITHM
Define the Person class:

1.Inside the Person class, define the __init__ method (constructor) with two parameters: name and age.
Inside the __init__ method, assign the name to self.name and age to self.age.
Define the PersonDetails class that inherits from the Person class:

2.Inside the PersonDetails class, define the __init__ method (constructor) with three parameters: name, age, and person_id.
Inside the __init__ method, call the __init__ method of the Person class using super() to initialize name and age.
Assign person_id to self.person_id.
Define the DisplayDetails class that inherits from the PersonDetails class:

3.Inside the DisplayDetails class, define the __init__ method (constructor) with three parameters: name, age, and person_id.
Inside the __init__ method, call the __init__ method of the PersonDetails class using super() to initialize name, age, and person_id.
Inside the DisplayDetails class, define the show_details method:

4.Inside the show_details method, return a formatted string with self.name, self.age, and self.person_id.
Prompt the user to enter name (string), age (integer), and person_id (integer).

Create an instance person of the DisplayDetails class, passing name, age, and person_id to the constructor.

Call the show_details method on the person object and print the result.

Terminate the program.

# PROGRAM
```
# Reg.No-212222060229
# Name-sarvesan lathika
class Parent:
    def __init__(self, name):
        self.name = name

    def getName(self):
        return self.name

class Child(Parent):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

    def getAge(self):
        return self.age

class Grandchild(Child):
    def __init__(self, name, age, id):
        super().__init__(name, age)
        self.id = id

    def getid(self):
        return self.id

# Input from user
name = input()
age = int(input())
id = int(input())

# Object creation and method calls
gc = Grandchild(name, age, id)
print(gc.getName(), gc.getAge(), gc.getid())
```

# OUTPUT
<img width="434" height="133" alt="image" src="https://github.com/user-attachments/assets/3cb36329-aabb-4893-a2cd-e7696a5c5de4" />


# RESULT
Thus the program to get the name, age, and ID of a person and display them using multilevel inheritance has been implemented and executed successfully.
