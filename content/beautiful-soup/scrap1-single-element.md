---
title: Scrap1-Single-Element
date: 2024-12-05
author: Your Name
cell_count: 8
score: 5
---

```python
import requests
```


```python
from bs4 import BeautifulSoup

```


```python
url = "https://books.toscrape.com/catalogue/a-light-in-the-attic_1000/index.html"
```


```python
response = requests.get(url)
```


```python
soup = BeautifulSoup(response.content, 'html.parser')

```


```python
price = soup.find('p', class_='price_color').text
```


```python
print(price)
```

    £51.77



```python

```


---
**Score: 5**
