---
title: Seaborn5 Pairplot
date: 2025-01-31
author: Your Name
cell_count: 14
score: 10
---

```python

```


```python
import matplotlib.pyplot as plt
```


```python
import seaborn as sns
```


```python
# Load dataset
```


```python
penguins = sns.load_dataset('penguins')
```


```python
# Create pairplot
```


```python
pairplot = sns.pairplot(data=penguins, hue="species", palette="muted", diag_kind="kde", markers=["o", "s", "D"])
```


    
![png](seaborn5_pairplot_files/seaborn5_pairplot_6_0.png)
    



```python
# Customize plot
```


```python
pairplot.fig.suptitle("Pairplot of Penguin Dataset", fontsize=16)
```




    Text(0.5, 0.98, 'Pairplot of Penguin Dataset')




```python
pairplot.fig.tight_layout()
```


```python
# Save plot
```


```python
pairplot.savefig("seaborn10_pairplot.png")
```


```python
plt.show()
```


```python

```


---
**Score: 10**
