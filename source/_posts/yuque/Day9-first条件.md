
---
title: Day9-first条件
date: 2019-02-20 09:41:08 +0800
tags: []
categories: 
---
# first(where:)
返回一个满足条件的值
```swift
func first(where predicate: (Value) throws -> Bool) rethrows -> Value?
```

例子:
```swift
let numbers = [2, 5, 8, -4, -10, 20, 19]
if let number = numbers.first(where: { $0 < 0 }) {
    print("数组中第一个小于0的数: \(number)")
}
// 数组中第一个小于0的数: -4
```


