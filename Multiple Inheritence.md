# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
~~~c
class Addition:
    def add(self, a, b):
        return a + b
class Subtraction:
    def subtract(self, a, b):
        return a - b
class Division:
    def divide(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Division by zero is not allowed"

class Calculator(Addition, Subtraction, Division):
    def __init__(self):
        pass

calc = Calculator()
a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

print(f"\nAddition of {a} and {b}: {calc.add(a, b)}")
print(f"Subtraction of {a} and {b}: {calc.subtract(a, b)}")
print(f"Division of {a} by {b}: {calc.divide(a, b)}")
~~~

## Output Example

![Screenshot 2025-05-28 184648](https://github.com/user-attachments/assets/e5e591e2-e379-4911-a600-eddf307b6b99)

##Result

Thus the program has been  executed successfully.
