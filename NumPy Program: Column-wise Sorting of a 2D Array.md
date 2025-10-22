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

<img width="335" height="256" alt="Screenshot 2025-10-22 222733" src="https://github.com/user-attachments/assets/d904753f-d896-49ef-ad2d-ecb715bbb8f3" />


## Result
successfully **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

