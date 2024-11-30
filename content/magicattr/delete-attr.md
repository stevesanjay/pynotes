---
title: Delete-Attr
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
# Delete an Attribute Using magicattr
```


```python
from magicattr import delete

```


```python
class Profile:
    def __init__(self, username, email):
        self.username = username
        self.email = email
```


```python
profile = Profile("user123", "user@example.com")
```


```python
delete(profile, "email")
```


```python
print(hasattr(profile, "email"))
```

    False



```python

```


---
**Score: 5**
