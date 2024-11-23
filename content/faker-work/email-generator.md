---
title: Email-Generator
date: 2024-11-23
author: Your Name
cell_count: 13
score: 10
---

```python
# json generator
```


```python
# Import necessary modules
```


```python
import pandas as pd
```


```python
from faker import Faker
```


```python
import random
```


```python
# Initialize Faker
```


```python
fake = Faker()
```


```python
# create a method write a logic
```


```python
def get_random_emails(max = 10):

    item_count = random.randint(1, max)

    email_list = []

    for _ in range(item_count):
        email_list.append(fake.email())

    return email_list
```


```python
def create_dataframe():

    email_list = [
        ",".join(get_random_emails()),
        ",".join(get_random_emails()),
        ",".join(get_random_emails()),
        ",".join(get_random_emails())
    ]

    # intialise data of lists.
    data = {
            'name':['Tom', 'nick', 'krish', 'jack'],
            'email':email_list
        }

    # Create DataFrame
    df = pd.DataFrame(data)

    # Print the output.
    print(df)

    df.to_csv('email.csv')
```


```python
def startpy():

    # print('Hey there')

    create_dataframe()
```


```python
startpy()
```

        name                                              email
    0    Tom  wraymond@example.org,onelson@example.org,mjone...
    1   nick  christinemartinez@example.net,ashleycole@examp...
    2  krish  barnesdawn@example.org,samuelmcdonald@example....
    3   jack                            danieljones@example.org



```python

```


---
**Score: 10**
