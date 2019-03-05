
---
title: Day13-MapFuction
date: 2019-03-05 11:13:06 +0800
tags: []
categories: 
---

```swift
func map<T>(_ transform: (Element) throws -> T) rethrows -> [T]
```
将序列中的每一个元素都映射到一个新的数组中.

例子:

```swift
let cast = ["Vivien", "Max", "Xie", "Kim"]
let lowercaseNames = cast.map { $0.lowercased() } // ["vivien", "max", "xie", "kim"]
let letterCounts = cast.map { $0.count )} // [6, 3, 3, 3]
```

对Optional值作变化和操作.

```swift
public enum Optional<T>:
		_Reflectable, NilLiteralConvertible {
      // 若果self为nil, 则返回nil. 否则返回f(self)
      public func map<U>(@noescape f:(T) -> U) -> U?
}

```

```swift
let num: Int? = 3
let result = num.map{ $0 * 2 } // Optional(6)
```


