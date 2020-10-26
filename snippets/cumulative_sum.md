---
title: cumulative_sum
tags: list,beginner
---

Returns the cumulative sum for a list.

- returns the cumulative sum of the list in linear time complexity.

```py
def cumulative_sum(lst):
    sum=0
    for i in range(len(lst)):
        lst[i]=lst[i]+sum
        sum=lst[i]
    return lst
```

```py
cumulative_sum([1, 2, 3, 4, 5, 6]) # [1, 3, 6, 10, 15, 21]
```