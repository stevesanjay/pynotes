---
title: Area-Plot
date: 2024-11-30
author: Your Name
cell_count: 14
score: 10
---

```python
# Area Plot
```


```python
# import necessary library
```


```python
import matplotlib.pyplot as plt
```


```python
import numpy as np

```


```python
# Data
```


```python
x = np.linspace(0, 10, 100)
```


```python
y = np.sin(x)
```


```python
# Creating an area plot
```


```python
plt.fill_between(x, y, color='skyblue', alpha=0.5)
```




    <matplotlib.collections.PolyCollection at 0x116e7bc20>




    
![png](area-plot_files/area-plot_8_1.png)
    



```python
# Adding title and labels
```


```python
plt.title('Area Plot')
```




    Text(0.5, 1.0, 'Area Plot')




    
![png](area-plot_files/area-plot_10_1.png)
    



```python
plt.xlabel('X-axis')
```




    Text(0.5, 0, 'X-axis')




    
![png](area-plot_files/area-plot_11_1.png)
    



```python
plt.ylabel('Y-axis')
```




    Text(0, 0.5, 'Y-axis')




    
![png](area-plot_files/area-plot_12_1.png)
    



```python

```


---
**Score: 10**
