In Python, conditional statements are used to execute certain code based on whether a condition is true or false. The primary conditional statements are `if`, `elif`, and `else`.

### 1. **`if` statement**
The `if` statement evaluates a condition, and if it is true, the code block inside the `if` is executed.

```python
age = 20
if age >= 18:
    print("You are an adult.")
```

### 2. **`elif` (else if) statement**
If the condition in the `if` statement is false, the program checks for conditions in the `elif` statement(s) (if any). It allows you to check multiple conditions.

```python
age = 15
if age >= 18:
    print("You are an adult.")
elif age >= 13:
    print("You are a teenager.")
```

### 3. **`else` statement**
The `else` statement is executed when none of the preceding `if` or `elif` conditions are true.

```python
age = 10
if age >= 18:
    print("You are an adult.")
elif age >= 13:
    print("You are a teenager.")
else:
    print("You are a child.")
```

### Example:
```python
x = 10

if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")
```

### Output:
```python
x is greater than 5
```

In this example, the first condition (`x > 5`) is true, so the corresponding block is executed.
