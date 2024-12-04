---
title: Random-Find-Even-Odd
date: 2024-12-05
author: Your Name
cell_count: 6
score: 5
---

```python
import random
import time
```


```python
def is_odd(number):

    if(number % 2 != 0):
        print(f'{number} is odd number')
    else:
        print(f'{number} is even number')
```


```python
for _ in range(10):
        c_number = random.randint(1000, 2000)
        is_odd(c_number)
        time.sleep(1)
```

    1617 is odd number
    1172 is even number
    1545 is odd number
    1652 is even number
    1302 is even number
    1907 is odd number
    1265 is odd number
    1273 is odd number
    1946 is even number
    1772 is even number



```python
is_odd(10)
```

    10 is even number



```python
is_odd(1)
```

    1 is odd number



```python

```


---
**Score: 5**
