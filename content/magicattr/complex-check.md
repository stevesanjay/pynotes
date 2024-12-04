---
title: Complex-Check
date: 2024-12-05
author: Your Name
cell_count: 10
score: 10
---

```python
# Check Attribute in a Complex Structure
```


```python
!pip install magicattr
```

    Requirement already satisfied: magicattr in /usr/local/Caskroom/miniconda/base/envs/py312/lib/python3.12/site-packages (0.1.6)



```python
from magicattr import get

```


```python
class A:
    def __init__(self, value):
        self.value = value

```


```python
class B:
    def __init__(self, a):
        self.a = a
```


```python
b = B(A(42))
```


```python
def has(obj, attr_path):
    try:
        get(obj, attr_path)
        return True
    except AttributeError:
        return False
```


```python
exists = has(b, "a.value")
```


```python
exists
```




    True




```python

```


---
**Score: 10**
