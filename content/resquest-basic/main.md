---
title: Main
date: 2025-01-30
author: Your Name
cell_count: 18
score: 15
---

```python
import requests as req
import json
```


```python
response = req.get("https://randomuser.me/api/")
```


```python
response
```




    <Response [200]>




```python
response_json = response.json()
```


```python
response_json
```




    {'results': [{'gender': 'female',
       'name': {'title': 'Ms', 'first': 'Madlen', 'last': 'Hettich'},
       'location': {'street': {'number': 3512, 'name': 'Jahnstraße'},
        'city': 'Buckow (Märkische Schweiz)',
        'state': 'Bayern',
        'country': 'Germany',
        'postcode': 92330,
        'coordinates': {'latitude': '-49.1783', 'longitude': '26.2957'},
        'timezone': {'offset': '+10:00',
         'description': 'Eastern Australia, Guam, Vladivostok'}},
       'email': 'madlen.hettich@example.com',
       'login': {'uuid': 'a5af5721-efdd-439f-bff4-7a0f058a1533',
        'username': 'crazykoala669',
        'password': 'zander',
        'salt': '9YZoK9T7',
        'md5': '8997fb783bdc8e5a2aab49e6b24531d9',
        'sha1': 'fc7ecb3d611effa5243e9e39836ddffca73fe320',
        'sha256': '2476c2301967393eb03de9f79a23af26985510ff586d43b4285cc328c4af34df'},
       'dob': {'date': '1944-10-21T18:16:15.911Z', 'age': 80},
       'registered': {'date': '2021-09-20T15:49:47.687Z', 'age': 3},
       'phone': '0356-0312722',
       'cell': '0179-3581641',
       'id': {'name': 'SVNR', 'value': '50 211044 H 784'},
       'picture': {'large': 'https://randomuser.me/api/portraits/women/1.jpg',
        'medium': 'https://randomuser.me/api/portraits/med/women/1.jpg',
        'thumbnail': 'https://randomuser.me/api/portraits/thumb/women/1.jpg'},
       'nat': 'DE'}],
     'info': {'seed': '7ff1574d980e5774',
      'results': 1,
      'page': 1,
      'version': '1.4'}}




```python
result_first_item = response_json["results"][0]
```


```python
result_first_item
```




    {'gender': 'female',
     'name': {'title': 'Ms', 'first': 'Madlen', 'last': 'Hettich'},
     'location': {'street': {'number': 3512, 'name': 'Jahnstraße'},
      'city': 'Buckow (Märkische Schweiz)',
      'state': 'Bayern',
      'country': 'Germany',
      'postcode': 92330,
      'coordinates': {'latitude': '-49.1783', 'longitude': '26.2957'},
      'timezone': {'offset': '+10:00',
       'description': 'Eastern Australia, Guam, Vladivostok'}},
     'email': 'madlen.hettich@example.com',
     'login': {'uuid': 'a5af5721-efdd-439f-bff4-7a0f058a1533',
      'username': 'crazykoala669',
      'password': 'zander',
      'salt': '9YZoK9T7',
      'md5': '8997fb783bdc8e5a2aab49e6b24531d9',
      'sha1': 'fc7ecb3d611effa5243e9e39836ddffca73fe320',
      'sha256': '2476c2301967393eb03de9f79a23af26985510ff586d43b4285cc328c4af34df'},
     'dob': {'date': '1944-10-21T18:16:15.911Z', 'age': 80},
     'registered': {'date': '2021-09-20T15:49:47.687Z', 'age': 3},
     'phone': '0356-0312722',
     'cell': '0179-3581641',
     'id': {'name': 'SVNR', 'value': '50 211044 H 784'},
     'picture': {'large': 'https://randomuser.me/api/portraits/women/1.jpg',
      'medium': 'https://randomuser.me/api/portraits/med/women/1.jpg',
      'thumbnail': 'https://randomuser.me/api/portraits/thumb/women/1.jpg'},
     'nat': 'DE'}




```python
result_country = result_first_item.get("location",{}).get("country",{})
```


```python
result_country
```




    'Germany'




```python
result_timezone = result_first_item.get("location",{}).get("timezone",{}).get("offset",{})
```


```python
result_timezone
```




    '+10:00'




```python
result_password = result_first_item.get("login",{}).get("password",{})
```


```python
result_password
```




    'zander'




```python
result_age = result_first_item.get("dob",{}).get("age",{})
```


```python
result_age
```




    80




```python
def get_user_details(response_json):
    result_first_item = response_json["results"][0]
    user_country  = result_first_item.get("location",{}).get("country",{})
    user_timezone = result_first_item.get("location",{}).get("timezone",{}).get("offset",{})
    user_password = result_first_item.get("login",{}).get("password",{})
    user_age      = result_first_item.get("dob",{}).get("age",{})

    result_dict = {
        "country"  : user_country,
        "timezone" : user_timezone,
        "password" : user_password,
        "age"      : user_age
    }
    return result_dict
```


```python
res = req.get("https://randomuser.me/api/")
get_user_details(res.json())
```




    {'country': 'New Zealand',
     'timezone': '+6:00',
     'password': 'viewer',
     'age': 65}




```python

```


---
**Score: 15**
