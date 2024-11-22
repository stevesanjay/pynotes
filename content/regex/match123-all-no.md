---
title: Match123-All-No
date: 2024-11-22
author: Your Name
cell_count: 6
score: 5
---

```python
#  Match All Numbers in a File
```


```python
import re
```


```python
def extract_numbers(filename):
    with open(filename, 'r') as file:
        content = file.read()
        numbers = re.findall(r'\b\d+(\.\d+)?\b', content)
        return numbers
```


```python
# Example usage
filename = 'sample.txt'
```


```python
numbers = extract_numbers(filename)
print("Numbers found:", numbers)
```

    Numbers found: ['', '', '', '', '', '']



```python

```


---
**Score: 5**
