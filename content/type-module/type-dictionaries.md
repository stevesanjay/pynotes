---
title: Type-Dictionaries
date: 2025-01-30
author: Your Name
cell_count: 7
score: 5
---

```python
# 20250130
```


```python
# Type Hint for Dictionaries
```


```python
from typing import Dict
```


```python
def count_fruits(fruit_counts: Dict[str, int]) -> int:
    return sum(fruit_counts.values())
```


```python
fruits = {"apple": 5, "banana": 3, "orange": 2}
```


```python
count_fruits(fruits)
```




    10




```python

```


---
**Score: 5**
