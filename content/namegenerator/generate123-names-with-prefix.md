---
title: Generate123-Names-With-Prefix
date: 2024-11-27
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Names with Specific Prefix and Save to File
```


```python
import namegenerator
```


```python
def generate_names_with_prefix(prefix, num_names, filename):
    names = [prefix + namegenerator.gen() for _ in range(num_names)]
    with open(filename, 'w') as file:
        for name in names:
            file.write(f"{name}\n")
    return f"Generated {num_names} names with prefix '{prefix}' and saved to {filename}"
```


```python
# Example usage
prefix = "user_"
num_names = 5
```


```python
filename = 'generated_names_with_prefix.txt'
print(generate_names_with_prefix(prefix, num_names, filename))
```

    Generated 5 names with prefix 'user_' and saved to generated_names_with_prefix.txt



```python

```


---
**Score: 5**
