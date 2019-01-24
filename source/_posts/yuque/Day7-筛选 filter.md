
---
title: Day7-筛选 filter
date: 2019-01-24 10:13:46 +0800
tags: []
categories: 
---
定义:
```swift
func filter(includeElement: (T) -> Bool) -> [T]
```
参数是一个条件, 根据Bool值来返回符合条件的元素

```swift
// 取出大于10 的数
let array = [1, 5, 20, 14, 6, 30, 9, 10]
let result = array.filter{ $0 > 10}
print(result) // [20, 14, 30]
```


