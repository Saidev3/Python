Here are a few examples demonstrating the use of the `re.search()` function from the `re` module. Each example shows a different use case for matching patterns.

---

### **1. Basic Search**
Search for the word "Python" in a string.
```python
import re

text = "I love Python programming."
pattern = r"Python"

result = re.search(pattern, text)
if result:
    print("Match found:", result.group())  # Output: Match found: Python
else:
    print("No match found")
```

---

### **2. Case-Insensitive Search**
Search for "python" regardless of case.
```python
text = "I love PYTHON programming."
pattern = r"python"

result = re.search(pattern, text, re.IGNORECASE)
if result:
    print("Match found:", result.group())  # Output: Match found: PYTHON
else:
    print("No match found")
```

---

### **3. Search for Digits**
Find the first sequence of digits in a string.
```python
text = "My phone number is 12345."
pattern = r"\d+"

result = re.search(pattern, text)
if result:
    print("Match found:", result.group())  # Output: Match found: 12345
else:
    print("No match found")
```

---

### **4. Match at Specific Position**
Search for a word that starts with "pro" and ends with "ing."
```python
text = "I am progressing in Python programming."
pattern = r"\bpro.*?ing\b"

result = re.search(pattern, text)
if result:
    print("Match found:", result.group())  # Output: Match found: progressing
else:
    print("No match found")
```

---

### **5. Using Meta-Characters**
Search for any character followed by "at."
```python
text = "The cat is on the mat."
pattern = r".at"

result = re.search(pattern, text)
if result:
    print("Match found:", result.group())  # Output: Match found: cat
else:
    print("No match found")
```

---

### **6. Validate Email Format**
Check if a string contains an email address.
```python
text = "Contact me at example@domain.com."
pattern = r"[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}"

result = re.search(pattern, text)
if result:
    print("Valid email found:", result.group())  # Output: Valid email found: example@domain.com
else:
    print("No email found")
```

---

### **7. Search for Words at the End of a String**
Search for "world" at the end of a string.
```python
text = "Hello world"
pattern = r"world$"

result = re.search(pattern, text)
if result:
    print("Match found:", result.group())  # Output: Match found: world
else:
    print("No match found")
```

---

### **8. Check if a String Contains Only Letters**
Verify if a string contains only alphabetic characters.
```python
text = "Python"
pattern = r"^[A-Za-z]+$"

result = re.search(pattern, text)
if result:
    print("Only letters:", result.group())  # Output: Only letters: Python
else:
    print("Contains non-letters")
```

---
