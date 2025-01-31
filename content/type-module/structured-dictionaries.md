---
title: Structured-Dictionaries
date: 2025-01-31
author: Your Name
cell_count: 8
score: 5
---

```python
# 20250130
```


```python
# Using TypedDict for Structured Dictionaries
```


```python
from typing import TypedDict
```


```python
class User(TypedDict):
    name: str
    age: int
    email: str
```


```python
def display_user(user: User) -> str:
    return f"{user['name']} ({user['age']}) can be reached at {user['email']}."
```


```python
user = {"name": "Alice", "age": 30, "email": "alice@example.com"}
```


```python
display_user(user)
```




    'Alice (30) can be reached at alice@example.com.'




```python

```


---
**Score: 5**
