---
title: Count-Word
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
# Count the Number of Words in a File
```


```python
import re
```


```python
def count_words(filename):
    with open(filename, 'r') as file:
        content = file.read()
        words = re.findall(r'\b\w+\b', content)
        return len(words)
```


```python
# Example usage
filename = 'sample.txt'

```


```python
word_count = count_words(filename)

```


```python
print(f"Number of words: {word_count}")

```

    Number of words: 38



```python

```


---
**Score: 5**
