# `print()` Function

## Basic Usage

The `print()` function is used to output text or variables to the console.

```python
print("Hello, World!")
```

## Key Features

**1. Multiple Arguments**

Separate multiple items with commas

```python
print("Hello", "World")  # Output: Hello World
```

**2. End Parameter**

Change the ending character (default is newline `\n`)

```python
print("Hello", end="!")  # Output: Hello!
```

**3. Sep Parameter**

Specify a separator between multiple arguments

```python
print("Apple", "Banana", "Cherry", sep=" | ")  # Output: Apple | Banana | Cherry
```

**4. File Parameter**

Redirect output to a file

```python
with open("output.txt", "w") as f:
    print("Hello, File!", file=f)
```

**5. Formatting**

Use with string formatting methods

```python
name = "Alice"
age = 30
print(f"{name} is {age} years old")  # Output: Alice is 30 years old
```

## Common Uses

- Debugging: Print variable values or status messages
- User interaction: Display prompts or results
- Data visualization: Simple text-based output of data

**Note**

In Python 2, print was a statement. In Python 3, it's a function and requires parentheses.