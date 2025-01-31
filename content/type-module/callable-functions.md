---
title: Callable-Functions
date: 2025-01-31
author: Your Name
cell_count: 7
score: 5
---

```python
# 20250130
```


```python
# Using Callable for Functions
```


```python
from typing import Callable
```


```python
def apply_operation(a: int, b: int, operation: Callable[[int, int], int]) -> int:
    return operation(a, b)
```


```python
result = apply_operation(2, 3, lambda x, y: x + y)
```


```python
result
```




    5




```python

```


---
**Score: 5**
