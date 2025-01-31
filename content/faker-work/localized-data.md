---
title: Localized-Data
date: 2025-01-30
author: Your Name
cell_count: 13
score: 10
---

```python
# Localized Fake Data
```


```python
# import necessary library
```


```python
from faker import Faker
```


```python
# Create Faker instance for French locale
```


```python
fake = Faker('fr_FR')

```


```python
# Generate localized fake data
```


```python
name = fake.name()
```


```python
name
```




    'Émilie Ferrand'




```python
address = fake.address()
```


```python
address
```




    '6, chemin Louis Lenoir\n74808 Besson'




```python
phone_number = fake.phone_number()
```


```python
phone_number
```




    '0384958153'




```python

```


---
**Score: 10**
