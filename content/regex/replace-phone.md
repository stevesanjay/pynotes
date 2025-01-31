---
title: Replace-Phone
date: 2025-01-31
author: Your Name
cell_count: 6
score: 5
---

```python
# Replace Phone Numbers in a File
```


```python
import re
```


```python
def replace_phone_numbers(filename, replacement="PHONE_NUMBER"):
    with open(filename, 'r') as file:
        content = file.read()
        updated_content = re.sub(r'\b\d{3}-\d{3}-\d{4}\b', replacement, content)
    
    with open(filename, 'w') as file:
        file.write(updated_content)
    
    return "Phone numbers replaced."
```


```python
filename = 'sample.txt'
```


```python
print(replace_phone_numbers(filename))
```

    Phone numbers replaced.



```python

```


---
**Score: 5**
