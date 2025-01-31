---
title: Argsparse
date: 2025-01-30
author: Your Name
cell_count: 6
score: 5
---

```python
d = {"aa": 3, "bb": 4, "cc": 2, "dd": 1}
```


```python
d
```




    {'aa': 3, 'bb': 4, 'cc': 2, 'dd': 1}




```python
s = [(k, d[k]) for k in sorted(d, key=d.get, reverse=True)]
```


```python
s
```




    [('bb', 4), ('aa', 3), ('cc', 2), ('dd', 1)]




```python
for k, v in s:
    print(k, v)
```

    bb 4
    aa 3
    cc 2
    dd 1



```python

```


---
**Score: 5**
