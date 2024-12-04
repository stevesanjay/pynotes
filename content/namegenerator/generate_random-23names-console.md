---
title: Generate Random-23Names-Console
date: 2024-12-05
author: Your Name
cell_count: 6
score: 5
---

```python
# Generate Random Names and Print to Console
```


```python
import namegenerator
```


```python
def generate_and_print_names(num_names):
    names = [namegenerator.gen() for _ in range(num_names)]
    for name in names:
        print(name)
```


```python
num_names = 5
```


```python
generate_and_print_names(num_names)
```

    gloppy-azure-chimpanzee
    squeaky-harlequin-oyster
    stinky-flax-chipmunk
    freaky-magnolia-zebra
    droopy-grey-vole



```python

```


---
**Score: 5**
