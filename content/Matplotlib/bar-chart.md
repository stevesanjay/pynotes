---
title: Bar-Chart
date: 2025-01-30
author: Your Name
cell_count: 13
score: 10
---

```python
# Bar Chart
```


```python
import matplotlib.pyplot as plt
```


```python
# Data
```


```python
categories = ['A', 'B', 'C', 'D']
```


```python
values = [7, 12, 5, 18]
```


```python
# Creating the bar chart
```


```python
plt.bar(categories, values)
```




    <BarContainer object of 4 artists>




    
![png](bar-chart_files/bar-chart_6_1.png)
    



```python
# Adding title and labels
```


```python
plt.title('Bar Chart')
```




    Text(0.5, 1.0, 'Bar Chart')




    
![png](bar-chart_files/bar-chart_8_1.png)
    



```python
plt.xlabel('Categories')
```




    Text(0.5, 0, 'Categories')




    
![png](bar-chart_files/bar-chart_9_1.png)
    



```python
plt.ylabel('Values')
```




    Text(0, 0.5, 'Values')




    
![png](bar-chart_files/bar-chart_10_1.png)
    



```python

```


```python

```


---
**Score: 10**
