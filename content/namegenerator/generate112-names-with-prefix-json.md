---
title: Generate112-Names-With-Prefix-Json
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Names with Prefix and Save to JSON

```


```python
import namegenerator
import json
```


```python
def generate_names_with_prefix_json(prefix, num_names, filename):
    names = [prefix + namegenerator.gen() for _ in range(num_names)]
    with open(filename, 'w') as file:
        json.dump(names, file)
    return f"Generated {num_names} names with prefix '{prefix}' and saved to {filename}"

```


```python
prefix = "guest_"
num_names = 6
```


```python
filename = 'generated_names_with_prefix.json'
print(generate_names_with_prefix_json(prefix, num_names, filename))
```

    Generated 6 names with prefix 'guest_' and saved to generated_names_with_prefix.json



```python

```


---
**Score: 5**
