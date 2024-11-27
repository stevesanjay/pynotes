---
title: Kwargs-Basics
date: 2024-11-27
author: Your Name
cell_count: 5
score: 5
---

```python
 # reading data by using the kwargs
```


```python
def greet(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")
```


```python
def main_fun():
    greet(name="Alice", age=25, city="New York")
```


```python
# Example usage
main_fun()
```

    name: Alice
    age: 25
    city: New York



```python

```


---
**Score: 5**
