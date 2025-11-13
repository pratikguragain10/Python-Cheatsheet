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

An **array** is a data structure that stores elements of the same type in contiguous memory.  
Python’s built-in `list` can act like a dynamic array, but you can also use the `array` module for type-restricted arrays.

### Example: Creating an Array

```python
import array

# Create an array of signed integers ('i')
my_array = array.array('i', [1, 2, 3, 4, 5])

print(my_array)        # Output: array('i', [1, 2, 3, 4, 5])
print(my_array[0])     # Access first element
```