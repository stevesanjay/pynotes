---
title: Replace-Specific-Word
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
# Replace Specific Words in a File
```


```python
import re
```


```python
def replace_words(filename, target_word, replacement_word):
    with open(filename, 'r') as file:
        content = file.read()
        updated_content = re.sub(rf'\b{re.escape(target_word)}\b', replacement_word, content)
    
    with open(filename, 'w') as file:
        file.write(updated_content)
    
    return f"Replaced '{target_word}' with '{replacement_word}'."
```


```python
filename = 'sample.txt'
```


```python
print(replace_words(filename, "John", "Jane"))
```

    Replaced 'John' with 'Jane'.



```python

```


---
**Score: 5**
