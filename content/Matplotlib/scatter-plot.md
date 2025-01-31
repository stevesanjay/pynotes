---
title: Scatter-Plot
date: 2025-01-31
author: Your Name
cell_count: 12
score: 10
---

```python
# Scatter Plot
```


```python
import matplotlib.pyplot as plt
```


```python
# Data
x = [1, 2, 3, 4, 5]
```


```python
# Data
y = [10, 20, 25, 30, 40]
```


```python
# Creating the scatter plot
plt.scatter(x, y)
```




    <matplotlib.collections.PathCollection at 0x10db69460>




    
![png](scatter-plot_files/scatter-plot_4_1.png)
    



```python
# Adding title and labels
```


```python
plt.title('Scatter Plot')
```




    Text(0.5, 1.0, 'Scatter Plot')




    
![png](scatter-plot_files/scatter-plot_6_1.png)
    



```python
plt.xlabel('X-axis')
```




    Text(0.5, 0, 'X-axis')




    
![png](scatter-plot_files/scatter-plot_7_1.png)
    



```python
plt.ylabel('Y-axis')
```




    Text(0, 0.5, 'Y-axis')




    
![png](scatter-plot_files/scatter-plot_8_1.png)
    



```python
plt.show()
```


```python
plt
```




    <module 'matplotlib.pyplot' from '/usr/local/Caskroom/miniconda/base/envs/py312/lib/python3.12/site-packages/matplotlib/pyplot.py'>




```python

```


---
**Score: 10**
