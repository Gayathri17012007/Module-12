# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
~~~c
class Student:
    def __init__(self, name="Student"):
        self.name = name
    def welcome_message(self):
        print(f"Welcome to the course, {self.name}!")
student_name = input("Enter the student's name: ")
student = Student(student_name)
student.welcome_message()
~~~

## Output

![Screenshot 2025-05-28 182927](https://github.com/user-attachments/assets/b580b116-9dd3-4c4d-8603-9a7ec31d8d25)

## Result
Thus the program has been executed successfully.
