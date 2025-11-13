## Python-Cheatsheet

-------------

| Table Of Contents | Lines |
| ----------- | ----------- |
| Array | Title |
| Dictionary | Text |
| List | Text |
| String | Text |


## Array

-------------

- An array is a data structure designed to store a collection of elements, typically of the same data type, in contiguous memory locations.
In Python, built-in lists works or functions like an dynamic arrays. While Python doen't have a built in 'array' type in the same sense as other languages, the list data structure serves a similar purpose and is frequently used as such.

- A true array structure, especially for efficient handling of numeric data, is provided by the array module and NumPy library in python.

1. The `array` module:

```Python
    " Sample of creation of array using import array"

    import array

    # Create an array of signed integers ('i')

    my_array = array.array('i', [1, 2, 3, 4, 5])

    print(my_array)
```