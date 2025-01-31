---
title: Basic-Multithreading
date: 2025-01-31
author: Your Name
cell_count: 13
score: 10
---

```python
# 20250131
```


```python
# Basic Multithreading with the GIL (CPU-bound)
```


```python
# import necessary library
```


```python
import threading
```


```python
import time
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
# Start two threads
```


```python
threads = []
```


```python
for _ in range(2):
    thread = threading.Thread(target=cpu_bound_task)
    threads.append(thread)
    thread.start()
```

    Result: 49999995000000Result: 49999995000000
    



```python
for thread in threads:
    thread.join()
```


```python

```


---
**Score: 10**
