---
title: Generate56-Unique-Names
date: 2024-11-27
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Unique Names and Save to File
```


```python
import namegenerator
```


```python
def generate_unique_names(num_names, filename):
    names = set()  # Using a set to ensure unique names
    while len(names) < num_names:
        names.add(namegenerator.gen())
    
    with open(filename, 'w') as file:
        for name in names:
            file.write(f"{name}\n")
    
    return f"Generated {num_names} unique names and saved to {filename}"
```


```python
num_names = 8
filename = 'unique_generated_names.txt'
```


```python
print(generate_unique_names(num_names, filename))
```

    Generated 8 unique names and saved to unique_generated_names.txt



```python

```


---
**Score: 5**
