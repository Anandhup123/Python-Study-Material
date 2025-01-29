### **Conditional Control Statements in Python**
Conditional statements in Python allow the execution of different code blocks based on conditions.

---

## **1. if Statement**
Executes a block of code **if the condition is true**.

```python
age = 18

if age >= 18:
    print("You are eligible to vote.")
```

**Output:**
```
You are eligible to vote.
```

---

## **2. if-else Statement**
Executes one block **if the condition is true** and another block **if false**.

```python
age = 16

if age >= 18:
    print("You can vote.")
else:
    print("You are not eligible to vote.")
```

**Output:**
```
You are not eligible to vote.
```

---

## **3. if-elif-else Statement**
Used to check **multiple conditions**.

```python
marks = 85

if marks >= 90:
    print("Grade: A")
elif marks >= 75:
    print("Grade: B")
elif marks >= 50:
    print("Grade: C")
else:
    print("Grade: F")
```

**Output:**
```
Grade: B
```

---

## **4. Nested if Statement**
An `if` statement inside another `if`.

```python
num = 10

if num > 0:
    if num % 2 == 0:
        print("Positive even number.")
    else:
        print("Positive odd number.")
else:
    print("Negative number.")
```

**Output:**
```
Positive even number.
```

---

## **5. Short-hand if (Ternary Operator)**
Used for single-line conditions.

```python
age = 20
status = "Adult" if age >= 18 else "Minor"
print(status)
```

**Output:**
```
Adult
```

---

### **Example: Checking the Largest of Three Numbers**
```python
a, b, c = 10, 25, 15

if a > b and a > c:
    print("Largest:", a)
elif b > c:
    print("Largest:", b)
else:
    print("Largest:", c)
```

**Output:**
```
Largest: 25
```

