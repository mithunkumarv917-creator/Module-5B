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

arr = np.array(eval(input()))
arr1 = np.sort(arr,axis=0)
print(f"Original 2D array:\n{arr}\nNew 2D Array after sorting\n{arr1}")
```
## Output
<img width="482" height="250" alt="image" src="https://github.com/user-attachments/assets/700cfe34-b1a9-44a5-8799-dd4781f7689d" />

## Result
Thus the program has been executed successfully.
