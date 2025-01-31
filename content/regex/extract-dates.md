---
title: Extract-Dates
date: 2025-01-30
author: Your Name
cell_count: 7
score: 5
---

```python
# Extract Dates in DD/MM/YYYY Format
```


```python
import re
```


```python
def extract_dates(filename):
    with open(filename, 'r') as file:
        content = file.read()
        dates = re.findall(r'\b\d{2}/\d{2}/\d{4}\b', content)
        return dates

```


```python
filename = 'sample.txt'
```


```python
dates = extract_dates(filename)
```


```python
dates
```




    ['12/05/2024', '25/12/2024']




```python

```


---
**Score: 5**
