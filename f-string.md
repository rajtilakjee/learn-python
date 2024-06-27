# f-string

f-strings, introduced in Python 3.6, provide a concise and readable way to embed expressions inside string literals.

## Basic Syntax

```python
name = "Alice"
age = 30
print(f"My name is {name} and I'm {age} years old.")
```

## Key Features

**1. Expression Evaluation**

f-strings can contain Python expressions

```python
x = 10
y = 20
print(f"The sum of {x} and {y} is {x + y}")
```

**2. Function Calls**

Call functions within f-strings

```python
def greet(name):
    return f"Hello, {name}!"

print(f"{greet('Bob')}")  # Output: Hello, Bob!
```

**3. Object Methods**

Access object methods and attributes

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

person = Person("Charlie", 25)
print(f"{person.name} is {person.age} years old")
```

**4. Formatting Options**

Use format specifiers for precision and alignment

```python
pi = 3.14159
print(f"Pi to 2 decimal places: {pi:.2f}")
print(f"{'Left':<10}|{'Center':^10}|{'Right':>10}")
```

**5. Multiline f-strings**

Span multiple lines for readability

```python
name = "David"
age = 35
occupation = "engineer"

info = f"""
Name: {name}
Age: {age}
Job: {occupation}
"""
print(info)
```

**6. Self-Documenting Expressions (Python 3.8+)**

Include the expression and its value

```python
x = 42
print(f"{x=}")  # Output: x=42
```

## Advantages

- More readable than older .format() method or %-formatting
- Evaluated at runtime, allowing for dynamic string creation
- Often faster than other string formatting methods

**Note**

F-strings are only available in Python 3.6 and later versions
Use double braces {{}} to include literal curly braces in the output