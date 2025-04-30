# 19CS301-Module-6

## EX: 6.1 POLYMORPHISM

### AIM: To create two classes Cat and Dog with functions mood() and sound() which are same for both the classes yet they produce distinct outputs. iterate over the objects of the two classes “Cat” and “Dog” without worrying about the class types


### ALGORITHM:

1.Define class Cat with methods mood() and sound().

2.Define class Dog with the same methods mood() and sound().

3.Create instances: hello_kitty (Cat), hello_puppy (Dog).

4.Iterate over both objects in a loop.

5.Call mood() and sound() on each object.

### PROGRAM:
```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Cat:
    def mood(self): 
       print("Grumpy") 
    def sound(self): 
       print("Meow") 
 
class Dog:
    def mood(self): 
       print("Happy") 
    def sound(self): 
       print("Woof") 
 
hello_kitty = Cat()
hello_puppy = Dog()
 
for pet in (hello_kitty, hello_puppy):
    pet.mood()
    pet.sound()

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/da6eb678-9891-4de6-85f1-d488671c17c3)

### RESULT: 
Thus, the program has been successfully executed.

## EXP.No: 6.b OPERATOR OVERLOADING

### AIM: Write a Python program for simply using the overloading operator for adding two objects.

### ALGORITHM:

1.Define a class Example with an __init__() method to store a value.

2.Overload the + operator using __add__() method to return the sum or concatenation.

3.Create two objects e1, e2 with integer values and print the result of e1 + e2.

4.Create two objects e3, e4 with string values and print the result of e3 + e4.

### PROGRAM:
```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Example:
    def __init__(self,x):
        self.x=x
    def __add__(self,other):
        return self.x+other.x

e1=Example(int(input()))
e2=Example(int(input()))
print("adding integers :",e1+e2)
e3=Example(input())
e4=Example(input())
print("adding strings :",e3+e4)
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/d70fe639-9248-415b-892e-cbd1c5fe48b7)

### RESULT:
Thus, the program has been successfully executed.

## EX: 6.3 ABSTRACT CLASS METHOD

### AIM: To create an abstract class Animal with an abstract mathod move which can be implemented by the subclasses of the animal class.

### ALGORITHM:

1.Import ABC and abstractmethod from the abc module.

2.Define an abstract class Animal with an abstract method move().

3.Create subclasses Human, Snake, Dog, and Lion that each implement the move() method differently.

4.Instantiate each subclass and call the move() method to demonstrate polymorphic behavior.


### PROGRAM:
```
# Reg.No-212223020018
# Name-Mohamed Jafin S
# Python program showing
# abstract base class work

from abc import ABC, abstractmethod
class Animal(ABC):

	def move(self):
		pass

class Human(Animal):

	def move(self):
		print("I can walk and run")

class Snake(Animal):

	def move(self):
		print("I can crawl")

class Dog(Animal):

	def move(self):
		print("I can bark")

class Lion(Animal):

	def move(self):
		print("I can roar")
		
# Driver code
R = Human()
R.move()

K = Snake()
K.move()

R = Dog()
R.move()

K = Lion()
K.move()
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/01953a13-f86d-4d90-a24c-d3c4cb0c08f5)

### RESULT:
Thus, the program has been successfully executed.

## EXP.No: 6.4     ENCAPSULATION

### AIM: Create a class Car with the private variables max_speed,name change the value of a private variable, Use a setter method  setMaxSpeed(). create an object of the class to invoke the methods

### ALGORITHM:

1.Define a class Car with two private variables __maxspeed and __name.

2.Initialize these variables in the __init__() method.

3.Create a method drive() to print the current max speed.

4.Define a setter method setMaxSpeed(speed) to modify __maxspeed.

5.Create an object redcar of class Car.

6.Call drive() to show the initial speed.

7.Use setMaxSpeed() to change the max speed.

8.Call drive() again to display the updated speed.

### PROGRAM:
```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Car:

    __maxspeed = 0
    __name = ""
    
    def __init__(self):
        self.__maxspeed = 200
        self.__name = "Supercar"
    
    def drive(self):
        print('driving. maxspeed ' + str(self.__maxspeed))

    def setMaxSpeed(self,speed):
        self.__maxspeed = speed

redcar = Car()
redcar.drive()
redcar.setMaxSpeed(320)
redcar.drive()
```
### OUTPUT:
 ![image](https://github.com/user-attachments/assets/2dc1ee8a-4d5e-439b-9884-482348dc8c80)

### RESULT:
Thus, the program has been successfully executed

## EXP.No: 6.5  SEB

### AIM:  To write a Python program for simply using the overloading operator for adding two objects.

### ALGORITHM:

1.Define a class example with an __init__() method to assign a value to self.x.

2.Overload the + operator using the __add__() method to return self.x + u.x.

3.Create two objects object_1, object_2 with integer inputs and print their sum.

4.Create two objects object_3, object_4 with string inputs and print their concatenation.

### PROGRAM:
```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class example:
    def __init__(self,x):
        self.x=x
    def __add__(self,u):
        return self.x+u.x
object_1=example(int(input()))
object_2=example(int(input()))
print(": ",object_1+object_2)
object_3=example(str(input()))
object_4=example(str(input()))
print(": ",object_3+object_4)

```
### OUTPUT:
 ![image](https://github.com/user-attachments/assets/e1e917c2-df12-48e3-ad0f-524dc29835bd)

### RESULT:
Thus, the program has been successfully executed
