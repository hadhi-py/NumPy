# NumPy Arrays

### How to create NumPy Arrays?

- By transforming a standard Python list
- Built-in functions
- Generating random data

### Importing NumPy

We need to import NumPy before use. For that:

```python
import numpy as np
```

We conventionally import NumPy with name ***_np_***.

## Creating NumPy Array: By transforming a standard Python list

We can pass a list into NumPy which returns a NumPy array.
```python
np.array(list_name)
```
We can store it into a new variable which will have the datatype as _numpy.ndarray._

We can create a multi-dimensional matrix. By creating a nested list and passing it.

For example:
```python
mylist = [[1,2,3],[4,5,6],[7,8,9]]
my_matrix = np.array(my_list)
```
## Creating NumPy Array: Built-in functions

```python
np.arange(start,stop,step)
```

This will create an NumPy array with elements starting from ***start*** to ***stop***, but not including ***stop*** with a step/jump size of ***step***.

</br>

### It will be often needed to create large arrays of zeros and ones
</br>

- ### Array of Zeros
```
np.zeros(shape)
```
Here, ***shape*** is the size of array to be formed. </br>
If the shape given is a number ***n***, it will return an one dimentional array of 'n' zeros. </br>

If the shape given is a tuple - *(rows,columns)*, then it will create a matrix with that number of rows and columns containing all zeros.

In default, the datatype of thus created array will be float. So all zeros will be represented by ***' 0. '***

We can change this datatype by changing the attribute, ***dtype*** of **np.zeros**. (By default its value will be float)

- ### Array of Ones
```
np.ones(shape)
```
Here, ***shape*** is the size of array to be formed. </br>
If the shape given is a number ***n***, it will return an one dimentional array of 'n' ones. </br>

If the shape given is a tuple - *(rows,columns)*, then it will create a matrix with that number of rows and columns containing all ones.

In default, the datatype of thus created array will be float. So all ones will be represented by ***' 1. '***

We can change this datatype by changing the attribute, ***dtype*** of **np.ones**. (By default its value will be float)

## linspace
