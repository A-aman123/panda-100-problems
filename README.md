# 100 Pandas Puzzles

Inspired by 100 Numpy exercises, here are 100 short puzzles for testing your knowledge of pandas' power.

Since pandas is a large library with many different specialist features and functions, these exercises focus mainly on the fundamentals of manipulating data (indexing, grouping, aggregating, cleaning), making use of the core DataFrame and Series objects.

## Getting Started

### Importing pandas
1. Import pandas under the alias pd.

   ```python
   import pandas as pd
   ```

2. Print the version of pandas that has been imported.

   ```python
   print(pd.__version__)
   ```

3. Print out all the version information of the libraries that are required by the pandas library.

   ```python
   pd.show_versions()
   ```

## DataFrame Basics

### A few of the fundamental routines for selecting, sorting, adding, and aggregating data in DataFrames

Consider the following Python dictionary data and Python list labels:

```python
data = {
    'animal': ['cat', 'cat', 'snake', 'dog', 'dog', 'cat', 'snake', 'cat', 'dog', 'dog'],
    'age': [2.5, 3, 0.5, np.nan, 5, 2, 4.5, np.nan, 7, 3],
    'visits': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
    'priority': ['yes', 'yes', 'no', 'yes', 'no', 'no', 'no', 'yes', 'no', 'no']
}

labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
```

4. Create a DataFrame `df` from this dictionary data which has the index labels.

   ```python
   import numpy as np

   df = pd.DataFrame(data, index=labels)
   ```

5. Display a summary of the basic information about this DataFrame and its data.

   ```python
   print(df.info())
   ```

---
