# Ex.No:5A Constructors - Parameterized Constructor
# AIM
To Write a python program using class to perform addition of three numbers using default constructor.Assume the three numbers are num1=1000 num2=2000 num3=3000

# ALGORITHM
Begin the program.
Define a class add with an init method to initialize the variables num1, num2, and num3 with values 1000, 2000, and 3000 respectively.
Define a method dis() inside the class that: Calculates the sum of num1, num2, and num3, and assigns it to self.num.
Prints the value of self.num.
Create an object obj of the class add.
Call the dis() method on the obj object to display the sum.
Terminate the program.
# PROGRAM
```
# REGNO:-212222060229
# Name:-sarvesan lathika
class add:
    def __init__(self):
        self.num1=1000
        self.num2=2000
        self.num3=3000
    def dis(self):
        self.num=self.num1+self.num2+self.num3
        print(self.num)
obj=add()
obj.dis()
```

# OUTPUT
<img width="1138" height="207" alt="image" src="https://github.com/user-attachments/assets/3cfbaea3-f0cd-4fe9-bedf-82dc5641cf0f" />


# RESULT
Thus a python program using class to perform addition of three numbers using default constructor has been successfully implemented.
