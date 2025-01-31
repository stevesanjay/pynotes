---
title: Func3 Forloop
date: 2025-01-31
author: Your Name
cell_count: 5
score: 5
---

```python
def for_loop_1():

    # change elements of a list [23, 18, 2, 25, 12, 33], to 0 if the element exceeds 20.
    Elements = [23, 18, 2, 12, 33]
    for a in range(len(Elements)):
        # print (Elements[a])
        if Elements[a]>20:
            print (0)
        else:
            print (Elements[a])
```


```python
def for_loop_2():

    # change elements of a list [23, 18, 2, 25, 12, 33], to 0 if the element exceeds 20.
    Elements = [23, 18, 2, 12, 33]
    for element in Elements:
        # print (Elements[a])
        if element > 20:
            print (0)
        else:
            print (element)
            
```


```python
for_loop_1()
```

    0
    18
    2
    12
    0



```python
for_loop_2()
```

    0
    18
    2
    12
    0



```python

```


---
**Score: 5**
