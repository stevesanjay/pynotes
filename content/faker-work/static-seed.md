---
title: Static-Seed
date: 2024-12-05
author: Your Name
cell_count: 14
score: 10
---

```python
# Static Seed for Reproducibility
# Set a static seed to ensure the same fake data is generated every time.
```


```python
# import necessary library
```


```python
from faker import Faker
```


```python
# Initialize Faker with a seed
```


```python
fake = Faker()
```


```python
Faker.seed(12345)
```


```python
# Generate reproducible fake data
```


```python
print(fake.name())
```

    Adam Bryan



```python
print(fake.address())
```

    49625 Morgan Green Apt. 982
    Joannaland, NC 96890



```python
print(fake.email())
```

    krichards@example.org



```python
print(fake.city())
```

    Lake Christian



```python
print(fake.phone_number())
```

    350-875-0860x02924



```python
print(fake.uuid4())
```

    93fd7234-ae71-4399-a2b2-848b1b1bcf72



```python

```


---
**Score: 10**
