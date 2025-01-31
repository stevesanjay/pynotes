---
title: Basic-Enum
date: 2025-01-30
author: Your Name
cell_count: 7
score: 5
---

```python
# basic enum
```


```python
# Import necessary modules
```


```python
from enum import Enum
```


```python
class AnimalEnum(Enum):
    HORSE = 1
    COW = 2
    CHICKEN = 3
    DOG = 4
```


```python
def startpy():
    
    print(AnimalEnum.CHICKEN)

    for animal in AnimalEnum:
        print('Name: {}  Value: {}'.format(animal, animal.value))
```


```python
startpy()
```

    AnimalEnum.CHICKEN
    Name: AnimalEnum.HORSE  Value: 1
    Name: AnimalEnum.COW  Value: 2
    Name: AnimalEnum.CHICKEN  Value: 3
    Name: AnimalEnum.DOG  Value: 4



```python

```


---
**Score: 5**
