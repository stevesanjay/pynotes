---
title: Random-Name
date: 2025-01-30
author: Your Name
cell_count: 10
score: 10
---

```python
# random names
```


```python
# import necessary library
```


```python
from faker import Faker
```


```python
fake=Faker()
```


```python
# create a function to write the logic
```


```python
def generate_random_names():

    random_names = []
    for x in range(5) :
        random_names.append(fake.name())
    return  random_names  
```


```python
# create a another function to call the above method 
```


```python
def startpy():
    random_name_list = generate_random_names()   
    print(random_name_list)
```


```python
startpy()
```

    ['Robert Robinson', 'Michael Rivera', 'Daryl Munoz', 'Martha Mendez', 'Stephen Ross']



```python

```


---
**Score: 10**
