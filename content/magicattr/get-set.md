---
title: Get-Set
date: 2024-11-23
author: Your Name
cell_count: 9
score: 5
---

```python
# Combine Get and Set for Dynamic Operations
```


```python
from magicattr import get, set

```


```python
class Values:
    def __init__(self, count):
        self.count = count
```


```python
class Data:
    def __init__(self):
        self.values = Values(5)
```


```python
data = Data()
```


```python
current_count = get(data, "values.count")
set(data, "values.count", current_count * 2)
```


```python
print(data.values.count)
```

    10



```python

```


```python

```


---
**Score: 5**
