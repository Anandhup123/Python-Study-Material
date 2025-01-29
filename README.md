### **🚀 Python Learning Roadmap (Step-by-Step) 🐍**  

This roadmap will guide you from **beginner to advanced level**, covering essential topics in a structured way. Follow each step, practice examples, and build small projects along the way. 💡  

---

## **📌 Phase 1: Python Basics (Week 1-2)**
**🔹 What to Learn:**  
✔ Python Installation & Setup (IDLE, VS Code, Jupyter Notebook)  
✔ Python Syntax & Indentation  
✔ Comments (`# Single-line`, `"""Multi-line"""`)  
✔ Variables & Constants  
✔ Data Types (`int`, `float`, `str`, `bool`, `list`, `tuple`, `dict`, `set`)  
✔ Type Casting (`str(5)`, `int("10")`, `float("3.14")`)  

**📌 Example:**
```python
name = "Alice"
age = 25
height = 5.6
is_student = True
print(f"{name} is {age} years old and {height} feet tall.")
```

✅ **Practice:**  
🔹 Convert `int` to `str`, `str` to `float`, etc.  
🔹 Write a program to swap two variables.  
🔹 Create a simple calculator.  

---

## **📌 Phase 2: Operators & Conditional Statements (Week 3)**
**🔹 What to Learn:**  
✔ Arithmetic Operators (`+`, `-`, `*`, `/`, `%`, `**`, `//`)  
✔ Comparison Operators (`==`, `!=`, `>`, `<`, `>=`, `<=`)  
✔ Logical Operators (`and`, `or`, `not`)  
✔ `if`, `if-else`, `elif`  
✔ `match` (Python 3.10+ alternative for `switch`)  

**📌 Example:**
```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

✅ **Practice:**  
🔹 Check if a number is even or odd.  
🔹 Find the largest number among three inputs.  
🔹 Implement a simple grade calculator.  

---

## **📌 Phase 3: Loops & Iteration (Week 4)**
**🔹 What to Learn:**  
✔ `for` loop  
✔ `while` loop  
✔ `break`, `continue`, `pass`  
✔ Nested loops  
✔ `else` with loops  

**📌 Example:**
```python
for i in range(1, 6):
    print(f"Square of {i} is {i**2}")
```

✅ **Practice:**  
🔹 Print numbers from 1 to 100 using a loop.  
🔹 Print the Fibonacci series up to `n` terms.  
🔹 Build a multiplication table generator.  

---

## **📌 Phase 4: Functions & Modular Programming (Week 5)**
**🔹 What to Learn:**  
✔ Defining and calling functions  
✔ Parameters and return values  
✔ Default & keyword arguments  
✔ `*args` and `**kwargs`  
✔ Lambda functions  

**📌 Example:**
```python
def greet(name="User"):
    return f"Hello, {name}!"

print(greet("Bob"))
```

✅ **Practice:**  
🔹 Create a function to calculate the area of a circle.  
🔹 Build a function to check if a number is prime.  
🔹 Write a function to reverse a string.  

---

## **📌 Phase 5: Data Structures (Week 6-7)**
**🔹 What to Learn:**  
✔ Lists (`append()`, `remove()`, `sort()`, `pop()`)  
✔ Tuples (Immutable lists)  
✔ Dictionaries (Key-value pairs, `get()`, `keys()`, `values()`)  
✔ Sets (Unique values, `union()`, `intersection()`)  
✔ List & Dictionary Comprehensions  

**📌 Example:**
```python
students = {"Alice": 85, "Bob": 92, "Charlie": 78}
for name, score in students.items():
    print(f"{name}: {score}")
```

✅ **Practice:**  
🔹 Create a contact book using a dictionary.  
🔹 Remove duplicates from a list using sets.  
🔹 Implement a student marks management system.  

---

## **📌 Phase 6: File Handling (Week 8)**
**🔹 What to Learn:**  
✔ Reading & writing text files (`open()`, `read()`, `write()`)  
✔ Using `with open()` for safe file handling  
✔ Handling CSV & JSON files (`csv` & `json` modules)  

**📌 Example:**
```python
with open("data.txt", "w") as file:
    file.write("Hello, world!")
```

✅ **Practice:**  
🔹 Read and write a list of names to a file.  
🔹 Convert a dictionary into a JSON file.  
🔹 Implement a basic log system.  

---

## **📌 Phase 7: Exception Handling (Week 9)**
**🔹 What to Learn:**  
✔ `try-except`  
✔ `finally`, `else`  
✔ Raising custom exceptions  

**📌 Example:**
```python
try:
    num = int(input("Enter a number: "))
    print(10 / num)
except ZeroDivisionError:
    print("Cannot divide by zero!")
```

✅ **Practice:**  
🔹 Handle invalid user input for a calculator.  
🔹 Write a program that catches multiple exceptions.  
🔹 Create a custom exception for invalid age input.  

---

## **📌 Phase 8: Object-Oriented Programming (Week 10-11)**
**🔹 What to Learn:**  
✔ Classes & Objects  
✔ `__init__` Constructor  
✔ Inheritance & Polymorphism  
✔ Encapsulation (`private` variables)  

**📌 Example:**
```python
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def details(self):
        return f"{self.brand} {self.model}"

car1 = Car("Tesla", "Model S")
print(car1.details())
```

✅ **Practice:**  
🔹 Create a class for a bank account with deposit & withdrawal methods.  
🔹 Implement an employee management system using classes.  
🔹 Build a simple student record system.  

---

## **📌 Phase 9: Modules & Libraries (Week 12)**
**🔹 What to Learn:**  
✔ Importing built-in modules (`math`, `random`, `datetime`)  
✔ Installing external libraries (`pip install numpy`)  
✔ Creating custom modules  

**📌 Example:**
```python
import random
print(random.randint(1, 10))
```

✅ **Practice:**  
🔹 Create a custom module for basic math operations.  
🔹 Use the `datetime` module to display the current time.  
🔹 Build a program that generates random passwords.  

---

## **📌 Phase 10: Algorithms & Problem Solving (Week 13+)**
**🔹 What to Learn:**  
✔ Sorting algorithms (Bubble, Selection, Merge)  
✔ Searching algorithms (Linear, Binary)  
✔ Recursion problems  

**📌 Example:**
```python
def factorial(n):
    return 1 if n == 0 else n * factorial(n-1)

print(factorial(5))  # Output: 120
```

✅ **Practice:**  
🔹 Solve at least 3 coding problems daily on **LeetCode** or **HackerRank**.  
🔹 Implement searching and sorting algorithms from scratch.  
🔹 Write a recursive function for the Fibonacci series.  

---

## **💡 What's Next?**
After mastering these, you can explore:  
🔹 **Web Development** (Django, Flask)  
🔹 **Data Science & Machine Learning** (NumPy, Pandas, Matplotlib)  
🔹 **Automation & Web Scraping** (Selenium, BeautifulSoup)  
🔹 **GUI Development** (Tkinter, PyQt)  

---

### **🔥 Final Advice:**  
✅ **Practice daily!**  
✅ **Work on projects!**  
✅ **Solve coding challenges!**  
🚀😊
