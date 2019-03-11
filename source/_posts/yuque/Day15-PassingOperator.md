
---
title: Day15-PassingOperator
date: 2019-03-11 15:35:29 +0800
tags: []
categories: 
---
将操作符号用作闭包传递

```swift
let numbers = [5,1,52,25,14,6,33]
let sorted = numbers.sorted(by: >)
print(sorted)
// [52, 33, 25, 14, 6, 5, 1]
```


