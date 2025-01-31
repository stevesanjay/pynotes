---
title: Remove-Extra-Space
date: 2025-01-31
author: Your Name
cell_count: 5
score: 5
---

```python
# Find and Remove Extra Whitespaces
```


```python
import re
```


```python
def remove_extra_spaces(filename):
    with open(filename, 'r') as file:
        content = file.read()
        updated_content = re.sub(r'\s+', ' ', content).strip()
    
    with open(filename, 'w') as file:
        file.write(updated_content)
    
    return "Extra spaces removed."
```


```python
# Example usage
filename = 'sample.txt'
print(remove_extra_spaces(filename))
```

    Extra spaces removed.



```python

```


---
**Score: 5**
