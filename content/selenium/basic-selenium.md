---
title: Basic-Selenium
date: 2025-01-31
author: Your Name
cell_count: 11
score: 10
---

```python
# import necessary library
```


```python
from selenium import webdriver
```


```python
# Initialize the Chrome driver
```


```python
driver = webdriver.Chrome()
```


```python
# Open a website
```


```python
driver.get("https://www.google.com")
```


```python
# Print the title of the page
```


```python
print(driver.title)
```

    Google



```python
# Close the browser
```


```python
driver.quit()
```


```python

```


---
**Score: 10**
