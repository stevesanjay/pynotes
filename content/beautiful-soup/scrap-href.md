---
title: Scrap-Href
date: 2024-11-27
author: Your Name
cell_count: 8
score: 5
---

```python
from bs4 import BeautifulSoup
```


```python
import requests
```


```python
url = "https://books.toscrape.com/"
```


```python
response = requests.get(url)
```


```python
soup = BeautifulSoup(response.text, "html.parser")
```


```python
def get_book_details():
    book_list = []
    for row in soup.select("section div ol li"):
        # print(row)

        link = row.select("a")[1]
        
        link_href = link['href']
       
        
        book_list.append({
            'link' : link_href
        })

    for 

    return book_list
```


```python
for book in get_book_details():
    print(book)
```

    {'link': 'catalogue/a-light-in-the-attic_1000/index.html'}
    {'link': 'catalogue/tipping-the-velvet_999/index.html'}
    {'link': 'catalogue/soumission_998/index.html'}
    {'link': 'catalogue/sharp-objects_997/index.html'}
    {'link': 'catalogue/sapiens-a-brief-history-of-humankind_996/index.html'}
    {'link': 'catalogue/the-requiem-red_995/index.html'}
    {'link': 'catalogue/the-dirty-little-secrets-of-getting-your-dream-job_994/index.html'}
    {'link': 'catalogue/the-coming-woman-a-novel-based-on-the-life-of-the-infamous-feminist-victoria-woodhull_993/index.html'}
    {'link': 'catalogue/the-boys-in-the-boat-nine-americans-and-their-epic-quest-for-gold-at-the-1936-berlin-olympics_992/index.html'}
    {'link': 'catalogue/the-black-maria_991/index.html'}
    {'link': 'catalogue/starving-hearts-triangular-trade-trilogy-1_990/index.html'}
    {'link': 'catalogue/shakespeares-sonnets_989/index.html'}
    {'link': 'catalogue/set-me-free_988/index.html'}
    {'link': 'catalogue/scott-pilgrims-precious-little-life-scott-pilgrim-1_987/index.html'}
    {'link': 'catalogue/rip-it-up-and-start-again_986/index.html'}
    {'link': 'catalogue/our-band-could-be-your-life-scenes-from-the-american-indie-underground-1981-1991_985/index.html'}
    {'link': 'catalogue/olio_984/index.html'}
    {'link': 'catalogue/mesaerion-the-best-science-fiction-stories-1800-1849_983/index.html'}
    {'link': 'catalogue/libertarianism-for-beginners_982/index.html'}
    {'link': 'catalogue/its-only-the-himalayas_981/index.html'}



```python

```


---
**Score: 5**
