---
title: Generate115-Unique-Names-Json
date: 2025-01-31
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Unique Names and Save to JSON
```


```python
import namegenerator
import json
```


```python
def generate_unique_names_json(num_names, filename):
    names = set()  # Ensure unique names
    while len(names) < num_names:
        names.add(namegenerator.gen())
    
    with open(filename, 'w') as file:
        json.dump(list(names), file)
    
    return f"Generated {num_names} unique names and saved to {filename}"

```


```python
num_names = 8
filename = 'unique_generated_names.json'
```


```python
print(generate_unique_names_json(num_names, filename))
```

    Generated 8 unique names and saved to unique_generated_names.json



```python

```


---
**Score: 5**
