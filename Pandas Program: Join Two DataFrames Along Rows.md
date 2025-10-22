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
```py
# Step 1: Import Libraries
import pandas as pd

# Step 2: Create First DataFrame
student_data1 = {
    'name': ['Anita', 'Bala'],
    'score': [85, 90],
    'attempts': [1, 2]
}
df1 = pd.DataFrame(student_data1)

# Step 3: Create Second DataFrame
student_data2 = {
    'name': ['Chitra', 'Dinesh'],
    'score': [78, 88],
    'attempts': [3, 1]
}
df2 = pd.DataFrame(student_data2)

# Step 4: Concatenate DataFrames row-wise
combined_df = pd.concat([df1, df2], axis=0)

# Step 5: Display Result
print("Combined Student Data:\n", combined_df)
```

## Output
<img width="567" height="189" alt="Screenshot 2025-10-22 224346" src="https://github.com/user-attachments/assets/41e2112c-1c0c-4a1a-85f6-5c8cf8912a52" />

## Result
successfully **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

