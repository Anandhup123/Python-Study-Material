## **Loops in Python**
Loops are used to execute a block of code multiple times. Python has two main types of loops:

1. **`for` loop** – Used for iterating over a sequence (e.g., list, tuple, string, range).
2. **`while` loop** – Runs as long as a condition is `True`.

---

## **1. for Loop**
The `for` loop iterates over sequences such as lists, tuples, dictionaries, strings, or `range()`.

### **Example 1: Looping through a list**
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
**Output:**
```
apple
banana
cherry
```

### **Example 2: Using `range()`**
```python
for i in range(5):  # Loops from 0 to 4
    print(i)
```
**Output:**
```
0
1
2
3
4
```

### **Example 3: Using `range(start, stop, step)`**
```python
for i in range(1, 10, 2):  # Loops from 1 to 9, step 2
    print(i)
```
**Output:**
```
1
3
5
7
9
```

---

## **2. while Loop**
A `while` loop continues execution **as long as the condition is `True`**.

### **Example 1: Basic while loop**
```python
count = 0
while count < 5:
    print(count)
    count += 1
```
**Output:**
```
0
1
2
3
4
```

---

## **3. Loop Control Statements**
### **a) break Statement**
Exits the loop immediately.

```python
for i in range(5):
    if i == 3:
        break  # Stops the loop when i is 3
    print(i)
```
**Output:**
```
0
1
2
```

---

### **b) continue Statement**
Skips the current iteration and moves to the next.

```python
for i in range(5):
    if i == 2:
        continue  # Skips when i is 2
    print(i)
```
**Output:**
```
0
1
3
4
```

---

### **c) pass Statement**
A placeholder that does nothing.

```python
for i in range(3):
    pass  # Placeholder for future code
```
*(No output, just a placeholder)*

---

## **4. Nested Loops**
A loop inside another loop.

```python
for i in range(3):
    for j in range(3):
        print(f"i={i}, j={j}")
```
**Output:**
```
i=0, j=0
i=0, j=1
i=0, j=2
i=1, j=0
i=1, j=1
i=1, j=2
i=2, j=0
i=2, j=1
i=2, j=2
```

---

## **5. else with Loops**
The `else` block runs **only if the loop completes without `break`**.

### **Example: `for` loop with `else`**
```python
for i in range(3):
    print(i)
else:
    print("Loop completed without break")
```
**Output:**
```
0
1
2
Loop completed without break
```

### **Example: `while` loop with `else`**
```python
x = 0
while x < 3:
    print(x)
    x += 1
else:
    print("Loop completed")
```
**Output:**
```
0
1
2
Loop completed
```

---

### **Summary of Python Loops**
| Loop Type | When to Use |
|-----------|------------|
| `for` loop | When iterating over sequences (`list`, `tuple`, `string`, `range`, etc.) |
| `while` loop | When repeating a block **until a condition is false** |
| `break` | To exit a loop prematurely |
| `continue` | To skip an iteration and continue with the next one |
| `pass` | To use as a placeholder in loops |
