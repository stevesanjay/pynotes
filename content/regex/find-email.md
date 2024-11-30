---
title: Find-Email
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
# Search for a Pattern in a File
```


```python
import re
```


```python
def extract_emails(filename):
    with open(filename, 'r') as file:
        content = file.read()
        emails = re.findall(r'[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}', content)
        return emails
```


```python
filename = 'sample.txt'
```


```python
emails = extract_emails(filename)
```


```python
emails
```




    ['john.doe@example.com']




```python

```


---
**Score: 5**
