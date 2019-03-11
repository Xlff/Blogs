
---
title: Day14-CompactMapFunction
date: 2019-03-06 15:33:31 +0800
tags: []
categories: 
---
Swift4.1 开始.<br />当转换数组时， 使用compactmap(_:)可剔出nil值, 可省略解包过程。<br />例子：
```swift
let numbers = ["5", "42", "nine", "100", "Bob"]
let mapResult = numbers.map({ Int($0) })

let compactResult = numbers.compactMap({ Int($0) })

print(mapResult)
// [Optional(5), Optional(42), nil, Optional(100), nil]  返回的数组类型为[Int?]
print(compactResult)
// [5, 42, 100]  返回的数组类型为[Int]
```


