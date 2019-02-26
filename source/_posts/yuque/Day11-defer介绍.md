
---
title: Day11-defer介绍
date: 2019-02-26 14:53:13 +0800
tags: []
categories: 
---
defer用于延迟执行,在函数执行完成后再执行defer中的代码.<br />例子:

```swift
func simpleDefer() {
    defer {
        print("defer code")
    }   
    print("other code")
}
simpleDefer()
// other code
// defer code
```


