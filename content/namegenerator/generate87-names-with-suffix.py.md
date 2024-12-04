---
title: Generate87-Names-With-Suffix.Py
date: 2024-12-05
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Names with Suffix and Save to File
```


```python
import namegenerator
```


```python
def generate_names_with_suffix(suffix, num_names, filename):
    names = [namegenerator.gen() + suffix for _ in range(num_names)]
    with open(filename, 'w') as file:
        for name in names:
            file.write(f"{name}\n")
    return f"Generated {num_names} names with suffix '{suffix}' and saved to {filename}"

```


```python
# Example usage
suffix = "_xyz"
num_names = 7
```


```python
filename = 'generated_names_with_suffix.txt'
print(generate_names_with_suffix(suffix, num_names, filename))
```

    Generated 7 names with suffix '_xyz' and saved to generated_names_with_suffix.txt



```python

```


---
**Score: 5**
