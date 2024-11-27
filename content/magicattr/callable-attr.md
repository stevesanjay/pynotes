---
title: Callable-Attr
date: 2024-11-27
author: Your Name
cell_count: 7
score: 5
---

```python
# Access a Callable Attribute
```


```python
from magicattr import get
```


```python
class Calculator:
    def add(self, x, y):
        return x + y


```


```python
calc = Calculator()
```


```python
# Access and call a method
add_method = get(calc, "add")
result = add_method(5, 3)

```


```python
print(result)
```

    8



```python

```


---
**Score: 5**
