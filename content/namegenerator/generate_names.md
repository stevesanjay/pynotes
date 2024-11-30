---
title: Generate Names
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
# Generate Random Usernames and Save to File
```


```python
!pip install namegenerator
```

    Collecting namegenerator
      Downloading namegenerator-1.0.6.tar.gz (4.4 kB)
      Preparing metadata (setup.py) ... [?25ldone
    [?25hBuilding wheels for collected packages: namegenerator
      Building wheel for namegenerator (setup.py) ... [?25ldone
    [?25h  Created wheel for namegenerator: filename=namegenerator-1.0.6-py3-none-any.whl size=4433 sha256=f5c8901d37e05e06b02c0c3a5c2ecf26c258d9617204297b1c186e0090a38040
      Stored in directory: /Users/tactlabs2/Library/Caches/pip/wheels/15/86/3c/110d482098a28761a75cce3a526b31de7789c17f381e459743
    Successfully built namegenerator
    Installing collected packages: namegenerator
    Successfully installed namegenerator-1.0.6



```python
import namegenerator

```


```python
def generate_usernames(filename, count=10):
    usernames = [namegenerator.gen() for _ in range(count)]
    
    with open(filename, 'w') as file:
        for username in usernames:
            file.write(username + "\n")
    
    return f"{count} usernames saved to {filename}"
```


```python
filename = 'usernames.txt'
```


```python
print(generate_usernames(filename))
```

    10 usernames saved to usernames.txt



```python

```


---
**Score: 5**
