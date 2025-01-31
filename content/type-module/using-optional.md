---
title: Using-Optional
date: 2025-01-31
author: Your Name
cell_count: 7
score: 5
---

```python
# 20250130
```


```python
# Using Optional for Nullable Parameters
```


```python
from typing import Optional

```


```python
def greet(name: Optional[str] = None) -> str:
    if name:
        return f"Hello, {name}!"
    return "Hello, Guest!"
```


```python
greet()
```




    'Hello, Guest!'




```python
greet("Alice")
```




    'Hello, Alice!'




```python

```


---
**Score: 5**
