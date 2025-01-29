In Python, there are several **types of functions** based on how they are defined, called, and used. Here’s a breakdown:

---

### **1. Built-in Functions**
These are functions that are pre-defined in Python, meaning they are available for use without having to define them. Some examples include `print()`, `len()`, `max()`, `sum()`, `abs()`, etc.

#### Example:
```python
print(len([1, 2, 3]))  # Output: 3
print(max([1, 2, 3]))  # Output: 3
```

---

### **2. User-Defined Functions**
These are functions created by the programmer to perform specific tasks. You define them using the `def` keyword.

#### Syntax:
```python
def function_name(parameters):
    # function body
    return result
```

#### Example:
```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Anandhu"))  # Output: Hello, Anandhu!
```

---

### **3. Recursive Functions**
A recursive function is one that calls itself to solve a smaller instance of the same problem. Recursion continues until a base condition is met.

#### Example:
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

---

### **4. Lambda Functions**
Lambda functions (also known as anonymous functions) are small, one-line functions defined using the `lambda` keyword. They are typically used for short, throwaway functions.

#### Syntax:
```python
lambda arguments: expression
```

#### Example:
```python
multiply = lambda x, y: x * y
print(multiply(2, 3))  # Output: 6
```

---

### **5. Higher-Order Functions**
These are functions that either take one or more functions as arguments, or return a function as a result. Examples of higher-order functions include `map()`, `filter()`, and `reduce()`.

#### Example (Using `map()`):
```python
numbers = [1, 2, 3, 4]
squared = list(map(lambda x: x**2, numbers))
print(squared)  # Output: [1, 4, 9, 16]
```

---

### **6. Functions with Default Arguments**
You can define default values for function parameters. If the caller does not provide a value for that parameter, the default value is used.

#### Example:
```python
def greet(name, message="Hello"):
    return f"{message}, {name}!"

print(greet("Anandhu"))  # Output: Hello, Anandhu!
print(greet("Anandhu", "Good morning"))  # Output: Good morning, Anandhu!
```

---

### **7. Functions with Variable-Length Arguments**
Python allows you to define functions that accept a variable number of arguments. You can use `*args` (for non-keyword arguments) and `**kwargs` (for keyword arguments).

- `*args`: Used to pass a variable number of positional arguments.
- `**kwargs`: Used to pass a variable number of keyword arguments.

#### Example (`*args`):
```python
def add(*args):
    return sum(args)

print(add(1, 2, 3, 4))  # Output: 10
```

#### Example (`**kwargs`):
```python
def greet(**kwargs):
    return f"Hello, {kwargs.get('name', 'Guest')}!"

print(greet(name="Anandhu"))  # Output: Hello, Anandhu!
```

---

### **8. Anonymous Functions (Using `lambda`)**
These functions are called "anonymous" because they are not bound to a name. They are useful for short-term use where defining a full function is unnecessary.

#### Example:
```python
add = lambda a, b: a + b
print(add(3, 4))  # Output: 7
```

---

### **9. Function with Keyword Arguments**
In Python, functions can be called using keyword arguments. You pass values to specific parameters by explicitly naming the parameter.

#### Example:
```python
def greet(name, age):
    return f"Hello {name}, you are {age} years old."

print(greet(name="Anandhu", age=25))  # Output: Hello Anandhu, you are 25 years old.
```

---

### **10. Method Functions**
Methods are functions that are associated with an object. They are typically used with object-oriented programming (OOP) concepts, where methods belong to a class and operate on instances of that class.

#### Example:
```python
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        return f"Hello, {self.name}"

person = Person("Anandhu")
print(person.greet())  # Output: Hello, Anandhu
```

---

### **Summary of Function Types**:

| **Function Type**                  | **Description**                                                | **Example**                                                   |
|------------------------------------|----------------------------------------------------------------|---------------------------------------------------------------|
| **Built-in Functions**             | Functions that are pre-defined in Python                      | `print()`, `len()`, `max()`                                   |
| **User-Defined Functions**         | Functions defined by the user using `def`                     | `def greet(name):`                                            |
| **Recursive Functions**            | Functions that call themselves                               | `def factorial(n):`                                           |
| **Lambda Functions**               | Small, one-line anonymous functions                            | `multiply = lambda x, y: x * y`                               |
| **Higher-Order Functions**         | Functions that take other functions as arguments or return them| `map()`, `filter()`, `reduce()`                               |
| **Functions with Default Arguments**| Functions with default parameter values                       | `def greet(name, message="Hello"):`                           |
| **Functions with Variable-Length Arguments**| Functions that accept variable number of arguments       | `def add(*args):` or `def greet(**kwargs):`                   |
| **Method Functions**               | Functions associated with objects in a class                  | `def greet(self):` inside a class                              |
