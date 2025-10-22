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

