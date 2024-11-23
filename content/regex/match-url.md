---
title: Match-Url
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
# Match URLs in a File
```


```python
import re
```


```python
def extract_urls(filename):
    with open(filename, 'r') as file:
        content = file.read()
        urls = re.findall(r'https?://[^\s]+', content)
        return urls
```


```python
# Example usage
filename = 'sample.txt'
```


```python
urls = extract_urls(filename)
print("URLs found:", urls)
```

    URLs found: ['https://www.example.com']



```python

```


---
**Score: 5**
