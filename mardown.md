## Python Cheatsheet

---

| Table Of Contents | Description |
| ------------------ | ----------- |
| [Array](#array) | Array creation and operations |
| [List](#list) | List basics and operations |
| [String](#string) | String handling and methods |
| [Dictionary](#dictionary) | Key-value data structure |

---

## Array

- An **array** is a data structure that stores elements of the same type in contiguous memory.  
- Python’s built-in `list` can act like a dynamic array, but you can also use the `array` module for type-restricted arrays.

### Example: Creating an Array

``` python
import array

# Create an array of signed integers ('i')
my_array = array.array('i', [1, 2, 3, 4, 5])

print(my_array)        # Output: array('i', [1, 2, 3, 4, 5])
print(my_array[0])     # Access first element
```

### Common Array Operations

``` python
my_array.append(6)       # Add an element
my_array.remove(2)       # Remove an element
my_array.pop()           # Remove last element
my_array.insert(1, 9)    # Insert at index 1
print(my_array.tolist()) # Convert to Python list
```
---

## List

- A **list** is a collection of ordered, mutable (changeable) items that can contain mixed data types.

### Example: Creating a List

``` python
fruits = ['apple', 'banana', 'cherry']
numbers = [1, 2, 3, 4]
mixed = [1, 'hello', 3.14, True]
```

### Accessing and Modifying Lists

``` python
print(fruits[0])       # Access first element
fruits[1] = 'mango'    # Modify an element
print(fruits[-1])      # Access last element
```

### Common List Methods

``` python
fruits.append('grape')     # Add an item
fruits.remove('apple')     # Remove an item
fruits.pop()               # Remove last item
fruits.insert(1, 'kiwi')   # Insert item at position
fruits.sort()              # Sort list
fruits.reverse()           # Reverse order
print(len(fruits))         # Length of list
```

### List Comprehension

``` python
squares = [x**2 for x in range(5)]
print(squares)   # Output: [0, 1, 4, 9, 16]
``` 
---

## String

- A ***string*** is a sequence of Unicode characters.
- Strings are immutable — meaning they cannot be changed after creation.

### Creating and Accessing Strings

``` python
text = "Hello, World!"
print(text[0])        # 'H'
print(text[-1])       # '!'
print(text[0:5])      # 'Hello'
```

### Common String Methods

``` python
text = "  Python Programming  "

print(text.lower())      # '  python programming  '
print(text.upper())      # '  PYTHON PROGRAMMING  '
print(text.strip())      # Remove whitespace
print(text.replace("Python", "Java"))  # Replace word
print(text.split())      # Split into list
print(" ".join(['I', 'love', 'Python'])) # Join list to string
```

### String Formatting

``` python
name = "Alice"
age = 25

print(f"My name is {name} and I am {age} years old.")  # f-string
print("My name is {} and I am {} years old.".format(name, age))
```
---

## Dictionary

- A ***dictionary*** stores data in key-value pairs.
- Keys must be unique and immutable, while values can be of any data type.

### Creating Dictionary

``` python
person = {
    'name': 'John',
    'age': 30,
    'city': 'New York'
}
```

### Accessing and Modifying

``` python
print(person['name'])         # Access value
person['age'] = 31            # Update value
person['email'] = 'john@example.com'  # Add new key
```

### Common Dictionary 

``` python
print(person.keys())      # Get all keys
print(person.values())    # Get all values
print(person.items())     # Get key-value pairs
person.pop('city')        # Remove a key
person.update({'age': 32, 'country': 'USA'})  # Update multiple
```

### Dictionary Comprehension

``` python
squares = {x: x**2 for x in range(5)}
print(squares)   # Output: {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
```

---