A `while` loop in Python repeatedly executes a block of code as long as a specified condition is true. The syntax for a `while` loop is:

```python
while condition:
    # Code to execute
```

### 1. **Basic `while` loop**
The loop continues to run as long as the condition evaluates to `True`. If the condition is `False`, the loop stops.

```python
# Basic while loop
count = 0
while count < 3:
    print(count)
    count += 1
```

### Output:
```
0
1
2
```

In this example, the condition `count < 3` is checked at the beginning of each loop iteration. The loop will run until `count` becomes `3`.

### 2. **Infinite `while` loop**
A `while` loop can run indefinitely if the condition always evaluates to `True`. This is known as an infinite loop, and you can stop it with a `break` statement or manually.

```python
# Infinite while loop
while True:
    print("This will print forever until you break!")
    break  # Breaks the loop after one iteration
```

### Output:
```
This will print forever until you break!
```

### 3. **Using `else` with a `while` loop**
The `else` block is executed when the loop finishes its execution without hitting a `break` statement.

```python
# Using while with else
count = 0
while count < 3:
    print(count)
    count += 1
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

### 4. **Using `break` to exit the loop early**
The `break` statement can be used to exit the loop before the condition becomes `False`.

```python
# Using break inside a while loop
count = 0
while count < 5:
    if count == 3:
        break  # Exit the loop when count is 3
    print(count)
    count += 1
```

### Output:
```
0
1
2
```

### 5. **Using `continue` to skip an iteration**
The `continue` statement is used to skip the rest of the code inside the loop for the current iteration and jump to the next iteration.

```python
# Using continue inside a while loop
count = 0
while count < 5:
    count += 1
    if count == 3:
        continue  # Skip printing when count is 3
    print(count)
```

### Output:
```
1
2
4
5
```

In this case, the number `3` is skipped because of the `continue` statement.
