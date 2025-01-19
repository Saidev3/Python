### **Python Syntax**
Python syntax refers to the set of rules that define how Python programs are written and interpreted.

#### **Key Features of Python Syntax:**
1. **Indentation**: 
   - Python uses indentation to define blocks of code (e.g., in loops, conditionals, and functions).
   - Indentation is mandatory and replaces the use of `{}` found in other languages.
   ```python
   if True:
       print("This is indented!")  # Indented block
   ```

2. **Case Sensitivity**:
   - Python is case-sensitive, meaning `Variable` and `variable` are different.

3. **No Semicolons**:
   - Lines end without semicolons, although you can optionally use them.
   ```python
   print("Hello, World")  # No semicolon needed
   ```

4. **Multi-line Statements**:
   - Use a backslash (`\`) to continue a statement to the next line.
   ```python
   total = 1 + 2 + \
           3 + 4
   ```
   - Parentheses, brackets, or curly braces allow implicit line continuation.
   ```python
   total = (1 + 2 +
            3 + 4)
   ```

---

### **Python Keywords**
Keywords are reserved words that cannot be used as variable names, function names, or identifiers. Python has 35 keywords (as of Python 3.10).

#### **Common Python Keywords**:
| Keyword      | Description                        |
|--------------|------------------------------------|
| `False`      | Boolean value                     |
| `None`       | Represents a null value           |
| `True`       | Boolean value                     |
| `and`        | Logical operator                  |
| `as`         | Alias in `import`                 |
| `assert`     | Debugging tool                    |
| `break`      | Exit a loop                       |
| `class`      | Define a class                    |
| `continue`   | Skip to the next iteration         |
| `def`        | Define a function                 |
| `del`        | Delete an object                  |
| `elif`       | Else if condition                 |
| `else`       | Conditional statement             |
| `except`     | Handle exceptions                 |
| `finally`    | Execute after try block           |
| `for`        | Loop over a sequence              |
| `if`         | Conditional statement             |
| `import`     | Import a module                   |
| `in`         | Membership test or iteration      |
| `is`         | Object identity test              |
| `lambda`     | Anonymous function                |
| `not`        | Logical NOT                       |
| `or`         | Logical OR                        |
| `pass`       | Placeholder                       |
| `raise`      | Raise an exception                |
| `return`     | Return from a function            |
| `try`        | Handle exceptions                 |
| `while`      | Loop while a condition is true    |
| `with`       | Context management                |
| `yield`      | Pause and resume a generator      |

Use the `help("keywords")` command to list all Python keywords in your interpreter.

---

### **Python Comments**
Comments are used to explain code and are ignored during execution.

1. **Single-line Comments**:
   - Use the `#` symbol for single-line comments.
   ```python
   # This is a single-line comment
   print("Hello, World!")  # Inline comment
   ```

2. **Multi-line Comments**:
   - Use triple quotes (`'''` or `"""`) to create multi-line comments, though technically these are treated as docstrings.
   ```python
   """
   This is a
   multi-line comment
   """
   print("Python is fun!")
   ```

---
