---
title: Exception Hand
date: 2024-12-05
author: Your Name
cell_count: 2
score: 0
---

```python
try:
    a = int(input("enter the numerator:")) 
    b = int(input("enter a denominator:"))
    divide_number = a/b
    result =  divide_number
    print(result)

except ZeroDivisionError:
    print(f'the denominator cannot be {b}')

finally:
    print("always printed")
```


```python

```


---
**Score: 0**
