### **🔥 Tuples in Python 🔥**

Tuples are one of the built-in data structures in Python that store an ordered collection of elements. Unlike lists, **tuples are immutable**, meaning that once created, you cannot change the elements within the tuple.

---

## **✅ Creating a Tuple**

You can create a tuple by enclosing elements in **parentheses** `()`.

```python
# Example 1: Simple Tuple
my_tuple = (10, 20, 30, 40)
print(my_tuple)  # Output: (10, 20, 30, 40)

# Example 2: Tuple with different data types
mixed_tuple = (1, "Hello", 3.14, True)
print(mixed_tuple)  # Output: (1, 'Hello', 3.14, True)
```

---

## **✅ Accessing Tuple Elements**

Just like lists, you can access tuple elements using **indexing** and **slicing**.

### **Indexing (Access by Position)**

```python
my_tuple = (10, 20, 30, 40)
print(my_tuple[0])  # Output: 10
print(my_tuple[-1])  # Output: 40 (Last element)
```

### **Slicing (Extract Sub-Tuple)**

```python
print(my_tuple[1:3])  # Output: (20, 30)
print(my_tuple[:2])   # Output: (10, 20)
print(my_tuple[::2])  # Output: (10, 30)
```

---

## **✅ Tuple Operations**

### **1️⃣ Concatenation**

You can join two tuples together using the `+` operator.

```python
tuple1 = (1, 2, 3)
tuple2 = (4, 5, 6)
combined_tuple = tuple1 + tuple2
print(combined_tuple)  # Output: (1, 2, 3, 4, 5, 6)
```

### **2️⃣ Repetition**

You can repeat a tuple using the `*` operator.

```python
repeated_tuple = (1, 2, 3) * 3
print(repeated_tuple)  # Output: (1, 2, 3, 1, 2, 3, 1, 2, 3)
```

---

## **✅ Tuple Methods**

Tuples have only two built-in methods:

### **1️⃣ `count()`**
Returns the number of occurrences of a specific element in the tuple.

```python
my_tuple = (10, 20, 30, 20, 20)
print(my_tuple.count(20))  # Output: 3
```

### **2️⃣ `index()`**
Returns the index of the first occurrence of a specific element.

```python
print(my_tuple.index(20))  # Output: 1 (First occurrence of 20)
```

---

## **✅ Immutability of Tuples**

You cannot modify a tuple directly. For example:

```python
my_tuple = (10, 20, 30)
# This will give an error!
# my_tuple[1] = 25  # TypeError: 'tuple' object does not support item assignment
```

---

## **✅ Nested Tuples**

Tuples can also contain other tuples as elements.

```python
nested_tuple = ((1, 2), (3, 4), (5, 6))
print(nested_tuple)  # Output: ((1, 2), (3, 4), (5, 6))

# Accessing elements in the nested tuple
print(nested_tuple[0])  # Output: (1, 2)
print(nested_tuple[1][1])  # Output: 4
```

---

## **✅ Tuple Packing and Unpacking**

### **Packing**
This is when multiple elements are grouped together into a tuple.

```python
packed_tuple = 1, 2, 3  # Tuple packing
print(packed_tuple)  # Output: (1, 2, 3)
```

### **Unpacking**
You can assign elements of a tuple to multiple variables.

```python
my_tuple = (10, 20, 30)
a, b, c = my_tuple  # Tuple unpacking
print(a)  # Output: 10
print(b)  # Output: 20
print(c)  # Output: 30
```

---

## **✅ Advantages of Tuples**

- **Faster than lists**: Since tuples are immutable, they are faster for iteration and accessing elements.
- **Data integrity**: Since they can't be changed, tuples are useful when you want to ensure that the data remains constant.
- **Hashable**: Tuples can be used as keys in a dictionary (while lists cannot).

---

## **🎯 Summary: Tuples in Python**

| **Operation**      | **Method**        | **Example**            |
|--------------------|-------------------|------------------------|
| **Create Tuple**   | `(1, 2, 3)`       | `my_tuple = (10, 20)`  |
| **Access by Index**| `my_tuple[1]`     | `print(my_tuple[0])`   |
| **Slicing**        | `my_tuple[1:3]`   | `print(my_tuple[1:])`  |
| **Concatenate**    | `tuple1 + tuple2` | `my_tuple + (4, 5)`    |
| **Repeat**         | `tuple * n`       | `(1, 2) * 3`           |
| **Count**          | `my_tuple.count(x)`| `my_tuple.count(2)`    |
| **Index**          | `my_tuple.index(x)`| `my_tuple.index(20)`   |
| **Packing**        | `a, b = (1, 2)`   | `x, y = (1, 2)`        |
| **Unpacking**      | `a, b = my_tuple` | `x, y = (10, 20)`      |

---

