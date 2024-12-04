---
title: Glob Vari
date: 2024-12-05
author: Your Name
cell_count: 7
score: 5
---

```python
#global variable
x = 5
```


```python
x
```




    5




```python
def foo():
    #local variable 
    x= 10
    print("local x:", x)
```


```python
foo()
```

    local x: 10



```python
def fool():
    print("local x:", x)
```


```python
fool()
```

    local x: 5



```python

```


---
**Score: 5**
