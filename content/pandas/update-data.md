---
title: Update-Data
date: 2025-01-31
author: Your Name
cell_count: 4
score: 0
---

```python
import pandas as pd
```


```python
def update_df(file_name):
    #read dataframe
    df = pd.read_excel(file_name)

    df.loc[df['name']=='jerin','age'] = 21

    df.to_excel(file_name,index=False)

    return df
```


```python
update_df("data.xlsx")
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
      <th>1</th>
      <td>sanjay</td>
      <td>26</td>
      <td>madurai</td>
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
