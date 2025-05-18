# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program

```
import numpy as np
arr=np.array(eval(input()))
print("Given array")
print(arr)
print()
print(np.sort(arr,axis=0))
```
## Output

![439196224-ad73f6e2-2acc-4156-8749-82281a1faf1c](https://github.com/user-attachments/assets/d3b4ad2f-8ae9-4384-b840-04fe701fc9da)

## Result

Thus the program that sorts the elements in each column of a given 2D array in ascending order is executed successfully.

# NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program

```
import numpy as np

x=np.array(eval(input()))
y=np.array(eval(input()))
gt=np.where(x>y)
eq=np.where(x==y)
print(gt)
print(eq)
```

## Output

![439325031-4c26dcc1-9990-4dd1-866f-dc1c6f347217](https://github.com/user-attachments/assets/bde095e8-aa58-4dbb-8dd4-7c3f601e10c6)

## Result

Thus the program that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y` is executed successfully.

# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```
import numpy as np

a=np.array(eval(input()))
b=np.array(eval(input()))
print("Printing Original array")
print(a)
print("Array after deleting column 2 on axis 1")
c=np.delete(a,1,axis=1)
print(c)
print("Array after inserting column 2 on axis 1")
print(np.insert(c,1,b,axis=1))
```

## Output

![439326579-56ee6af8-835c-4881-9f98-3188cd2ed32e](https://github.com/user-attachments/assets/ee721b51-27bb-4025-bcb0-c284e2b165e7)

## Result

Thus the program that deletes the second column from a given 2D array and inserts a new column at the same position is executed successfully.
