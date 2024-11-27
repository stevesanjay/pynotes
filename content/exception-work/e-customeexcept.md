---
title: E-Customeexcept
date: 2024-11-27
author: Your Name
cell_count: 4
score: 0
---

```python

```


```python
number = 18
```


```python
try:
    input_number = int(input("Enter a number :"))

    if input_number < number:
        raise InvalidAgeException
    else:
        print(f"your age {input_number} is eligible to vote ")

except InvalidAgeException:
    print("exception occured : invalid Age")
```

    Enter a number : 20


    your age 20 is eligible to vote 



```python

```


---
**Score: 0**
