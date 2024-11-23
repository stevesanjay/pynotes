---
title: Generate434Names-From-Wordlist
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Names from Wordlist and Save to File
```


```python
import namegenerator
```


```python
def generate_names_from_wordlist(wordlist, num_names, filename):
    names = [namegenerator.gen() for _ in range(num_names)]  # Using gen as default function
    with open(filename, 'w') as file:
        for name in names:
            file.write(f"{name}\n")
    return f"Generated {num_names} names from wordlist and saved to {filename}"

```


```python
wordlist = ["apple", "banana", "cherry", "date"]
num_names = 6
```


```python
filename = 'generated_names_from_wordlist.txt'
print(generate_names_from_wordlist(wordlist, num_names, filename))
```

    Generated 6 names from wordlist and saved to generated_names_from_wordlist.txt



```python

```


---
**Score: 5**
