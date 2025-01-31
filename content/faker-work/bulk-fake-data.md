---
title: Bulk-Fake-Data
date: 2025-01-31
author: Your Name
cell_count: 11
score: 10
---

```python
# Generate Fake Data in Bulk
```


```python
# import necessary library
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
# Generate 5 fake user profiles
```


```python
for _ in range(5):
    name = fake.name()
    email = fake.email()
    city = fake.city()
    print(f'Name: {name}, Email: {email}, City: {city}')
```

    Name: Haley Hall, Email: amberholland@example.org, City: Melindaport
    Name: Morgan Bryant, Email: bernard47@example.org, City: Sherifurt
    Name: Savannah Anderson, Email: prodriguez@example.org, City: New Logan
    Name: Jenny Lara, Email: friedmanmaxwell@example.net, City: Port Judithland
    Name: Cathy Hernandez, Email: pcraig@example.org, City: Moraview



```python
name
```




    'Cheryl Sharp MD'




```python
email
```




    'pcraig@example.org'




```python
city
```




    'Moraview'




```python

```


---
**Score: 10**
