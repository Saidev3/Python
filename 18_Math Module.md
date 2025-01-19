The **`math`** module in Python provides mathematical functions and constants to perform complex mathematical operations, such as trigonometry, logarithms, factorials, and more.

---

### Importing the `math` Module
To use the `math` module, you need to import it first.

```python
import math
```

---

### Commonly Used Constants

| Constant     | Description             |
|--------------|-------------------------|
| `math.pi`    | The value of π (3.14159). |
| `math.e`     | The value of e (2.71828). |
| `math.tau`   | The value of τ (6.28318, which is 2π). |
| `math.inf`   | Represents infinity.     |
| `math.nan`   | Represents "Not a Number". |

```python
print(math.pi)   # Output: 3.141592653589793
print(math.e)    # Output: 2.718281828459045
print(math.inf)  # Output: inf
print(math.nan)  # Output: nan
```

---

### Basic Mathematical Functions

#### 1. Absolute Value
```python
print(math.fabs(-7.5))  # Output: 7.5
```

#### 2. Ceiling and Floor
```python
print(math.ceil(4.2))  # Output: 5 (smallest integer >= 4.2)
print(math.floor(4.7)) # Output: 4 (largest integer <= 4.7)
```

#### 3. Factorial
```python
print(math.factorial(5))  # Output: 120 (5! = 5 × 4 × 3 × 2 × 1)
```

#### 4. Square Root
```python
print(math.sqrt(16))  # Output: 4.0
```

#### 5. Power
```python
print(math.pow(2, 3))  # Output: 8.0 (2 raised to the power of 3)
```

#### 6. GCD (Greatest Common Divisor)
```python
print(math.gcd(24, 36))  # Output: 12
```

---

### Logarithmic Functions

#### 1. Natural Logarithm (base `e`)
```python
print(math.log(2.71828))  # Output: ~1.0
```

#### 2. Logarithm with a Custom Base
```python
print(math.log(100, 10))  # Output: 2.0 (log base 10 of 100)
```

#### 3. Logarithm Base 2 and Base 10
```python
print(math.log2(8))   # Output: 3.0
print(math.log10(100))  # Output: 2.0
```

---

### Trigonometric Functions

#### 1. Basic Trigonometric Functions
All angles are in radians.

| Function          | Description                         |
|-------------------|-------------------------------------|
| `math.sin(x)`     | Sine of `x` (radians).             |
| `math.cos(x)`     | Cosine of `x` (radians).           |
| `math.tan(x)`     | Tangent of `x` (radians).          |

```python
angle = math.pi / 6  # 30 degrees in radians
print(math.sin(angle))  # Output: 0.5
print(math.cos(angle))  # Output: 0.8660254037844386
print(math.tan(angle))  # Output: 0.5773502691896257
```

#### 2. Inverse Trigonometric Functions
| Function            | Description                          |
|---------------------|--------------------------------------|
| `math.asin(x)`      | Inverse sine (returns radians).      |
| `math.acos(x)`      | Inverse cosine (returns radians).    |
| `math.atan(x)`      | Inverse tangent (returns radians).   |

```python
print(math.asin(0.5))  # Output: ~0.5235987755982988 (30 degrees in radians)
print(math.acos(0.5))  # Output: ~1.0471975511965976 (60 degrees in radians)
```

#### 3. Converting Between Degrees and Radians
```python
# Degrees to radians
print(math.radians(180))  # Output: 3.141592653589793

# Radians to degrees
print(math.degrees(math.pi))  # Output: 180.0
```

---

### Hyperbolic Functions
| Function           | Description                          |
|--------------------|--------------------------------------|
| `math.sinh(x)`     | Hyperbolic sine of `x`.             |
| `math.cosh(x)`     | Hyperbolic cosine of `x`.           |
| `math.tanh(x)`     | Hyperbolic tangent of `x`.          |

```python
print(math.sinh(1))  # Output: ~1.1752011936438014
print(math.cosh(1))  # Output: ~1.5430806348152437
print(math.tanh(1))  # Output: ~0.7615941559557649
```

---

### Rounding and Precision

#### 1. Truncate a Decimal
```python
print(math.trunc(4.8))  # Output: 4 (removes the decimal part)
```

#### 2. Rounding to Nearest Integer
```python
print(round(4.5))  # Output: 4 (rounds to nearest even number)
```

---

### Special Functions

#### 1. `math.isfinite(x)`
Checks if `x` is a finite number.

```python
print(math.isfinite(100))  # Output: True
print(math.isfinite(math.inf))  # Output: False
```

#### 2. `math.isnan(x)`
Checks if `x` is NaN (Not a Number).

```python
print(math.isnan(math.nan))  # Output: True
```

#### 3. `math.isinf(x)`
Checks if `x` is infinite.

```python
print(math.isinf(math.inf))  # Output: True
```

---

### Examples

#### 1. Calculate the Area of a Circle
```python
def circle_area(radius):
    return math.pi * math.pow(radius, 2)

print(circle_area(5))  # Output: 78.53981633974483
```

#### 2. Compound Interest Formula
```python
def compound_interest(principal, rate, time):
    return principal * math.pow(1 + rate / 100, time)

print(compound_interest(1000, 5, 2))  # Output: 1102.5
```

---

### Summary of `math` Module Functions

| Function          | Description                              |
|-------------------|------------------------------------------|
| `math.sqrt(x)`    | Returns the square root of `x`.          |
| `math.pow(x, y)`  | Returns `x` raised to the power `y`.     |
| `math.factorial(x)`| Returns the factorial of `x`.           |
| `math.log(x)`     | Returns the natural logarithm of `x`.    |
| `math.sin(x)`     | Returns the sine of `x` (in radians).    |
| `math.radians(x)` | Converts degrees to radians.            |
| `math.degrees(x)` | Converts radians to degrees.            |
