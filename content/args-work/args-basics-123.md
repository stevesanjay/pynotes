---
title: Args-Basics-123
date: 2024-11-27
author: Your Name
cell_count: 7
score: 5
---

```python
# reading data by using the args.
```


```python
def print_everything(*args):
        for count, thing in enumerate(args):
            print( '{0}. {1}'.format(count, thing))
```


```python
# read the data from the print_everything method 
```


```python
def main():
    print_everything('apple', 'banana', 'cabbage', 'spinach')
```


```python
main()
```

    0. apple
    1. banana
    2. cabbage
    3. spinach



```python
print_everything()
```


```python

```


---
**Score: 5**
