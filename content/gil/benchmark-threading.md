---
title: Benchmark-Threading
date: 2025-01-31
author: Your Name
cell_count: 23
score: 20
---

```python
# 20250130
```


```python
# GIL and Performance Benchmark (CPU-bound)
```


```python
# import necessary library
```


```python
import threading
```


```python
import multiprocessing
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
```


```python
# Benchmark threading
```


```python
start_time = time.time()
```


```python
threads = [threading.Thread(target=cpu_bound_task) for _ in range(2)]
```


```python
threads
```




    [<Thread(Thread-5 (cpu_bound_task), initial)>,
     <Thread(Thread-6 (cpu_bound_task), initial)>]




```python
for thread in threads:
    thread.start()
```


```python
for thread in threads:
    thread.join()
```


```python
threading_time = time.time() - start_time
```


```python
threading_time
```




    38.49284315109253




```python
# Benchmark multiprocessing
```


```python
start_time = time.time()
```


```python
processes = [multiprocessing.Process(target=cpu_bound_task) for _ in range(2)]
```


```python

```


```python

multiprocessing_time = time.time() - start_time
```


```python
print(f"Threading time: {threading_time} seconds")
print(f"Multiprocessing time: {multiprocessing_time} seconds")
```

    Threading time: 38.49284315109253 seconds
    Multiprocessing time: 99.18928098678589 seconds



```python

```


---
**Score: 20**
