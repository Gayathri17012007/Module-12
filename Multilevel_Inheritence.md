# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
~~~c
class Person:
    def __init__(self):
        self.name = ""
        self.age = 0

    def get_personal_details(self):
        self.name = input("Enter name: ")
        self.age = int(input("Enter age: "))

    def display_personal_details(self):
        print(f"Name: {self.name}")
        print(f"Age: {self.age}")
class Resident(Person):
    def __init__(self):
        super().__init__()
        self.location = ""

    def get_location(self):
        self.location = input("Enter location: ")

    def display_location(self):
        print(f"Location: {self.location}")
class Citizen(Resident):
    def __init__(self):
        super().__init__()
~~~

## Sample Output

![Screenshot 2025-05-28 184248](https://github.com/user-attachments/assets/f401ac14-7294-47ea-b881-8672b554d5fd)

##Result

Thus the program has been executed successfully.
