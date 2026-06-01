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
