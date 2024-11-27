---
title: Faker2Csv-Batch
date: 2024-11-27
author: Your Name
cell_count: 17
score: 15
---

```python
# Basic Enum Example
```


```python
# import necessary library
```


```python
from enum import Enum
```


```python
from faker import Faker
```


```python
import random
```


```python
import pandas as pd
```


```python
# Initialize Faker
```


```python
fake = Faker()
```


```python
# Define an Enum for job roles
```


```python
class JobRole(Enum):
    ENGINEER   = "Engineer"
    MANAGER    = "Manager"
    ANALYST    = "Analyst"
    CONSULTANT = "Consultant"
    DEVELOPER  = "Developer"
```


```python
# Function to generate random data
```


```python
def generate_data(num_records):
    data = []
    for _ in range(num_records):
        record = {
            "name": fake.name(),
            "email": fake.email(),
            "address": fake.address(),
            "job_role": random.choice(list(JobRole)).value,
            "company": fake.company(),
            "phone_number": fake.phone_number()
        }
        data.append(record)
    return data
```


```python
# Function to generate a batch of 5 records
```


```python
def generate_batch():
    batch = []
    for _ in range(5):
        record = {
            "name": fake.name(),
            "email": fake.email(),
            "address": fake.address(),
            "job_role": random.choice(list(JobRole)).value,
            "company": fake.company(),
            "phone_number": fake.phone_number()
        }
        batch.append(record)
    return batch
```


```python
def startpy():

    # Initialize an empty CSV file and write headers first
    csv_file_path_incremental = 'user1.csv'
    df = pd.DataFrame(generate_batch())  # Generate initial 5 rows for headers
    df.to_csv(csv_file_path_incremental, index=False, mode='w')  # Write headers with initial data

    # Generate remaining 995 rows in increments of 5 and append to CSV
    for _ in range(199):  # Remaining 199 batches of 5 rows each = 995 rows
        batch_data = generate_batch()
        batch_df = pd.DataFrame(batch_data)
        batch_df.to_csv(csv_file_path_incremental, index=False, mode='a', header=False)  # Append without headers
```


```python
startpy()
```


```python

```


---
**Score: 15**
