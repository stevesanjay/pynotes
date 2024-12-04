---
title: Custom-Provider
date: 2024-12-05
author: Your Name
cell_count: 12
score: 10
---

```python
# Custom Provider
```


```python
# import necessary library
```


```python
from faker import Faker
```


```python
from faker.providers import BaseProvider
```


```python
# Custom provider class
```


```python
class MyProvider(BaseProvider):
    def programming_language(self):
        return self.random_element(['Python', 'JavaScript', 'Java', 'C++', 'Go'])

```


```python
# Initialize Faker
```


```python
fake = Faker()
```


```python
fake.add_provider(MyProvider)
```


```python
# Use the custom provider
```


```python
language = fake.programming_language()

```


```python
language
```




    'Java'




---
**Score: 10**
