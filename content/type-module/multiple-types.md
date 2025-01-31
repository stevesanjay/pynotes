---
title: Multiple-Types
date: 2025-01-31
author: Your Name
cell_count: 7
score: 5
---

```python
# 20250130
```


```python
# Using Union for Multiple Types
```


```python
from typing import Union
```


```python
def square_or_length(value: Union[int, str]) -> int:
    if isinstance(value, int):
        return value ** 2
    return len(value)
```


```python
square_or_length(4)
```




    16




```python
square_or_length("test")
```




    4




```python

```


---
**Score: 5**
