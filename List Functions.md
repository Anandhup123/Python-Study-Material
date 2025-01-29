### **🔥 List Operations in Python 🔥**
Lists are one of the most powerful data structures in Python. You can perform various operations like adding, removing, sorting, and modifying list elements.

---

## **✅ Basic List Operations**

### **1️⃣ Creating a List**
```python
my_list = [10, 20, 30, 40, 50]
print(my_list)  # Output: [10, 20, 30, 40, 50]
```

---

## **✅ Accessing Elements**

### **2️⃣ Indexing (Accessing Elements by Index)**
```python
print(my_list[0])   # Output: 10
print(my_list[-1])  # Output: 50 (Last element)
```

### **3️⃣ Slicing (Extracting a Part of the List)**
```python
print(my_list[1:4])  # Output: [20, 30, 40] (from index 1 to 3)
print(my_list[:3])   # Output: [10, 20, 30] (first 3 elements)
print(my_list[::2])  # Output: [10, 30, 50] (every second element)
```

---

## **✅ Adding Elements to a List**

### **4️⃣ Using `append()` (Adds Element at the End)**
```python
my_list.append(60)
print(my_list)  # Output: [10, 20, 30, 40, 50, 60]
```

### **5️⃣ Using `insert()` (Adds Element at Specific Position)**
```python
my_list.insert(2, 25)
print(my_list)  # Output: [10, 20, 25, 30, 40, 50]
```

### **6️⃣ Using `extend()` (Merges Two Lists)**
```python
new_list = [70, 80]
my_list.extend(new_list)
print(my_list)  # Output: [10, 20, 30, 40, 50, 70, 80]
```

---

## **✅ Removing Elements from a List**

### **7️⃣ Using `remove()` (Removes Specific Value)**
```python
my_list.remove(30)
print(my_list)  # Output: [10, 20, 40, 50]
```

### **8️⃣ Using `pop()` (Removes and Returns an Element by Index)**
```python
removed_element = my_list.pop(2)
print(removed_element)  # Output: 40
print(my_list)  # Output: [10, 20, 50]
```

### **9️⃣ Using `clear()` (Removes All Elements)**
```python
my_list.clear()
print(my_list)  # Output: []
```

---

## **✅ Modifying Elements in a List**

### **🔟 Changing an Element**
```python
my_list = [10, 20, 30, 40]
my_list[2] = 35
print(my_list)  # Output: [10, 20, 35, 40]
```

---

## **✅ Searching for Elements in a List**

### **1️⃣1️⃣ Using `index()` (Finds Position of an Element)**
```python
position = my_list.index(35)
print(position)  # Output: 2
```

### **1️⃣2️⃣ Using `count()` (Counts the Number of Occurrences)**
```python
count = my_list.count(20)
print(count)  # Output: 1
```

---

## **✅ Sorting and Reversing a List**

### **1️⃣3️⃣ Using `sort()` (Sorts in Ascending Order)**
```python
my_list = [40, 10, 30, 20]
my_list.sort()
print(my_list)  # Output: [10, 20, 30, 40]
```

### **1️⃣4️⃣ Using `sort(reverse=True)` (Sorts in Descending Order)**
```python
my_list.sort(reverse=True)
print(my_list)  # Output: [40, 30, 20, 10]
```

### **1️⃣5️⃣ Using `reverse()` (Reverses the List)**
```python
my_list.reverse()
print(my_list)  # Output: [10, 20, 30, 40]
```

---

## **✅ Copying a List**

### **1️⃣6️⃣ Using `copy()` (Creates a Copy of the List)**
```python
copy_list = my_list.copy()
print(copy_list)  # Output: [10, 20, 30, 40]
```

---

## **✅ List Comprehensions (One-Line List Creation)**

### **1️⃣7️⃣ Creating a List with `for` Loop**
```python
squares = [x**2 for x in range(1, 6)]
print(squares)  # Output: [1, 4, 9, 16, 25]
```

### **1️⃣8️⃣ Filtering a List**
```python
evens = [x for x in range(10) if x % 2 == 0]
print(evens)  # Output: [0, 2, 4, 6, 8]
```

---

## **🎯 Summary: Most Common List Operations**
| **Operation**        | **Method**                  | **Example** |
|----------------------|----------------------------|-------------|
| **Add Element**      | `append(x)`, `insert(i, x)`, `extend(list)` | `my_list.append(5)` |
| **Remove Element**   | `remove(x)`, `pop(i)`, `clear()` | `my_list.remove(5)` |
| **Find Element**     | `index(x)`, `count(x)` | `my_list.index(3)` |
| **Modify Element**   | `my_list[i] = x` | `my_list[1] = 10` |
| **Sorting**         | `sort()`, `sort(reverse=True)`, `reverse()` | `my_list.sort()` |
| **Copying**         | `copy()` | `new_list = my_list.copy()` |
| **Comprehension**   | `[x for x in list]` | `[x**2 for x in range(5)]` |