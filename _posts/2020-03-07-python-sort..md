---
title: python sort学习
description: sort 学习
categories:
 - python
tags:
---

## 简单用法
直接`sort`
```python
a = [1,7,9,5,6,3]
a.sort()
# a = [1,3,5,6,7,9]
a.sort(reverse=True)
# a = [9,7,6,5,3,1]

```

指定key,可以理解成将每个元素通过key映射成一个值，用该值进行排序
```
prior = [1,2,4,5,6]
def helper(x):
    if x in prior:
        return (0, x)
    return (1, x)
a=[1,5,6,8,3]
a.sort(key=helper)
```
## reference
https://docs.python.org/zh-cn/3/howto/sorting.html
