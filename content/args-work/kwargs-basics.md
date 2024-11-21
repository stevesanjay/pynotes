---
title: Kwargs-Basics
date: 2024-11-21
author: Your Name
cell_count: 3
score: 0
---

```python
def print_everything(*args):
        for count, thing in enumerate(args):
            print( '{0}. {1}'.format(count, thing))
```


```python
print_everything("steve","sanjay")
```

    0. steve
    1. sanjay



```python

```


---
**Score: 0**
