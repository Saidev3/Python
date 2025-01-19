In Python, functions are defined using the `def` keyword, followed by the function name, parameters (optional), and a block of code. Functions are called by using their name followed by parentheses.

### 1. **Defining a Function**
To define a function, you use the `def` keyword followed by the function name and any parameters inside parentheses. The code block that follows the function definition is indented.

```python
def greet():
    print("Hello, welcome to Python!")
```

In this example, `greet` is a function that doesn't take any parameters and simply prints a greeting message.

### 2. **Calling a Function**
Once a function is defined, you can call it by writing its name followed by parentheses.

```python
greet()  # Calling the function
```

### Output:
```
Hello, welcome to Python!
```

### 3. **Function with Parameters**
Functions can accept parameters, which allow you to pass values to the function when calling it.

```python
def greet(name):
    print(f"Hello, {name}!")
```

In this case, the `greet` function takes one parameter `name`.

### Calling the function with an argument:
```python
greet("Saidev")  # Passing the argument "Saidev"
```

### Output:
```
Hello, Saidev!
```

### 4. **Function with Return Value**
You can use the `return` keyword in a function to return a value to the caller. The `return` statement exits the function and sends a result back.

```python
def add(a, b):
    return a + b
```

### Calling the function and using the return value:
```python
result = add(3, 5)
print(result)
```

### Output:
```
8
```

### 5. **Function with Default Parameters**
You can define default values for function parameters. If a value is not passed when calling the function, the default value is used.

```python
def greet(name="Guest"):
    print(f"Hello, {name}!")
```

### Calling the function:
```python
greet("Alice")  # Passing a value
greet()         # Using the default value
```

### Output:
```
Hello, Alice!
Hello, Guest!
```

### 6. **Variable Scope in Functions**
Variables defined inside a function are local to that function, meaning they can't be accessed outside of it.

```python
x = 20

def example():
    x = 10  # Local variable
    print(x) # 10

print(x) # 20
example()
print(x) # 20
```

### Summary:
- **Defining a function**: Use `def` followed by the function name and parameters.
- **Calling a function**: Use the function name followed by parentheses, passing arguments if required.
- **Return values**: Use `return` to send values back from the function.
- **Default parameters**: You can set default values for parameters to use when no argument is passed.
- **Local variables**: Variables inside a function cannot be accessed outside the function.
