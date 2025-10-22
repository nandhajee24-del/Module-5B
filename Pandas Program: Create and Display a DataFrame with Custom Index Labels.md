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

