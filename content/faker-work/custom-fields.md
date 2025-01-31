---
title: Custom-Fields
date: 2025-01-30
author: Your Name
cell_count: 10
score: 10
---

```python
# Generate Fake Data for Custom Fields
# Generate structured fake data for applications like user testing or mock APIs.
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
# Generate a structured fake user record
```


```python
user_data = {
    'id': fake.uuid4(),
    'name': fake.name(),
    'email': fake.email(),
    'phone': fake.phone_number(),
    'birthdate': fake.date_of_birth(minimum_age=18, maximum_age=65),
    'address': fake.address(),
}
```


```python
user_data
```




    {'id': '50d6d27a-423a-4589-9062-ab2f860c0a9b',
     'name': 'James Beard MD',
     'email': 'lsanders@example.com',
     'phone': '001-904-757-9199x8878',
     'birthdate': datetime.date(2004, 5, 5),
     'address': '097 Robinson Branch Apt. 464\nCobbberg, PA 47813'}




```python
user_data
```




    {'id': '50d6d27a-423a-4589-9062-ab2f860c0a9b',
     'name': 'James Beard MD',
     'email': 'lsanders@example.com',
     'phone': '001-904-757-9199x8878',
     'birthdate': datetime.date(2004, 5, 5),
     'address': '097 Robinson Branch Apt. 464\nCobbberg, PA 47813'}




```python

```


---
**Score: 10**
