---
title: Custom-Aliases
date: 2025-01-31
author: Your Name
cell_count: 7
score: 5
---

```python
# 20250130
```


```python
# Custom Type Aliases
```


```python
from typing import List
```


```python
Vector = List[float]
```


```python
def dot_product(vec1: Vector, vec2: Vector) -> float:
    return sum(x * y for x, y in zip(vec1, vec2))
```


```python
dot_product([1.0, 2.0], [3.0, 4.0])
```




    11.0




```python

```


---
**Score: 5**
