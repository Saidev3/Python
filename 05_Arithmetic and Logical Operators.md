### **Basic Arithmetic and Logical Operators in Python**

#### **1. Arithmetic Operators**
Arithmetic operators perform mathematical operations on numbers.

| Operator | Name             | Example           | Description                       |
|----------|------------------|-------------------|-----------------------------------|
| `+`      | Addition         | `x + y`          | Adds `x` and `y`.                |
| `-`      | Subtraction      | `x - y`          | Subtracts `y` from `x`.          |
| `*`      | Multiplication   | `x * y`          | Multiplies `x` and `y`.          |
| `/`      | Division         | `x / y`          | Divides `x` by `y` (result is a float). |
| `//`     | Floor Division   | `x // y`         | Divides `x` by `y` (result is an integer, rounded down). |
| `%`      | Modulus          | `x % y`          | Returns the remainder of `x / y`. |
| `**`     | Exponentiation   | `x ** y`         | Raises `x` to the power of `y`.  |

#### **Examples**:
```python
x = 10
y = 3

print(x + y)   # 13
print(x - y)   # 7
print(x * y)   # 30
print(x / y)   # 3.3333333333333335
print(x // y)  # 3
print(x % y)   # 1
print(x ** y)  # 1000
```

---

#### **2. Logical Operators**
Logical operators are used to combine conditional statements and return Boolean values (`True` or `False`).

| Operator | Description                              | Example               |
|----------|------------------------------------------|-----------------------|
| `and`    | Returns `True` if both conditions are `True`.  | `x > 5 and y < 10`   |
| `or`     | Returns `True` if at least one condition is `True`. | `x > 5 or y < 1`    |
| `not`    | Reverses the result (negates the condition). | `not(x > 5)`         |

#### **Examples**:
```python
x = 10
y = 5

# Logical AND
print(x > 5 and y > 3)  # True (both conditions are True)
print(x > 5 and y > 10) # False (one condition is False)

# Logical OR
print(x > 5 or y > 10)  # True (one condition is True)
print(x < 5 or y > 10)  # False (both conditions are False)

# Logical NOT
print(not(x > 5))       # False (reverses the condition)
```

---

### **3. Combining Arithmetic and Logical Operators**
You can combine arithmetic and logical operators in more complex expressions.

#### Example:
```python
x = 15
y = 5
z = 20

# Combining arithmetic and logical operators
result = (x + y > z) and (z - x < y)
print(result)  # True
```

---

### **Operator Precedence**
The order in which operators are evaluated follows a standard precedence:
1. **Parentheses**: `()`
2. **Exponentiation**: `**`
3. **Multiplication/Division/Floor Division/Modulus**: `*`, `/`, `//`, `%`
4. **Addition/Subtraction**: `+`, `-`
5. **Comparison Operators**: `==`, `!=`, `<`, `>`, `<=`, `>=`
6. **Logical NOT**: `not`
7. **Logical AND**: `and`
8. **Logical OR**: `or`

#### Example:
```python
result = 5 + 2 * 3 ** 2 - 4 / 2
# Order: (3 ** 2) -> (2 * 9) -> (4 / 2) -> (5 + 18 - 2)
print(result)  # 21.0
```

---
