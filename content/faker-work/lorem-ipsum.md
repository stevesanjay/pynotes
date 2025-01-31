---
title: Lorem-Ipsum
date: 2025-01-31
author: Your Name
cell_count: 8
score: 5
---

```python
# Import necessary modules
```


```python
from faker import Faker
```


```python
# Initialize Faker
```


```python
fake = Faker()
```


```python
# create a method to write a logic.
```


```python
def startpy():
    my_word_list = [
    'danish','cheesecake','sugar',
    'Lollipop','wafer','Gummies',
    'sesame','Jelly','beans',
    'pie','bar','Ice','oat' ]

    print(fake.sentence())
    # 'Expedita at beatae voluptatibus nulla omnis.'

    print(fake.sentence(ext_word_list=my_word_list))
```


```python
startpy()
```

    Provide vote expect that.
    Jelly oat Gummies sugar Jelly cheesecake.



```python

```


---
**Score: 5**
