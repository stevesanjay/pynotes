---
title: Replace-Space
date: 2024-11-22
author: Your Name
cell_count: 6
score: 5
---

```python
# Match and Replace Multiple Spaces with a Single Space
```


```python
import re
```


```python
def replace_multiple_spaces(filename):
    with open(filename, 'r') as file:
        content = file.read()
        updated_content = re.sub(r'\s+', ' ', content)
    
    with open(filename, 'w') as file:
        file.write(updated_content)
    
    return "Multiple spaces replaced with a single space."

```


```python
# Example usage
filename = 'sample.txt'
```


```python
print(replace_multiple_spaces(filename))
```

    Multiple spaces replaced with a single space.



```python

```


---
**Score: 5**
