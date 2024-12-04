---
title: Stacked-Bar-Chart
date: 2024-12-05
author: Your Name
cell_count: 16
score: 15
---

```python
# Stacked Bar Chart
```


```python
# import necessary library
```


```python
import matplotlib.pyplot as plt

```


```python
# Data
```


```python
labels = ['A', 'B', 'C', 'D']
```


```python
category1 = [4, 7, 9, 6]
```


```python
category2 = [3, 2, 5, 1]

```


```python
# Creating a stacked bar chart
```


```python
plt.bar(labels, category1, label='Category 1')
```




    <BarContainer object of 4 artists>




    
![png](stacked-bar-chart_files/stacked-bar-chart_8_1.png)
    



```python
plt.bar(labels, category2, bottom=category1, label='Category 2')
```




    <BarContainer object of 4 artists>




    
![png](stacked-bar-chart_files/stacked-bar-chart_9_1.png)
    



```python
# Adding title and labels
```


```python
plt.title('Stacked Bar Chart')
```




    Text(0.5, 1.0, 'Stacked Bar Chart')




    
![png](stacked-bar-chart_files/stacked-bar-chart_11_1.png)
    



```python
plt.xlabel('Categories')
```




    Text(0.5, 0, 'Categories')




    
![png](stacked-bar-chart_files/stacked-bar-chart_12_1.png)
    



```python
plt.ylabel('Values')
```




    Text(0, 0.5, 'Values')




    
![png](stacked-bar-chart_files/stacked-bar-chart_13_1.png)
    



```python
plt.legend()
```

    /var/folders/ss/5vtwrdm14673srh7sngd_6880000gn/T/ipykernel_51940/4061938096.py:1: UserWarning: No artists with labels found to put in legend.  Note that artists whose label start with an underscore are ignored when legend() is called with no argument.
      plt.legend()





    <matplotlib.legend.Legend at 0x116fecf50>




    
![png](stacked-bar-chart_files/stacked-bar-chart_14_2.png)
    



```python

```


---
**Score: 15**
