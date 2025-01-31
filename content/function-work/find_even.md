---
title: Find Even
date: 2025-01-31
author: Your Name
cell_count: 3
score: 0
---

```python
def startpy():
    
    # change elements of a list [1, 9, 10, 11, 201, 8], to 0 if the element exceeds 20.
    element_list = [1, 9, 10, 11, 201, 8]
    new_element_list = []
    
    for a in element_list:
        
        if (a % 2 == 0):
            new_element_list.append(a)
        else:
            print(f"{a} is odd number")

    print(new_element_list)
```


```python
 startpy()
```

    1 is odd number
    9 is odd number
    11 is odd number
    201 is odd number
    [10, 8]



```python

```


---
**Score: 0**
