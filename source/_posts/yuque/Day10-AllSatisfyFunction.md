
---
title: Day10-AllSatisfyFunction
date: 2019-02-21 10:09:17 +0800
tags: []
categories: 
---
返回序列中的值是否都满足条件:
```swift
    public func allSatisfy(_ predicate: (Element) throws -> Bool) rethrows -> Bool
```

例子:

```swift
let names = ["Sofia", "Camilla", "Martina", "Mateo", "Nicolás"]
let allHaveAtLeastFive = names.allSatisfy({ $0.count >= 5 })
// allHaveAtLeastFive = true

let numbers = [2, 10, 15, 19, 8]
let allNumberLargeThanTen = numbers.allSatisfy({ $0 > 10 })
// allNumberLargeThanTen = false
```



