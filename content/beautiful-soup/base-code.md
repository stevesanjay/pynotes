---
title: Base-Code
date: 2024-11-27
author: Your Name
cell_count: 16
score: 15
---

```python
# import necessary library
```


```python
from bs4 import BeautifulSoup
```


```python
# Sample HTML content
```


```python
html_content = """
<html>
<head>
    <title>Sample Page</title>
</head>
<body>
    <h1>Welcome to Web Scraping</h1>
    <p>This is a simple paragraph for demonstration.</p>
    <div>
        <h2>Subsection</h2>
        <ul>
            <li>Item 1</li>
            <li>Item 2</li>
            <li>Item 3</li>
        </ul>
    </div>
</body>
</html>
"""
```


```python
# Parse the HTML content
```


```python
soup = BeautifulSoup(html_content, 'html.parser')
```


```python
# Extract the title
```


```python
title = soup.title.text
```


```python
print(f"Title of the page: {title}")
```

    Title of the page: Sample Page



```python
# Extract the main header
```


```python
header = soup.h1.text
```


```python
print(f"Header: {header}")
```

    Header: Welcome to Web Scraping



```python
# Extract all list items
```


```python
list_items = soup.find_all('li')
```


```python
for idx, item in enumerate(list_items, start=1):
    print(f"List item {idx}: {item.text}")
```

    List item 1: Item 1
    List item 2: Item 2
    List item 3: Item 3



```python

```


---
**Score: 15**
