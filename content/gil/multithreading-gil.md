---
title: Multithreading-Gil
date: 2025-01-31
author: Your Name
cell_count: 12
score: 10
---

```python
# 20250130
```


```python
# Multithreading with the GIL (I/O-bound)
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
# I/O-bound task
```


```python
def io_bound_task():
    time.sleep(2)  # Simulate I/O operation
    print("I/O Task Done")
```


```python
# Start two threads
```


```python
threads = []
```


```python
for _ in range(2):
    thread = threading.Thread(target=io_bound_task)
    threads.append(thread)
    thread.start()
```

    I/O Task DoneI/O Task Done
    



```python
for thread in threads:
    thread.join()
```


```python

```


---
**Score: 10**
