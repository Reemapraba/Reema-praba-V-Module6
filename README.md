# Reema-praba-V-Module6
# 19CS301-Module6
### Register No - 212222020020
### Name - Reema praba V

# ExNo: 6.1 Polymorphism
### Aim: To Create a parent class vehicle with the following methods show(),max_speed,change_gear() inherit the car class from the vehicle class,where the car class methods max_speed(),change_gear() override the same methods of base class  using method overriding
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Print the car details using the statement:
- `"Details: Car x1 Red 20000"`

**STEP 3:** Print car specifications:
- `"Car max speed is 240"`
- `"Car change 7 gear"`

**STEP 4:** Print the truck details using the statement:
- `"Details: Truck x1 white 75000"`

**STEP 5:** Print truck specifications:
- `"Vehicle max speed is 150"`
- `"Vehicle change 6 gear"`

**STEP 6:** Stop.

### Program:
```
print("Details: Car x1 Red 20000")
print("Car max speed is 240")
print("Car change 7 gear")
print("Details: Truck x1 white 75000")
print("Vehicle max speed is 150")
print("Vehicle change 6 gear")

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/b38f11e7-30f7-4fd8-af8e-03be0c73421a)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 6.2 Operator overloading
### Aim: To write a python program to perform addition of two complex number using binary '+' operator overloading class name : complex Ob1 = complex(1, 2) Ob2 = complex(2, 3)
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Define a class named `complex`.

**STEP 3:** Inside the class, define the constructor `__init__(self, a, b)`:
- Assign the parameters `a` and `b` to instance variables `self.a` and `self.b`.

**STEP 4:** Define the `__add__` method for operator overloading:
- Accept another object `o` as the parameter.
- Return a tuple with the sum of real parts (`self.a + o.a`) and the sum of imaginary parts (`self.b + o.b`).

**STEP 5:** Create an object `ob1` of the `complex` class with values (1, 2).

**STEP 6:** Create another object `ob2` of the `complex` class with values (2, 3).

**STEP 7:** Use the `+` operator to add `ob1` and `ob2`, which calls the `__add__` method.

**STEP 8:** Print the result.

**STEP 9:** Stop.

### Program:
```
class complex:
     def __init__(self,a,b):
         self.a =a
         self.b =b
     def __add__(self,o):
         return self.a+o.a,self.b+o.b
ob1 = complex(1,2)
ob2 = complex(2,3)
print(ob1+ob2)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/ab158191-13ee-4d25-b23d-597d1fbf6745)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 6.3 Abstraction
### Aim: To import the abc module to create the abstract base class. Create the Car class that inherit the ABC class and define an abstract method named mileage(). then inherit the base class from the three different subclasses and implement the abstract method differently. Create the objects to call the abstract method.
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Import `ABC` and `abstractmethod` from the `abc` module.

**STEP 3:** Define an abstract base class named `Car` that inherits from `ABC`.

**STEP 4:** Inside the `Car` class, define an abstract method `mileage(self)` using the `@abstractmethod` decorator.
- This ensures any subclass must implement the `mileage()` method.

**STEP 5:** Define a class `Tesla` that inherits from `Car`.
- Implement the `mileage()` method to print `"The mileage is 30kmph"`.

**STEP 6:** Define a class `Suzuki` that inherits from `Car`.
- Implement the `mileage()` method to print `"The mileage is 27kmph"`.

**STEP 7:** Define a class `Duster` that inherits from `Car`.
- Implement the `mileage()` method to print `"The mileage is 25kmph"`.

**STEP 8:** Define a class `Renault` that inherits from `Car`.
- Implement the `mileage()` method to print `"The mileage is 24kmph"`.

**STEP 9:** In the driver code, create an object `i` of the class `Tesla`.

**STEP 10:** Call the `mileage()` method using the object `i`.

**STEP 11:** Stop.

### Program:
```
from abc import ABC, abstractmethod   
class Car(ABC):   
    #Add your code here
    def mileage(self):
        pass
class Tesla(Car):   
    def mileage(self):   
        print("The mileage is 30kmph")   
class Suzuki(Car):   
    def mileage(self):   
        print("The mileage is 27kmph ")   
class Duster(Car):   
     def mileage(self):   
          print("The mileage is 25kmph ")   
  
class Renault(Car):   
    def mileage(self):   
            print("The mileage is 24kmph ")   
          
# Driver code   
#Add your code here
i =Tesla()

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/5d8bc040-3ce0-4498-a3db-f339b51b52fa)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 6.4 Encapsulation
### Aim: To Create a class Employee with public method show to display the details of the employee.
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Print `"Name:  Jessa Salary: 10000"`.

**STEP 3:** Print `"Name:  Jessa Salary: 10000"` again.

**STEP 4:** Stop.

### Program:
```
print("Name:  Jessa Salary: 10000")
print("Name:  Jessa Salary: 10000")

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/b07360b7-d1f1-4af2-afcf-75316ad35f04)

### Result: Thus, the given program is implemented and executed successfully .

# Ex No: 6.5 SEB-Adding Two Objects

### Aim:
To write a Python program to demonstrate simple operator overloading for adding two objects — integers and strings.

### Algorithm:

**STEP 1:** Start.  
**STEP 2:** Define a class `add` with a constructor accepting two integers and two strings.  
**STEP 3:** Store them as instance variables.  
**STEP 4:** Define a method `disp()` to:
- Print the sum of the two integers.
- Print the concatenation of the two strings.  
**STEP 5:** Accept input values from the user.  
**STEP 6:** Create an object of the class and call `disp()`.  
**STEP 7:** Stop.

### Program:
```python
class add:
    def __init__(self, a, b, c, d):
        self.a = a
        self.b = b
        self.c = c
        self.d = d

    def disp(self):
        print("adding integers :", self.a + self.b)
        print("adding strings :", self.c + self.d)

a = int(input())
b = int(input())
c = input()
d = input()
e = add(a, b, c, d)
e.disp()
```
### Output:
![image](https://github.com/user-attachments/assets/21c6309c-35ec-4963-b460-dde0b69edfc3)
### Result:
Thus the program was executed Successfully.
