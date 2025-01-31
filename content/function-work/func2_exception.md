---
title: Func2 Exception
date: 2025-01-31
author: Your Name
cell_count: 4
score: 0
---

```python
def divided_number(a, b):
    try:


        result = a/b
    except ZeroDivisionError:
        return "cannot divided by zero"
    return result

```


```python
a = int(input("enter a number :"))
b = int(input("enter a number :"))
```

    enter a number : 1
    enter a number : 4



```python
print(divided_number(a,b))
```

    0.25



```python

```


---
**Score: 0**
