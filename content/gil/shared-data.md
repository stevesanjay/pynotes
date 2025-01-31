---
title: Shared-Data
date: 2025-01-31
author: Your Name
cell_count: 15
score: 15
---

```python
# 20250131
```


```python
# Threading with Shared Data (GIL Locking)
```


```python
# import necessary library
```


```python
import threading
```


```python
# Shared resource
```


```python
shared_list = []
```


```python
# Task to append to shared list
```


```python
def append_to_list():
    for _ in range(100000):
        shared_list.append(1)
```


```python
append_to_list()
```


```python
# Start two threads
```


```python
threads = []
```


```python
for _ in range(2):
    thread = threading.Thread(target=append_to_list)
    threads.append(thread)
    thread.start()
```


```python
for thread in threads:
    thread.join()
```


```python
print(f"Shared list length: {len(shared_list)}")
```


```python

```


---
**Score: 15**
