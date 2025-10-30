# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you select rows from a DataFrame where any value in the row exceeds a threshold?

```python
import pandas as pd

# Example DataFrame
df = pd.DataFrame({
    'A': [1, 2, 3],
    'B': [4, 3, 6],
    'C': [1, 8, 9]
})

threshold = 5

# Select rows where ANY value in the row exceeds the threshold
result = df[df.gt(threshold).any(axis=1)]
print(result)

```


### Question 2

Question: How do you sort a DataFrame by columns `A` and `B`?

```python

df = pd.DataFrame({'A': [3, 1, 2], 'B': [2, 3, 1], 'C': [1, 2, 3]})
result = df.sort_values(by=['A', 'B'],ascending=true)
print(result)

```

### Question 3

Question: How do you concatenate two DataFrames vertically?

```python
import pandas as pd

df1 = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})
df2 = pd.DataFrame({'A': [7, 8, 9], 'B': [10, 11, 12]})
```

Answer:

```python
result = pd.concat([df1, df2])
print(result)

```

### Question 4

Question: How do you compute the cumulative sum of a column in a DataFrame?

```python
import pandas as pd

df = pd.DataFrame({'A': [1, 2, 3, 4, 5]})
```

Answer:

```python
df = pd.DataFrame({'A': [1, 2, 3, 4, 5]})
result= df.cumsum()
print(result)
```

### Question 5

Question: How do you convert a Series of strings to uppercase?

```python
import pandas as pd

series = pd.Series(['apple', 'banana', 'cherry'])
```

Answer:

```python
result = series.str.upper()
print(result)
```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
