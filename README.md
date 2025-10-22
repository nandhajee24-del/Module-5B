Nandha A(25017364)


# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

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
```py
# Step 1: Import NumPy
import numpy as np

# Step 2: Define arrays
x = np.array([10, 20, 30, 40])
y = np.array([15, 20, 25, 35])

# Step 3: Boolean indexing
greater_than = x > y
equal_to = x == y

# Step 4: Find indices where x >= y
indices = np.where(x >= y)

# Step 5: Print results
print("x:", x)
print("y:", y)
print("x > y:", greater_than)
print("x == y:", equal_to)
print("Indices where x >= y:", indices[0])
```


## Output
<img width="463" height="167" alt="Screenshot 2025-10-22 223354" src="https://github.com/user-attachments/assets/aa3cbc4d-94c5-47fc-be5e-1a02184e8d72" />

## Result
successfully Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

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
```py
# Step 1: Import NumPy
import numpy as np

# Step 2: Get input - define a sample 2D array
array = np.array([[12, 5, 7],
                  [3, 8, 1],
                  [9, 6, 4]])

# Step 3: Sort column-wise
sorted_array = np.sort(array, axis=0)

# Step 4 & 5: Display original and sorted arrays
print("Original Array:\n", array)
print("Column-wise Sorted Array:\n", sorted_array)
```


## Output
<img width="335" height="256" alt="Screenshot 2025-10-22 222733" src="https://github.com/user-attachments/assets/f7a9cfda-2753-4e1b-a03b-c8cded1803f3" />

## Result
successfully **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.
 

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
```py
# Step 1: Import NumPy
import numpy as np

# Step 2: Define a 2D array and a new column
original_array = np.array([[1, 2, 3],
                           [4, 5, 6],
                           [7, 8, 9]])

new_column = np.array([10, 11, 12])

# Step 3: Delete the second column (index 1)
array_without_column = np.delete(original_array, 1, axis=1)

# Step 4: Insert the new column at index 1
updated_array = np.insert(array_without_column, 1, new_column, axis=1)

# Step 5: Display the result
print("Original Array:\n", original_array)
print("Updated Array:\n", updated_array)
```

## Output
<img width="284" height="270" alt="Screenshot 2025-10-22 223857" src="https://github.com/user-attachments/assets/0a05811d-449a-4348-9638-05ed75c9fae9" />

## Result
successfully  **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

# Pandas Program: Create and Display a DataFrame with Custom Index Labels

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
```py
# Step 1: Import Libraries
import pandas as pd
import numpy as np

# Step 2: Create Dictionary
exam_data = {
    'name': ['Anita', 'Bala', 'Chitra', 'Dinesh'],
    'score': [88, 92, 79, 85],
    'attempts': [1, 2, 1, 3],
    'qualify': ['yes', 'yes', 'no', 'yes']
}

# Step 3: Index Labels
labels = ['a', 'b', 'c', 'd']

# Step 4: Create DataFrame
df = pd.DataFrame(exam_data, index=labels)

# Step 5: Display Output
print("Exam DataFrame:\n", df)
```

## Output
<img width="658" height="199" alt="Screenshot 2025-10-22 224158" src="https://github.com/user-attachments/assets/13391f55-446f-4a4a-80a6-13ff21f7968f" />

## Result
successfully **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

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
