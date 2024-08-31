In Python, `is`, `not`, `in`, and `and` are fundamental operators and keywords used in various contexts to perform comparisons, logical operations, and membership tests. Let's break down each one with concrete examples:

### 1. `is`
The `is` operator checks if two variables refer to the same object in memory (i.e., they are identical objects). It is different from `==`, which checks if the values of two variables are equal.

**Example:**
```python
a = [1, 2, 3]
b = [1, 2, 3]
c = a

print(a is b)  # False, because a and b are different objects in memory
print(a is c)  # True, because c refers to the same object as a
```

### 2. `not`
The `not` keyword is a logical operator that negates the truth value of an expression. If the expression is `True`, `not` makes it `False`, and vice versa.

**Example:**
```python
x = True
y = False

print(not x)  # False
print(not y)  # True
```

### 3. `in`
The `in` operator checks if a value is present in a sequence (like a list, tuple, string, or dictionary). It returns `True` if the value is found, and `False` otherwise.

**Example:**
```python
my_list = [1, 2, 3, 4, 5]
print(3 in my_list)  # True, because 3 is in the list
print(6 in my_list)  # False, because 6 is not in the list

my_string = "hello"
print('e' in my_string)  # True, because 'e' is in the string
```

### 4. `and`
The `and` operator is a logical operator that returns `True` if both expressions on either side of it are `True`. If either expression is `False`, it returns `False`.

**Example:**
```python
a = 5
b = 10
c = 15

# Both conditions must be True for the result to be True
print(a < b and b < c)  # True, because both conditions are True
print(a < b and b > c)  # False, because the second condition is False
```

### Combining Them
These operators can be combined to form more complex expressions. For example:

**Example:**
```python
# Check if a variable is not None and is in a list
value = 3
my_list = [1, 2, 3, 4, 5]

if value is not None and value in my_list:
    print("Value is in the list")
else:
    print("Value is either None or not in the list")
```

**Explanation:**
- `value is not None`: Ensures that `value` is not `None`.
- `value in my_list`: Checks if `value` exists in `my_list`.
- `and`: Combines both conditions, so the print statement executes only if both conditions are `True`.

This covers the basics of `is`, `not`, `in`, and `and` in Python. These are essential tools in Python programming for writing clear and concise code.