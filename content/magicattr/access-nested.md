---
title: Access-Nested
date: 2024-11-23
author: Your Name
cell_count: 9
score: 5
---

```python
# Access Nested Attributes
```


```python
from magicattr import get
```


```python
class Address:
    def __init__(self, city):
        self.city = city
```


```python
class Person:
    def __init__(self, name, address):
        self.name = name
        self.address = address
```


```python
address = Address("coimbatore")
```


```python
person  = Person("steve", address)
```


```python
city  = get(person, "address.city")
```


```python
city
```




    'coimbatore'




```python

```


---
**Score: 5**
