# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
~~~c
class Demo:
    def __init__(self):
        self.message = "Hello from the constructor!"
        print(self.message)

    def __del__(self):
        print("Destructor called. Cleaning up...")
obj = Demo()
del obj
~~~

## 🧪 Output

![Screenshot 2025-05-28 183302](https://github.com/user-attachments/assets/ea1b5e2d-1e12-4e8a-b9ff-6842c2b006b8)


## Result
Thus the program has been executed successfully.
