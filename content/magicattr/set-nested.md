---
title: Set-Nested
date: 2024-12-05
author: Your Name
cell_count: 7
score: 5
---

```python
from magicattr import set
```


```python
class Theme:
    def __init__(self, color):
        self.color = color
```


```python
class Config:
    def __init__(self):
        self.theme = Theme("blue")
```


```python
config = Config()
```


```python
set(config, "theme.color", "red")
```


```python
print(config.theme.color) 
```

    red



```python

```


---
**Score: 5**
