### **🔥 Sets in Python 🔥**

A **set** in Python is an unordered collection of **unique** elements. Unlike lists or tuples, sets do not allow duplicate elements, and they do not maintain any order of elements.

Sets are useful when you need to store a collection of items where duplicate values should not be allowed and the order of the items doesn't matter.

---

## **✅ Creating a Set**

You can create a set by enclosing elements in curly braces `{}` or using the `set()` constructor.

```python
# Example 1: Creating a set with curly braces
my_set = {1, 2, 3, 4, 5}
print(my_set)  # Output: {1, 2, 3, 4, 5}

# Example 2: Creating a set using the set() constructor
my_set = set([1, 2, 3, 4, 5])
print(my_set)  # Output: {1, 2, 3, 4, 5}

# Example 3: Creating an empty set
empty_set = set()
print(empty_set)  # Output: set()

# Example 4: Creating a set from a string (removes duplicates)
my_set = set("hello")
print(my_set)  # Output: {'h', 'e', 'l', 'o'}
```

---

## **✅ Properties of Sets**

1. **Unordered**: The elements in a set are not stored in any specific order.
2. **Unique elements**: A set automatically removes any duplicate values.
3. **Mutable**: You can add or remove items after a set is created.
4. **No indexing or slicing**: You cannot access elements of a set by index (since it's unordered).
5. **Supports mathematical set operations**: You can perform set operations like union, intersection, and difference.

---

## **✅ Adding and Removing Items**

You can add or remove items from a set using built-in methods.

### **1️⃣ `add()`**
Adds an element to the set.

```python
my_set = {1, 2, 3}
my_set.add(4)
print(my_set)  # Output: {1, 2, 3, 4}
```

### **2️⃣ `update()`**
Adds multiple elements (from an iterable) to the set.

```python
my_set = {1, 2, 3}
my_set.update([4, 5, 6])
print(my_set)  # Output: {1, 2, 3, 4, 5, 6}
```

### **3️⃣ `remove()`**
Removes an element from the set. If the element doesn't exist, it raises a KeyError.

```python
my_set = {1, 2, 3}
my_set.remove(2)
print(my_set)  # Output: {1, 3}
```

### **4️⃣ `discard()`**
Removes an element from the set. If the element doesn't exist, it does **not** raise an error.

```python
my_set = {1, 2, 3}
my_set.discard(4)  # Does nothing because 4 is not in the set
print(my_set)  # Output: {1, 2, 3}
```

### **5️⃣ `pop()`**
Removes and returns a random element from the set (since sets are unordered).

```python
my_set = {1, 2, 3}
removed_element = my_set.pop()
print(removed_element)  # Output: 1 (or some other element, random order)
print(my_set)  # Output: {2, 3} (order might differ)
```

### **6️⃣ `clear()`**
Removes all elements from the set.

```python
my_set = {1, 2, 3}
my_set.clear()
print(my_set)  # Output: set()
```

---

## **✅ Set Operations**

You can perform various mathematical set operations such as union, intersection, difference, and symmetric difference.

### **1️⃣ `union()`**
Returns a new set that contains all elements from both sets (removes duplicates).

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
union_set = set1.union(set2)
print(union_set)  # Output: {1, 2, 3, 4, 5}
```

Alternatively, you can use the `|` operator for union:

```python
union_set = set1 | set2
print(union_set)  # Output: {1, 2, 3, 4, 5}
```

### **2️⃣ `intersection()`**
Returns a new set with elements that are common in both sets.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
intersection_set = set1.intersection(set2)
print(intersection_set)  # Output: {3}
```

Alternatively, you can use the `&` operator for intersection:

```python
intersection_set = set1 & set2
print(intersection_set)  # Output: {3}
```

### **3️⃣ `difference()`**
Returns a new set with elements that are in the first set but not in the second.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
difference_set = set1.difference(set2)
print(difference_set)  # Output: {1, 2}
```

Alternatively, you can use the `-` operator for difference:

```python
difference_set = set1 - set2
print(difference_set)  # Output: {1, 2}
```

### **4️⃣ `symmetric_difference()`**
Returns a new set with elements that are in either of the sets but not in both.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
sym_diff_set = set1.symmetric_difference(set2)
print(sym_diff_set)  # Output: {1, 2, 4, 5}
```

Alternatively, you can use the `^` operator for symmetric difference:

```python
sym_diff_set = set1 ^ set2
print(sym_diff_set)  # Output: {1, 2, 4, 5}
```

---

## **✅ Set Comprehension**

Just like list comprehension, you can use **set comprehension** to create a new set based on some iterable.

```python
# Creating a set of squares
squares = {x**2 for x in range(1, 6)}
print(squares)  # Output: {1, 4, 9, 16, 25}
```

---

## **✅ Set Methods**

Here are some commonly used set methods:

- **`copy()`**: Returns a shallow copy of the set.

```python
my_set = {1, 2, 3}
copy_set = my_set.copy()
print(copy_set)  # Output: {1, 2, 3}
```

- **`isdisjoint()`**: Returns `True` if two sets have no elements in common.

```python
set1 = {1, 2, 3}
set2 = {4, 5, 6}
print(set1.isdisjoint(set2))  # Output: True
```

- **`issubset()`**: Returns `True` if all elements of the set are in another set.

```python
set1 = {1, 2}
set2 = {1, 2, 3}
print(set1.issubset(set2))  # Output: True
```

- **`issuperset()`**: Returns `True` if the set contains all elements of another set.

```python
set1 = {1, 2, 3}
set2 = {2, 3}
print(set1.issuperset(set2))  # Output: True
```

---

## **✅ Summary: Sets in Python**

| **Operation**           | **Method/Operator**     | **Example**                  |
|-------------------------|-------------------------|------------------------------|
| **Create Set**          | `{}` or `set()`         | `my_set = {1, 2, 3}`         |
| **Add Element**         | `add()`                 | `my_set.add(4)`              |
| **Add Multiple Elements** | `update()`             | `my_set.update([4, 5])`      |
| **Remove Element**      | `remove()`              | `my_set.remove(2)`           |
| **Remove Element Safely**| `discard()`             | `my_set.discard(4)`          |
| **Remove Random Element**| `pop()`                 | `my_set.pop()`               |
| **Clear Set**           | `clear()`               | `my_set.clear()`             |
| **Union**               | `union()` or `|`        | `set1 | set2`                |
| **Intersection**        | `intersection()` or `&` | `set1 & set2`                |
| **Difference**          | `difference()` or `-`   | `set1 - set2`                |
| **Symmetric Difference**| `symmetric_difference()` or `^` | `set1 ^ set2`   |
