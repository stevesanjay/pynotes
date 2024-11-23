---
title: Generate65-Names-To-Csv
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Names and Save to CSV File

```


```python
import namegenerator
import csv
```


```python
def generate_names_to_csv(num_names, filename):
    names = [namegenerator.gen() for _ in range(num_names)]
    with open(filename, mode='w', newline='') as file:
        writer = csv.writer(file)
        writer.writerow(["Generated Names"])
        for name in names:
            writer.writerow([name])
    return f"Generated {num_names} names and saved to {filename}"
```


```python
num_names = 5
```


```python
filename = 'generated_names.csv'
print(generate_names_to_csv(num_names, filename))
```

    Generated 5 names and saved to generated_names.csv



```python

```


---
**Score: 5**
