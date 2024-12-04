---
title: Read-Data
date: 2024-12-05
author: Your Name
cell_count: 4
score: 0
---

```python
import pandas as pd
```


```python
def read_excel(file_name):
    df = pd.read_excel(file_name)
    print(df)
    return df
```


```python
read_excel("data.xlsx")
```

           name  age        city
    0     steve   25     chennai
    1    sanjay   26     madurai
    2     jerin   27  coimbatore
    3  saravana   28       salem





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
      <td>27</td>
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
