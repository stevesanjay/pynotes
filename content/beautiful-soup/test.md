---
title: Test
date: 2025-01-31
author: Your Name
cell_count: 14
score: 10
---

```python
# import necessary library
```


```python
import requests
```


```python
from bs4 import BeautifulSoup
```


```python
# URL of the webpage
```


```python
url = "https://books.toscrape.com/catalogue/a-light-in-the-attic_1000/index.html"
```


```python
# Send a GET request to fetch the webpage content
```


```python
response = requests.get(url)
```


```python
# Parse the HTML content
```


```python
soup = BeautifulSoup(response.text, 'html.parser')
```


```python
# Use the copied CSS selector to find the price
```


```python
price_element = soup.select_one("#content_inner > article > div.row > div.col-sm-6.product_main > p.price_color")
```


```python
# Check if the element is found and extract the text
```


```python
if price_element:
    print("Price:", price_element.text)
else:
    print("Price not found")
```

    Price: Â£51.77



```python

```


---
**Score: 10**
