---
title: Args1
date: 2024-11-22
author: Your Name
cell_count: 4
score: 0
---

```python
def print_everything(*args):
        for count, thing in enumerate(args):
            print( '{0}. {1}'.format(count, thing))
```


```python
def main():
    print_everything('apple', 'banana', 'cabbage', 'spinach')
```


```python
if __name__ == '__main__':
    main()
```

    0. apple
    1. banana
    2. cabbage
    3. spinach



```python

```


---
**Score: 0**
