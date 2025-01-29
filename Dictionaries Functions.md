### **🔥 Dictionaries in Python 🔥**

A **dictionary** in Python is an unordered collection of **key-value pairs**. Each key is unique, and it is associated with a value. Unlike lists or tuples, dictionaries do not store elements in a specific order. They are very useful when you want to store data that is related in pairs, such as name and age or product and price.

---

## **✅ Creating a Dictionary**

You can create a dictionary by enclosing key-value pairs in curly braces `{}`. The key and value are separated by a colon `:`.

```python
# Example 1: Simple Dictionary
my_dict = {"name": "John", "age": 30, "city": "New York"}
print(my_dict)  # Output: {'name': 'John', 'age': 30, 'city': 'New York'}

# Example 2: Dictionary with different data types
mixed_dict = {"name": "Alice", "age": 25, "height": 5.5, "is_student": True}
print(mixed_dict)  # Output: {'name': 'Alice', 'age': 25, 'height': 5.5, 'is_student': True}
```

---

## **✅ Accessing Dictionary Elements**

You can access the values in a dictionary by using the **key**.

```python
my_dict = {"name": "John", "age": 30, "city": "New York"}

# Accessing value using key
print(my_dict["name"])  # Output: John

# Using get() method (it returns None if the key doesn't exist)
print(my_dict.get("age"))  # Output: 30
print(my_dict.get("country"))  # Output: None
```

---

## **✅ Adding and Modifying Items**

You can add new items or modify existing items in a dictionary by using the key.

```python
my_dict = {"name": "John", "age": 30}

# Adding a new key-value pair
my_dict["city"] = "New York"
print(my_dict)  # Output: {'name': 'John', 'age': 30, 'city': 'New York'}

# Modifying an existing value
my_dict["age"] = 31
print(my_dict)  # Output: {'name': 'John', 'age': 31, 'city': 'New York'}
```

---

## **✅ Removing Items**

You can remove items from a dictionary using several methods.

### **1️⃣ `pop()`**
Removes an item by its key and returns its value.

```python
my_dict = {"name": "John", "age": 30, "city": "New York"}
removed_value = my_dict.pop("age")
print(removed_value)  # Output: 30
print(my_dict)  # Output: {'name': 'John', 'city': 'New York'}
```

### **2️⃣ `popitem()`**
Removes the last inserted item (since Python 3.7+, dictionaries maintain insertion order).

```python
my_dict = {"name": "John", "age": 30, "city": "New York"}
removed_item = my_dict.popitem()
print(removed_item)  # Output: ('city', 'New York')
print(my_dict)  # Output: {'name': 'John', 'age': 30}
```

### **3️⃣ `del`**
Deletes a key-value pair by specifying the key.

```python
my_dict = {"name": "John", "age": 30, "city": "New York"}
del my_dict["age"]
print(my_dict)  # Output: {'name': 'John', 'city': 'New York'}
```

### **4️⃣ `clear()`**
Removes all items from the dictionary.

```python
my_dict = {"name": "John", "age": 30, "city": "New York"}
my_dict.clear()
print(my_dict)  # Output: {}
```

---

## **✅ Dictionary Methods**

Here are some useful methods for working with dictionaries:

- **`keys()`**: Returns a view of all the keys in the dictionary.

```python
print(my_dict.keys())  # Output: dict_keys(['name', 'age'])
```

- **`values()`**: Returns a view of all the values in the dictionary.

```python
print(my_dict.values())  # Output: dict_values(['John', 30])
```

- **`items()`**: Returns a view of all key-value pairs as tuples.

```python
print(my_dict.items())  # Output: dict_items([('name', 'John'), ('age', 30)])
```

- **`update()`**: Updates the dictionary with another dictionary or key-value pairs.

```python
my_dict = {"name": "John", "age": 30}
my_dict.update({"city": "New York", "age": 31})
print(my_dict)  # Output: {'name': 'John', 'age': 31, 'city': 'New York'}
```

---

## **✅ Nested Dictionaries**

Dictionaries can contain other dictionaries, which is useful for organizing complex data.

```python
nested_dict = {
    "person1": {"name": "Alice", "age": 25},
    "person2": {"name": "Bob", "age": 30}
}
print(nested_dict["person1"]["name"])  # Output: Alice
print(nested_dict["person2"]["age"])   # Output: 30
```

---

## **✅ Dictionary Comprehension**

You can create dictionaries using **dictionary comprehension**, which is similar to list comprehension.

```python
# Creating a dictionary of squares
squares = {x: x**2 for x in range(1, 6)}
print(squares)  # Output: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

---

## **✅ Advantages of Dictionaries**

- **Efficient lookup**: Since dictionaries use keys, the values can be accessed very quickly, even for large datasets.
- **Flexible**: You can store any type of data as the value (including other dictionaries, lists, tuples, etc.).
- **Insertion order**: In Python 3.7+, dictionaries maintain insertion order, so the items are stored in the order in which they were added.

---

## **🎯 Summary: Dictionaries in Python**

| **Operation**        | **Method**              | **Example**               |
|----------------------|-------------------------|---------------------------|
| **Create Dictionary** | `{"key": value}`        | `my_dict = {"name": "John", "age": 30}` |
| **Access by Key**     | `my_dict["key"]`        | `my_dict["name"]`         |
| **Get with Default**  | `my_dict.get("key")`    | `my_dict.get("city")`     |
| **Add/Modify Items**  | `my_dict["key"] = value`| `my_dict["age"] = 31`     |
| **Remove with pop()** | `my_dict.pop("key")`    | `my_dict.pop("age")`      |
| **Remove with del**   | `del my_dict["key"]`    | `del my_dict["city"]`     |
| **Clear Dictionary**  | `my_dict.clear()`       | `my_dict.clear()`         |
| **Keys**              | `my_dict.keys()`        | `my_dict.keys()`          |
| **Values**            | `my_dict.values()`      | `my_dict.values()`        |
| **Items**             | `my_dict.items()`       | `my_dict.items()`         |
| **Update Dictionary** | `my_dict.update()`      | `my_dict.update({"city": "New York"})` |
