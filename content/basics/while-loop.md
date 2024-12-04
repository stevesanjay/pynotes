---
title: While-Loop
date: 2024-12-05
author: Your Name
cell_count: 4
score: 0
---

```python
import random
import time
```


```python
def startpy():

    count = 0
    while (True):

        count += 1

        c_number = random.randint(1000, 2000)

        if(c_number %9 == 0):
            print(f"{count}: my number : {c_number} is divided by nine. So breaking the loop")
            break

        print(f"{count}: my number : {c_number}")
        time.sleep(1)

        # breaking the loop
        if(count > 4):
            break
```


```python
startpy()
```

    1: my number : 1490
    2: my number : 1249
    3: my number : 1938
    4: my number : 1491
    5: my number : 1183



```python

```


---
**Score: 0**
