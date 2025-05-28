# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
~~~c
class Person:
    def __init__(self):
        self.name = ""
        self.age = 0

    def input_details(self):
        self.name = input("Enter name: ")
        self.age = int(input("Enter age: "))

    def display_details(self):
        print(f"Name: {self.name}")
        print(f"Age: {self.age}")
class Employee(Person):
    def __init__(self):
        super().__init__()
        self.employee_id = ""
        self.department = ""

    def input_details(self):
        super().input_details()
        self.employee_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")

    def display_details(self):
        super().display_details()
        print(f"Employee ID: {self.employee_id}")
        print(f"Department: {self.department}")
class Patient(Person):
    def __init__(self):
        super().__init__()
        self.patient_id = ""
        self.ailment = ""

    def input_details(self):
        super().input_details()
        self.patient_id = input("Enter patient ID: ")
        self.ailment = input("Enter ailment: ")

    def display_details(self):
        super().display_details()
        print(f"Patient ID: {self.patient_id}")
        print(f"Ailment: {self.ailment}")
print("\n--- Enter Employee Details ---")
emp = Employee()
emp.input_details()
print("\n--- Employee Information ---")
emp.display_details()
print("\n--- Enter Patient Details ---")
pat = Patient()
pat.input_details()
print("\n--- Patient Information ---")
pat.display_details()
~~~
## Sample Output
![Screenshot 2025-05-28 183821](https://github.com/user-attachments/assets/00117e3d-20f4-44a9-9ac0-7b0605fc5285)

##Result


Thus the program has been executed successfully

