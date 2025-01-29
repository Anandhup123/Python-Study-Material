In Python, data types define the kind of data a variable can hold. Python has several built-in data types:

### **1. Numeric Types**
   - **int** → Integer (e.g., `10`, `-5`, `1000`)
   - **float** → Floating-point number (e.g., `10.5`, `-3.14`)
   - **complex** → Complex number (e.g., `3+5j`, `-2j`)

### **2. Sequence Types**
   - **str** → String (e.g., `"Hello"`, `'Python'`)
   - **list** → Ordered, mutable collection (e.g., `[1, 2, 3]`, `['a', 'b', 'c']`)
   - **tuple** → Ordered, immutable collection (e.g., `(1, 2, 3)`, `('x', 'y')`)
   - **range** → Sequence of numbers (e.g., `range(5) → 0,1,2,3,4`)

### **3. Set Types**
   - **set** → Unordered, mutable collection of unique elements (e.g., `{1, 2, 3}`)
   - **frozenset** → Immutable version of a set (e.g., `frozenset({1, 2, 3})`)

### **4. Mapping Type**
   - **dict** → Key-value pairs (e.g., `{"name": "John", "age": 25}`)

### **5. Boolean Type**
   - **bool** → Represents `True` or `False`

### **6. Binary Types**
   - **bytes** → Immutable byte sequence (e.g., `b"hello"`)
   - **bytearray** → Mutable byte sequence (e.g., `bytearray([65, 66, 67])`)
   - **memoryview** → Memory view object (e.g., `memoryview(b"abc")`)

### **7. None Type**
   - **NoneType** → Represents absence of a value (`None`)

#### **Example Usage**
```python
x = 10            # int
y = 3.14         # float
z = 2 + 3j       # complex
s = "Hello"      # str
lst = [1, 2, 3]  # list
tup = (1, 2, 3)  # tuple
st = {1, 2, 3}   # set
dct = {"a": 1}   # dict
b = True         # bool
n = None         # NoneType
```