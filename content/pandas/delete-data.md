---
title: Delete-Data
date: 2025-01-31
author: Your Name
cell_count: 4
score: 0
---

```python
import pandas as pd
```


```python
def delete_data_from_excel(file_name):
    df = pd.read_excel(file_name)

    dfs = df[df["name"]!= 'sanjay']

    dfs.to_excel(file_name,index=False)

    return dfs
```


```python
delete_data_from_excel("data.xlsx")
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>age</th>
      <th>city</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>steve</td>
      <td>25</td>
      <td>chennai</td>
    </tr>
    <tr>
      <th>2</th>
      <td>jerin</td>
      <td>21</td>
      <td>coimbatore</td>
    </tr>
    <tr>
      <th>3</th>
      <td>saravana</td>
      <td>28</td>
      <td>salem</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


---
**Score: 0**
