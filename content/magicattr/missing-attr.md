---
title: Missing-Attr
date: 2024-11-23
author: Your Name
cell_count: 7
score: 5
---

```python
# Handle Missing Attributes Gracefully
```


```python
from magicattr import get
```


```python
class System:
    pass
```


```python
system = System()
```


```python
value = get(system, "non_existent_attr", default="Not Found")
```


```python
value
```




    'Not Found'




```python

```


---
**Score: 5**
