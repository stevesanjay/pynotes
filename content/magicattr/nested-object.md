---
title: Nested-Object
date: 2024-11-22
author: Your Name
cell_count: 9
score: 5
---

```python
# Get Nested Attributes in a Deeply Nested Object
```


```python
from magicattr import get

```


```python
class Inner:
    def __init__(self, value):
        self.value = value
```


```python
class Outer:
    def __init__(self, inner):
        self.inner = inner
```


```python
inner = Inner("Hello")
```


```python
outer = Outer(inner)
```


```python
# Access deeply nested attribute
value = get(outer, "inner.value")
```


```python
value
```




    'Hello'




```python

```


---
**Score: 5**
