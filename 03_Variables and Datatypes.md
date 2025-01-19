### **Python Variables**
Variables are containers for storing data values. In Python, you don’t need to declare a variable explicitly; it is created as soon as you assign a value.

#### **Key Features of Python Variables**:
1. **Dynamic Typing**: The type of a variable is determined at runtime based on the assigned value.
   ```python
   x = 10        # Integer
   x = "Hello"   # Now a string
   ```

2. **No Declaration**: Variables do not need to be declared with a type or explicitly initialized.
   ```python
   name = "Alice"  # String
   age = 25        # Integer
   ```

3. **Case Sensitive**: Variables are case-sensitive.
   ```python
   var = 10
   Var = 20
   print(var, Var)  # Output: 10 20
   ```

#### **Variable Naming Rules**:
1. Must start with a letter (a-z, A-Z) or an underscore `_`.
2. Cannot start with a number.
3. Can only contain alphanumeric characters and underscores.
4. Cannot use Python keywords or built-in function names.
   ```python
   # Valid
   _my_var = 5
   var123 = "hello"

   # Invalid
   123var = 5       # Starts with a number
   for = 10         # Keyword
   ```

---

### **Python Data Types**
Python provides several built-in data types, categorized into basic, collection, and specialized types.

#### **1. Numeric Data Types**
- **int**: Integer values (e.g., `1`, `100`, `-50`).
  ```python
  age = 25  # int
  ```

- **float**: Floating-point numbers (e.g., `3.14`, `-0.5`).
  ```python
  price = 19.99  # float
  ```

- **complex**: Complex numbers with a real and imaginary part (e.g., `3+4j`).
  ```python
  number = 3 + 4j  # complex
  ```

#### **2. Text Data Type**
- **str**: Sequence of Unicode characters (e.g., `"Hello"`, `'World'`).
  ```python
  message = "Python is fun!"  # str
  ```

#### **3. Boolean Data Type**
- **bool**: Represents `True` or `False`.
  ```python
  is_active = True  # bool
  ```

#### **4. Sequence Data Types**
- **list**: Ordered, mutable collection (e.g., `[1, 2, 3]`).
  ```python
  fruits = ["apple", "banana", "cherry"]  # list
  ```

- **tuple**: Ordered, immutable collection (e.g., `(1, 2, 3)`).
  ```python
  coordinates = (10, 20, 30)  # tuple
  ```

- **range**: Sequence of numbers (e.g., `range(5)`).
  ```python
  numbers = range(5)  # range
  ```

#### **5. Set Data Types**
- **set**: Unordered collection of unique items (e.g., `{1, 2, 3}`).
  ```python
  unique_numbers = {1, 2, 3, 4}  # set
  ```

- **frozenset**: Immutable version of a set.
  ```python
  frozen = frozenset([1, 2, 3])  # frozenset
  ```

#### **6. Mapping Data Type**
- **dict**: Key-value pairs (e.g., `{"name": "Alice", "age": 25}`).
  ```python
  person = {"name": "Alice", "age": 25}  # dict
  ```

#### **7. Binary Data Types**
- **bytes**: Immutable sequence of bytes (e.g., `b"data"`).
  ```python
  byte_data = b"Hello"  # bytes
  ```

- **bytearray**: Mutable sequence of bytes.
  ```python
  mutable_bytes = bytearray(5)  # bytearray
  ```

- **memoryview**: Memory view of another binary data type.

#### **8. None Type**
- **None**: Represents the absence of a value.
  ```python
  result = None  # NoneType
  ```

---

### **Type Conversion**
You can convert between different data types using type-casting functions:
- `int()`: Converts to an integer.
- `float()`: Converts to a float.
- `str()`: Converts to a string.
- `list()`, `tuple()`, `set()`, etc.: Converts to the respective collection.

```python
x = "10"
y = int(x)  # Convert string to int
z = float(y)  # Convert int to float
```

---

### **Checking Data Type**
Use the `type()` function to check the data type of a variable:
```python
x = 42
print(type(x))  # Output: <class 'int'>
```
