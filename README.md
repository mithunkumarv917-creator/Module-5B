## Developed by: Mithun Kumar V (21225040236 / 25012629)

# 1.NumPy Program: Column-wise Sorting of a 2D Array

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

# 2.NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

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

x = np.array(eval(input()))
y = np.array(eval(input()))

ind = np.where(x>=y)
print("Indexs where value of array X is greater than or equal to Array y is:\n",ind)
```
## Output
<img width="745" height="121" alt="image" src="https://github.com/user-attachments/assets/537abeb1-ffdc-4769-89a6-80845336570a" />

## Result
Thus the program has been executed successfully.

# 3.NumPy Program: Replace the Second Column in a 2D Array

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

arr = np.array(eval(input()))
print("Enter the new column elements:")
new_col = list(map(int, input().split()))

arr = np.delete(arr, 1, axis=1)

arr = np.insert(arr, 1, new_col, axis=1)

print("Updated Array:")
print(arr)
```
## Output
<img width="386" height="216" alt="image" src="https://github.com/user-attachments/assets/315ee3f3-7237-4e80-879f-1d66d5d7a918" />

## Result
Thus the program has been executed successfully.

# 4.Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
import numpy as np

exam_data = {
    'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily'],
    'score': [12.5, 9, 16.5, np.nan, 9],
    'attempts': [1, 3, 2, 3, 2],
    'qualify': ['yes', 'no', 'yes', 'no', 'no']
}

labels = ['a', 'b', 'c', 'd', 'e']

df = pd.DataFrame(exam_data, index=labels)

print(df)
```
## Output
<img width="452" height="189" alt="image" src="https://github.com/user-attachments/assets/fbd0e3c2-3374-4cf7-9600-df74afbc9261" />

## Result
Thus the program has been executed successfully.

# 5.🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

```
import pandas as pd

student_data1 = {
    'Student_ID': [1, 2, 3],
    'Name': ['John', 'Alice', 'Bob'],
    'Marks': [85, 90, 78]
}

df1 = pd.DataFrame(student_data1)

student_data2 = {
    'Student_ID': [4, 5, 6],
    'Name': ['Emma', 'David', 'Sophia'],
    'Marks': [88, 76, 95]
}

df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0)

print(combined_df)
```
## Output
<img width="381" height="217" alt="image" src="https://github.com/user-attachments/assets/131f8cdf-9525-4e44-8149-ec75352d616f" />

## Result
Thus the program has been executed successfully.
