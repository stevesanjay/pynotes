---
title: Literal-Pecific-Values
date: 2025-01-30
author: Your Name
cell_count: 8
score: 5
---

```python
# 20250130
```


```python
# Using Literal for Specific Values
```


```python
from typing import Literal
```


```python
def choose_plan(plan: Literal["free", "premium", "enterprise"]) -> str:
    return f"You selected the {plan} plan."
```


```python
choose_plan("premium")
```




    'You selected the premium plan.'




```python
choose_plan("free")
```




    'You selected the free plan.'




```python
choose_plan("enterprise")
```




    'You selected the enterprise plan.'




```python

```


---
**Score: 5**
