---
title: Find123-Hexa
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
# Extract All Hexadecimal Values
```


```python
import re
```


```python
def extract_hex_values(filename):
    with open(filename, 'r') as file:
        content = file.read()
        hex_values = re.findall(r'\b0[xX][0-9a-fA-F]+\b', content)
        return hex_values

```


```python
filename = 'sample.txt'
```


```python
hex_values = extract_hex_values(filename)
print("Hexadecimal values found:", hex_values)

```

    Hexadecimal values found: []



```python

```


---
**Score: 5**
