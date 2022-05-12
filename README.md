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

- ## linspace

We can specify an interval, say between ***start*** and ***stop*** and a number, ***num*** and linspace returns evenly/equally spaced *num* numbers between the intervals *start* and *stop* (by default including them).

```
np.linspace(start,stop,num)
```
> </BR>**Example:**
> ```python
> np.linspace(1,100,50)
> ``` 
> </BR> Returns:
```
array([  1. ,   3.02040816,   5.04081633,   7.06122449, 9.08163265,  11.10204082,  13.12244898,  15.14285714,7.16326531,  19.18367347,  21.20408163,  23.2244898 , 25.24489796,  27.26530612,  29.28571429,  31.30612245, 33.32653061,  35.34693878,  37.36734694,  39.3877551 , 41.40816327,  43.42857143,  45.44897959,  47.46938776, 49.48979592,  51.51020408,  53.53061224,  55.55102041, 57.57142857,  59.59183673,  61.6122449 ,  63.63265306, 65.65306122,  67.67346939,  69.69387755,  71.71428571, 73.73469388,  75.75510204,  77.7755102 ,  79.79591837, 81.81632653,  83.83673469,  85.85714286,  87.87755102, 89.89795918,  91.91836735,  93.93877551,  95.95918367, 97.97959184, 100.])
```
which is the NumPy array containing 50 equally spaced numbers between 1 and 100 including them.

- ### Identity Matrix
  Idenity matrix of the size ***n*** can be created using

```python
np.eye(n)
```

## Useful attributes and methods

- reshape()
  
     We can reshape our NumPy array to any shape by specifying the matrix order.


```python
arr = np.arange(25)
arr.reshape(5,5)
```
returns :
```
array([[ 0,  1,  2,  3,  4],
       [ 5,  6,  7,  8,  9],
       [10, 11, 12, 13, 14],
       [15, 16, 17, 18, 19],
       [20, 21, 22, 23, 24]])
```
When reshaping, care must be given inorder to ensure the number of elements is equal to the size of the reshaped array.

- max() and min()

```python
arr.max()

arr.min
```

Returns maximum and minimum values in the NumPy array, **arr**.

- argmax() and argmin()
  
  ```python
  arr.argmax()
  arr.argmin()
  ```
Returns the **index postion** of the maximum and minimum value.

- shape()
  ```
  arr.shape()
  ```
  Returns the shape of the array which is the order of the matrix in the form of a tuple.
