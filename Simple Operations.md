Python supports various simple operations on different data types. Below are some fundamental operations:

---

## **1. Arithmetic Operations**
Used for mathematical calculations.

```python
a = 10
b = 3

print(a + b)   # Addition → 13
print(a - b)   # Subtraction → 7
print(a * b)   # Multiplication → 30
print(a / b)   # Division → 3.333...
print(a // b)  # Floor Division → 3 (removes decimal part)
print(a % b)   # Modulus (Remainder) → 1
print(a ** b)  # Exponentiation (Power) → 10³ = 1000
```

---

## **2. Comparison Operations**
Used for comparing values.

```python
print(a > b)   # Greater than → True
print(a < b)   # Less than → False
print(a == b)  # Equal to → False
print(a != b)  # Not equal to → True
print(a >= b)  # Greater than or equal → True
print(a <= b)  # Less than or equal → False
```

---

## **3. Logical Operations**
Used for Boolean logic.

```python
x = True
y = False

print(x and y)  # AND → False
print(x or y)   # OR → True
print(not x)    # NOT → False
```

---

## **4. Assignment Operations**
Used for assigning values to variables.

```python
a = 5   # Assign 5 to a
a += 2  # a = a + 2 → 7
a -= 1  # a = a - 1 → 6
a *= 3  # a = a * 3 → 18
a /= 2  # a = a / 2 → 9.0
```

---

## **5. Bitwise Operations**
Used for operations on binary numbers.

```python
x = 5   # 0101 (binary)
y = 3   # 0011 (binary)

print(x & y)  # AND → 0001 (1)
print(x | y)  # OR → 0111 (7)
print(x ^ y)  # XOR → 0110 (6)
print(~x)     # NOT → -6
print(x << 1) # Left Shift → 1010 (10)
print(x >> 1) # Right Shift → 0010 (2)
```

---

## **6. Membership Operations**
Used for checking if a value is in a sequence.

```python
lst = [1, 2, 3, 4, 5]

print(3 in lst)  # True
print(6 not in lst)  # True
```

---

## **7. Identity Operations**
Used for checking object identity.

```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)   # True (same object)
print(a is c)   # False (different objects with same values)
print(a == c)   # True (values are same)
```
