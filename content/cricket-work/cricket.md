---
title: Cricket
date: 2024-12-05
author: Your Name
cell_count: 8
score: 5
---

```python
import random
```


```python
import time
```


```python
def startpy():

    count = 0
    total_score = 0
    total_wickets = 0
    while (True):

        count += 1

        c_score     = random.randint(0, 6)
        c_flag      = random.choice([True, False, True, True, True, True])

        if(c_flag == False):

            print(f"Ball {count}: It's a Wicket")
            
            total_wickets += 1

            if(total_wickets > 1):
                print(f"Ball {count}: Wicket, so finishing the match")
                break

            continue

        print(f"Ball {count}: Score : {c_score}")
        time.sleep(1)

        total_score += c_score

        # breaking the loop
        if(count >=6 ):
            break

    print(f'\nTotal Score : {total_score}')

```


```python
startpy()
```

    Ball 1: Score : 4
    Ball 2: It's a Wicket
    Ball 3: Score : 2
    Ball 4: Score : 2
    Ball 5: Score : 4
    Ball 6: Score : 0
    
    Total Score : 12



```python
startpy()
```

    Ball 1: Score : 0
    Ball 2: Score : 4
    Ball 3: It's a Wicket
    Ball 4: Score : 4
    Ball 5: Score : 5
    Ball 6: Score : 1
    
    Total Score : 14



```python
startpy()
```

    Ball 1: Score : 0
    Ball 2: Score : 5
    Ball 3: Score : 5
    Ball 4: Score : 2
    Ball 5: Score : 2
    Ball 6: Score : 4
    
    Total Score : 18



```python
startpy()
```

    Ball 1: Score : 3
    Ball 2: Score : 0
    Ball 3: Score : 2
    Ball 4: Score : 2
    Ball 5: Score : 6
    Ball 6: Score : 5
    
    Total Score : 18



```python

```


---
**Score: 5**
