The `re` module in Python is used for working with **regular expressions**, which are patterns used for matching text. It provides functions to search, match, and manipulate strings using regex patterns. Here's an overview:

---

### **Common Functions in `re`**

#### 1. **`re.match()`**
   - Checks for a match at the **start** of the string.
   - **Example**:
     ```python
     import re

     result = re.match(r"hello", "hello world")
     print(result)  # <re.Match object; span=(0, 5), match='hello'>
     print(result.group())  # hello
     ```

#### 2. **`re.search()`**
   - Searches for the **first occurrence** of the pattern in the string.
   - **Example**:
     ```python
     result = re.search(r"world", "hello world")
     print(result)  # <re.Match object; span=(6, 11), match='world'>
     print(result.group())  # world
     ```

#### 3. **`re.findall()`**
   - Returns **all occurrences** of the pattern as a list.
   - **Example**:
     ```python
     result = re.findall(r"o", "hello world")
     print(result)  # ['o', 'o']
     ```

#### 4. **`re.finditer()`**
   - Returns an **iterator** yielding match objects for each match.
   - **Example**:
     ```python
     result = re.finditer(r"o", "hello world")
     for match in result:
         print(match)  # <re.Match object> for each match
     ```

#### 5. **`re.sub()`**
   - Replaces matches with a specified string.
   - **Example**:
     ```python
     result = re.sub(r"world", "Python", "hello world")
     print(result)  # hello Python
     ```

#### 6. **`re.split()`**
   - Splits the string by the occurrences of the pattern.
   - **Example**:
     ```python
     result = re.split(r"\s", "hello world")
     print(result)  # ['hello', 'world']
     ```

#### 7. **`re.fullmatch()`**
   - Checks if the **entire string** matches the pattern.
   - **Example**:
     ```python
     result = re.fullmatch(r"hello world", "hello world")
     print(result)  # <re.Match object; span=(0, 11), match='hello world'>
     ```

---

### **Regex Patterns**
- **Meta-characters**:
  - `.`: Matches any character except a newline.
  - `^`: Matches the start of the string.
  - `$`: Matches the end of the string.
  - `*`: Matches 0 or more repetitions of the preceding character.
  - `+`: Matches 1 or more repetitions of the preceding character.
  - `?`: Matches 0 or 1 of the preceding character.
  - `{n,m}`: Matches between `n` and `m` repetitions.

- **Character Sets**:
  - `[abc]`: Matches `a`, `b`, or `c`.
  - `[a-z]`: Matches any lowercase letter.
  - `[^abc]`: Matches anything except `a`, `b`, or `c`.

- **Special Sequences**:
  - `\d`: Matches any digit (equivalent to `[0-9]`).
  - `\D`: Matches any non-digit.
  - `\w`: Matches any word character (alphanumeric + underscore).
  - `\W`: Matches any non-word character.
  - `\s`: Matches any whitespace.
  - `\S`: Matches any non-whitespace.

---

### **Flags**
Flags modify the behavior of regex functions:
- `re.IGNORECASE` or `re.I`: Makes the pattern case-insensitive.
- `re.MULTILINE` or `re.M`: Allows `^` and `$` to match the start and end of lines, respectively.
- `re.DOTALL` or `re.S`: Makes `.` match newline characters as well.

**Example with Flags**:
```python
result = re.search(r"hello", "Hello world", re.IGNORECASE)
print(result)  # <re.Match object; span=(0, 5), match='Hello'>
```

---
