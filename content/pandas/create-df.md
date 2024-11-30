---
title: Create-Df
date: 2024-11-30
author: Your Name
cell_count: 6
score: 5
---

```python
import pandas as pd
```


```python
def create_df():

    data = {
        'name':['steve','sanjay','jerin','saravana'],
        'age':[25,26,27,28],
        'city':['chennai','madurai','coimbatore','salem']
    }

    df = pd.DataFrame(data)
    print(df)
```


```python
print(create_df())
```

           name  age        city
    0     steve   25     chennai
    1    sanjay   26     madurai
    2     jerin   27  coimbatore
    3  saravana   28       salem
    None



```python
def create_dataframe_(filename):

    data = {
        'name':['steve','sanjay','jerin','saravana'],
        'age':[25,26,27,28],
        'city':['chennai','madurai','coimbatore','salem']
    }

    df = pd.DataFrame(data)
    df.to_excel(filename,index=False)
```


```python
create_dataframe_("datas.xlsx")
```


```python

```


---
**Score: 5**
