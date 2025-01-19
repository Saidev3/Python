In Python, **strings** are sequences of characters used to store and manipulate text. Strings are immutable, meaning their contents cannot be changed after creation.

---

### Creating Strings
You can create strings using single quotes (`'`), double quotes (`"`), or triple quotes (`'''` or """ """).

```python
# Using single or double quotes
string1 = 'Hello'
string2 = "World"

# Using triple quotes for multiline strings
multiline_string = """This is a
multiline string."""
```

---

### Accessing Characters in a String
You can access characters using indexing (0-based) and retrieve substrings using slicing.

```python
text = "Python"

# Accessing individual characters
print(text[0])   # Output: P
print(text[-1])  # Output: n (last character)

# Slicing strings
print(text[1:4])  # Output: yth
print(text[:3])   # Output: Pyt (first 3 characters)
print(text[3:])   # Output: hon (from index 3 to end)
```

---

### String Operations

#### 1. Concatenation
Strings can be concatenated using the `+` operator or combined with `join()`.

```python
str1 = "Hello"
str2 = "World"
result = str1 + " " + str2
print(result)  # Output: Hello World
```

#### 2. Repetition
You can repeat a string using the `*` operator.

```python
repeated = "Ha" * 3
print(repeated)  # Output: HaHaHa
```

#### 3. Length
Use the `len()` function to find the length of a string.

```python
print(len("Python"))  # Output: 6
```

#### 4. Membership Testing
You can check if a substring exists using `in` or `not in`.

```python
text = "Hello World"
print("World" in text)  # Output: True
print("Python" not in text)  # Output: True
```

---

### Common String Methods
Python provides many built-in methods for string manipulation:

#### Changing Case
```python
text = "Hello World"

print(text.lower())   # Output: hello world
print(text.upper())   # Output: HELLO WORLD
print(text.title())   # Output: Hello World
print(text.capitalize())  # Output: Hello world
print(text.swapcase())    # Output: hELLO wORLD
```

#### Trimming Whitespace
```python
text = "  Hello  "
print(text.strip())   # Output: Hello (removes leading/trailing spaces)
print(text.lstrip())  # Output: Hello   (removes leading spaces)
print(text.rstrip())  # Output:   Hello (removes trailing spaces)
```

#### Finding and Replacing
```python
text = "Hello, World"
print(text.find("World"))     # Output: 7 (index of substring)
print(text.replace("World", "Python"))  # Output: Hello, Python
```

#### Splitting and Joining
```python
text = "Hello World Python"

# Splitting a string into a list
words = text.split()  # Default split by spaces
print(words)  # Output: ['Hello', 'World', 'Python']

# Joining a list into a string
joined = "-".join(words)
print(joined)  # Output: Hello-World-Python
```

#### Checking String Properties
```python
text = "Python3"

print(text.isalpha())  # Output: False (contains numbers)
print(text.isdigit())  # Output: False (not all characters are digits)
print("123".isdigit())  # Output: True
print("hello".islower())  # Output: True
print("HELLO".isupper())  # Output: True
```

---

### String Formatting
String formatting allows you to insert variables into strings.

#### 1. Using f-strings (Python 3.6+)
```python
name = "Alice"
age = 25
print(f"My name is {name} and I am {age} years old.")
```

#### 2. Using `str.format()`
```python
print("My name is {} and I am {} years old.".format(name, age))
```

#### 3. Using `%` Formatting
```python
print("My name is %s and I am %d years old." % (name, age))
```

---

### Escape Characters
Escape sequences are used to include special characters in strings.

| Escape Sequence | Description          |
|------------------|----------------------|
| `\'`            | Single quote         |
| `\"`            | Double quote         |
| `\\`            | Backslash           |
| `\n`            | Newline             |
| `\t`            | Tab                 |

```python
text = "Hello\nWorld\t!"
print(text)
# Output:
# Hello
# World    !
```

---

### Raw Strings
Raw strings treat backslashes as literal characters. Prefix the string with `r`.

```python
path = r"C:\Users\Saidev"
print(path)  # Output: C:\Users\Saidev
```

---

### Iterating Over Strings
You can iterate over each character in a string using a `for` loop.

```python
for char in "Python":
    print(char)
# Output:
# P
# y
# t
# h
# o
# n
```

---

### Summary of String Methods

| Method                | Description                               |
|-----------------------|-------------------------------------------|
| `lower()`             | Converts all characters to lowercase.    |
| `upper()`             | Converts all characters to uppercase.    |
| `title()`             | Converts to title case.                  |
| `strip()`             | Removes leading and trailing spaces.     |
| `replace(old, new)`   | Replaces occurrences of a substring.     |
| `split(separator)`    | Splits string into a list of substrings. |
| `join(iterable)`      | Joins elements of an iterable into a string. |
| `find(substring)`     | Returns index of the first occurrence of a substring. |
| `startswith(prefix)`  | Checks if the string starts with a prefix. |
| `endswith(suffix)`    | Checks if the string ends with a suffix.  |
| `isalpha()`           | Checks if all characters are alphabets.  |
| `isdigit()`           | Checks if all characters are digits.     |

---

### Immutability of Strings
Strings are immutable, meaning once created, their contents cannot be changed. Any operation that modifies a string creates a new string instead.

```python
text = "Hello"
text = text + " World"
print(text)  # Output: Hello World
```
