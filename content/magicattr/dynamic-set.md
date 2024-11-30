---
title: Dynamic-Set
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
# Set Attributes Dynamically in a Class
```


```python
from magicattr import set
```


```python
class User:
    def __init__(self, name, age):
        self.name = name
        self.age = age
```


```python
user = User("Alice", 25)
```


```python
set(user, "name", "Bob")
```


```python
print(user.name) 
```

    Bob



```python

```


---
**Score: 5**
