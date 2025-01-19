File handling in Python allows you to work with files for tasks like reading, writing, and appending data. Python provides built-in functions to handle file operations.

---

### Opening a File
To open a file, use the **`open()`** function. It returns a file object.

```python
file = open("example.txt", "mode")
```

#### File Modes
| Mode   | Description                                     |
|--------|-------------------------------------------------|
| `'r'`  | Read mode (default). Opens the file for reading. |
| `'w'`  | Write mode. Creates a new file or overwrites if it exists. |
| `'x'`  | Exclusive creation. Fails if the file already exists. |
| `'a'`  | Append mode. Writes to the end of the file if it exists. |
| `'b'`  | Binary mode. Used for non-text files (e.g., images). |
| `'t'`  | Text mode (default). Used for text files.        |
| `'+'`  | Read and write mode.                            |

---

### Reading from a File
You can read the contents of a file using various methods.

#### 1. **`read()`**: Reads the entire file.
```python
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

#### 2. **`readline()`**: Reads one line at a time.
```python
with open("example.txt", "r") as file:
    line = file.readline()
    print(line)  # Output: First line of the file
```

#### 3. **`readlines()`**: Reads all lines into a list.
```python
with open("example.txt", "r") as file:
    lines = file.readlines()
    print(lines)  # Output: ['Line 1\n', 'Line 2\n']
```

---

### Writing to a File
You can write to a file using **`write()`** or **`writelines()`**.

#### 1. **`write()`**: Writes a string to the file.
```python
with open("example.txt", "w") as file:
    file.write("This is a new file.\n")
    file.write("Second line.")
```

#### 2. **`writelines()`**: Writes multiple lines from a list.
```python
with open("example.txt", "w") as file:
    lines = ["Line 1\n", "Line 2\n", "Line 3\n"]
    file.writelines(lines)
```

**Note**: When opening a file in `'w'` mode, its content is erased.

---

### Appending to a File
Use the **`a`** mode to append data without overwriting the file.

```python
with open("example.txt", "a") as file:
    file.write("\nThis is an appended line.")
```

---

### Closing a File
Always close the file after performing operations to free system resources. If you use `with`, the file is automatically closed.

```python
file = open("example.txt", "r")
content = file.read()
file.close()
```

---

### Working with Binary Files
For binary files (e.g., images, PDFs), use the `'b'` mode.

```python
# Writing binary data
with open("example.bin", "wb") as file:
    file.write(b"This is binary data.")

# Reading binary data
with open("example.bin", "rb") as file:
    content = file.read()
    print(content)  # Output: b'This is binary data.'
```

---

### File Pointer
The file pointer indicates the current position in the file. You can use the following methods to manage it:

#### 1. **`tell()`**: Returns the current position of the pointer.
```python
with open("example.txt", "r") as file:
    print(file.tell())  # Output: 0 (start of file)
    file.read(5)
    print(file.tell())  # Output: 5
```

#### 2. **`seek()`**: Moves the pointer to a specific position.
```python
with open("example.txt", "r") as file:
    file.seek(10)  # Move to the 10th byte
    print(file.read())  # Reads from the 10th byte onward
```

---

### Checking if a File Exists
Before performing file operations, you can check if a file exists using the **`os`** module or the **`pathlib`** module.

#### Using `os` Module
```python
import os

if os.path.exists("example.txt"):
    print("File exists.")
else:
    print("File does not exist.")
```

#### Using `pathlib` Module
```python
from pathlib import Path

file_path = Path("example.txt")
if file_path.is_file():
    print("File exists.")
else:
    print("File does not exist.")
```

---

### Exception Handling in File Operations
To handle file-related errors, use a `try-except` block.

```python
try:
    with open("nonexistent.txt", "r") as file:
        content = file.read()
except FileNotFoundError:
    print("File not found.")
except Exception as e:
    print(f"An error occurred: {e}")
```

---

### Deleting a File
You can delete a file using the **`os`** module.

```python
import os

if os.path.exists("example.txt"):
    os.remove("example.txt")
    print("File deleted.")
else:
    print("File does not exist.")
```

---

### Summary of File Methods

| Method       | Description                                       |
|--------------|---------------------------------------------------|
| `read(size)` | Reads up to `size` bytes or the entire file.      |
| `readline()` | Reads a single line from the file.                |
| `readlines()`| Reads all lines into a list.                      |
| `write(text)`| Writes a string to the file.                     |
| `writelines(lines)`| Writes a list of strings to the file.       |
| `tell()`     | Returns the current file pointer position.        |
| `seek(offset)`| Moves the file pointer to the specified position.|

---
