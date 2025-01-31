---
title: Multiprocessing-To-Bypass-Gil
date: 2025-01-31
author: Your Name
cell_count: 10
score: 10
---

```python
# 20250130
```


```python
# Using multiprocessing to Bypass GIL
```


```python
# import necessary library
```


```python
import multiprocessing
```


```python
# CPU-bound task
```


```python

def cpu_bound_task():
    result = 0
    for i in range(10**7):
        result += i
    print(f"Result: {result}")

```


```python
cpu_bound_task()
```

    Result: 49999995000000



```python
# Start two processes
```


```python
if __name__ == "__main__":
    processes = []
    for _ in range(2):
        process = multiprocessing.Process(target=cpu_bound_task())
        processes.append(process)
        process.start()

    for process in processes:
        process.join()
```

    Result: 49999995000000
    Result: 49999995000000



```python

```


---
**Score: 10**
