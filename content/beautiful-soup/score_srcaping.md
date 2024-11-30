---
title: Score Srcaping
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python

```


```python
import requests
```


```python
from bs4 import BeautifulSoup
```


```python
def get_score(url):

    # Fetch the page content
    response = requests.get(url)

    # Parse the HTML content
    soup = BeautifulSoup(response.text, 'html.parser')

    overall_score_element = soup.find('p')  # Locate the <p> tag
    if overall_score_element:
        strong_tag = overall_score_element.find('strong')  # Locate the <strong> tag inside <p>
        if strong_tag and "Overall Score:" in strong_tag.text:
            overall_score = overall_score_element.get_text(strip=True).replace("Overall Score:", "").strip()
            return int(overall_score)
        return -1

    return -1
```


```python
def startpy():

    # print("Tact101")
    print(get_score("https://stevesanjay.github.io/pynotes/archives.html"))
```


```python
startpy()
```

    510



```python

```


---
**Score: 5**
