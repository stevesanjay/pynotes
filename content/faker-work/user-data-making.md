---
title: User-Data-Making
date: 2025-01-30
author: Your Name
cell_count: 15
score: 15
---

```python
#  user data making

```


```python
# Import necessary modules
```


```python
import pandas as pd
```


```python
import random
```


```python
from faker import Faker
```


```python
# Initialize Faker
```


```python
faker = Faker()
```


```python
# global variable 
COUNT = 1000
```


```python
# create a method to write the logic
```


```python
def generate_names(count, type):

    item_list = []
    for i in range(count):
        if(type == 'name'):
            c_item = faker.name()
        elif(type == 'address'):
            c_item = faker.address()

        # print(f'[{i}] : {c_item}')
        item_list.append(c_item)

    return item_list
```


```python
def generate_data():

    global faker

    username_list   = generate_names(COUNT, 'name')
    address_list    = generate_names(COUNT, 'address')

    data    = pd.DataFrame({
        'username' : username_list,
        'address' : address_list
    })

    return data
```


```python
file_name = "user-1m.csv"
```


```python
def startpy():

    data = generate_data()
    # print(data)
    
    data.to_csv(file_name)
```


```python
startpy()
```


```python

```


---
**Score: 15**
