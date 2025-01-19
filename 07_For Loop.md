In Python, a `for` loop is used to iterate over a sequence (like a list, tuple, string, or range) and execute a block of code multiple times.

### 1. **Basic `for` loop** with a sequence
You can loop through a sequence like a list or a string and execute the code inside the loop for each item.

```python
# Looping through a list
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    print(fruit)
```

### Output:
```
apple
banana
cherry
```

### 2. **Using `range()` for iteration**
The `range()` function generates a sequence of numbers, which is commonly used in `for` loops when you need to repeat a block of code a certain number of times.

```python
# Looping through a range of numbers
for i in range(5):
    print(i)
```

### Output:
```
0
1
2
3
4
```

- The `range(5)` generates numbers from `0` to `4` (5 is not included).

### 3. **Looping through a string**
You can also loop through the characters in a string.

```python
# Looping through a string
word = "hello"
for letter in word:
    print(letter)
```

### Output:
```
h
e
l
l
o
```

### 4. **Using `for` loop with `else`**
The `else` part of the loop is executed when the loop completes without hitting a `break` statement.

```python
# Using for loop with else
for i in range(3):
    print(i)
else:
    print("Loop finished")
```

### Output:
```
0
1
2
Loop finished
```

### Example with `break`:
If the loop hits a `break` statement, it exits the loop and skips the `else` block.

```python
# Using break to exit the loop early
for i in range(5):
    if i == 3:
        break
    print(i)
else:
    print("Loop finished")  # This will not be printed
```

### Output:
```
0
1
2
```
