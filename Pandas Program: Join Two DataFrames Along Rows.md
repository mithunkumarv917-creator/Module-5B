# 🧪 Pandas Program: Join Two DataFrames Along Rows

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
