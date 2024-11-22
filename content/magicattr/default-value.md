---
title: Default-Value
date: 2024-11-22
author: Your Name
cell_count: 7
score: 5
---

```python
 # Default Value if Attribute Does Not Exist

```


```python
from magicattr import get
```


```python
class Example:
    def __init__(self):
        self.value = 42

```


```python
example = Example()
```


```python
result = get(example, "non_existent_attribute", default="Default Value")
```


```python
result
```




    'Default Value'




```python

```


---
**Score: 5**
