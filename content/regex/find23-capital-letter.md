---
title: Find23-Capital-Letter
date: 2025-01-31
author: Your Name
cell_count: 6
score: 5
---

```python
# Extract All Capitalized Words
```


```python
import re
```


```python
def extract_capitalized_words(filename):
    with open(filename, 'r') as file:
        content = file.read()
        capitalized_words = re.findall(r'\b[A-Z][a-z]*\b', content)
        return capitalized_words
```


```python
# Example usage
filename = 'sample.txt'
```


```python
capitalized_words = extract_capitalized_words(filename)
print("Capitalized words found:", capitalized_words)
```

    Capitalized words found: ['Hello', 'I', 'Here', 'Check']



```python

```


---
**Score: 5**
