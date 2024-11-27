---
title: Func-Kwargs
date: 2024-11-27
author: Your Name
cell_count: 5
score: 5
---

```python
def display_info(name,value):
    c = name 
    full_name = c + value
    return full_name
    # for key,value in name.items():
    #     print(f"{key}: {value}")
```


```python
display_info("steve", "sanjay")
```




    'stevesanjay'




```python
def display_info(**kwargs):
    for key,value in kwargs.items():
        print(f"{key}: {value}")
```


```python
display_info(name='steve', age=21, city="coimbatore", fullname="stevesanjay")
```

    name: steve
    age: 21
    city: coimbatore
    fullname: stevesanjay



```python

```


---
**Score: 5**
