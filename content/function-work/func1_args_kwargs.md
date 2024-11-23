---
title: Func1 Args Kwargs
date: 2024-11-23
author: Your Name
cell_count: 3
score: 0
---

```python
def print_value(*args,**kwargs):
    for args in args:
        print(f'args:{args}')

    for key in kwargs:
        print(f"{key}: {kwargs[key]}")
```


```python
print_value(1,2,3,4,5,6,7,8,"steve",name="sanjay",age=21)
```

    args:1
    args:2
    args:3
    args:4
    args:5
    args:6
    args:7
    args:8
    args:steve
    name: sanjay
    age: 21



```python

```


---
**Score: 0**
