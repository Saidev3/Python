### **Input and Output in Python**
Python provides simple built-in functions for input and output operations. Let's go over them in detail.

---

### **1. Input in Python**
The `input()` function is used to take input from the user.

#### **Basic Usage**
- The `input()` function reads the input as a string.
  ```python
  name = input("Enter your name: ")
  print("Hello, " + name + "!")
  ```

#### **Converting Input to Other Data Types**
- Use type-casting functions like `int()`, `float()`, etc., to convert user input.
  ```python
  age = int(input("Enter your age: "))
  print("You are", age, "years old!")
  ```

#### **Example: Adding Two Numbers**
```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
print("The sum is:", num1 + num2)
```

---

### **2. Output in Python**
The `print()` function is used to display output to the user.

#### **Basic Usage**
```python
print("Hello, World!")
```

#### **Printing Multiple Values**
- Separate multiple values with commas. Python automatically inserts a space between them.
  ```python
  name = "Alice"
  age = 25
  print("Name:", name, "Age:", age)
  ```

#### **Using String Formatting**
- **f-strings** (Python 3.6+):
  ```python
  name = "Alice"
  age = 25
  print(f"My name is {name}, and I am {age} years old.")
  ```

- **`format()` Method**:
  ```python
  print("My name is {}, and I am {} years old.".format(name, age))
  ```

- **Old-style Formatting (`%` Operator)**:
  ```python
  print("My name is %s, and I am %d years old." % (name, age))
  ```

#### **Changing Separator and End Characters**
- **`sep` Parameter**: Specifies the separator between values.
  ```python
  print("apple", "banana", "cherry", sep=", ")
  ```

- **`end` Parameter**: Changes the ending character (default is a newline `\n`).
  ```python
  print("Hello", end=" ")
  print("World!")
  ```

---

### **3. Example Program: Simple Calculator**
```python
print("Simple Calculator")
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))

print("Choose an operation:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

choice = int(input("Enter your choice (1-4): "))

if choice == 1:
    print("Result:", num1 + num2)
elif choice == 2:
    print("Result:", num1 - num2)
elif choice == 3:
    print("Result:", num1 * num2)
elif choice == 4:
    if num2 != 0:
        print("Result:", num1 / num2)
    else:
        print("Error: Division by zero is not allowed!")
else:
    print("Invalid choice.")
```

---

### **4. Advanced Output Formatting**
Python provides the `format()` function and formatted string literals for more control.

#### **Controlling Decimal Places**
- Using `:.nf` (where `n` is the number of decimal places):
  ```python
  pi = 3.14159265358979
  print(f"Pi to 2 decimal places: {pi:.2f}")
  ```

#### **Padding and Alignment**
- Left-align, right-align, and center-align using `<`, `>`, and `^`:
  ```python
  print(f"{'Name':<10}{'Age':>5}")
  print(f"{'Alice':<10}{25:>5}")
  ```

#### **Printing Percentages**
- Use `:.n%` for percentages:
  ```python
  success_rate = 0.857
  print(f"Success rate: {success_rate:.2%}")
  ```

---
