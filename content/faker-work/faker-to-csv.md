---
title: Faker-To-Csv
date: 2024-11-22
author: Your Name
cell_count: 7
score: 5
---

```python
import csv
```


```python
from faker import Faker
```


```python
fake = Faker()
```


```python
datas = []
```


```python
def generate_data():
    for i in range(1000):
        row = [
            i + 1,
            fake.name(),
            fake.email(),
            f"https://github.com/{fake.user_name()}",
            fake.city(),
            fake.country(),
            fake.state(),  
            
        ]
        datas.append(row)
    
    csv_file = 'fake_data.csv'

    with open(csv_file, mode='w') as file:
        writer = csv.writer(file)
        writer.writerow(['index','name','E mail' 'city', 'country', 'State', 'Github Link', 'phone_number'])
        writer.writerows(datas)

    print(f'1000 rows of fake data added to {csv_file}.')
```


```python
generate_data()

```

    1000 rows of fake data added to fake_data.csv.



```python

```


---
**Score: 5**
