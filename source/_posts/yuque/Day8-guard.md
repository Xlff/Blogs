
---
title: Day8-guard
date: 2019-01-24 17:18:42 +0800
tags: []
categories: 
---
guard是一个条件语句,必须条件为真时才继续执行, 否则提前退出函数.
# 1. 验证入口条件

```swift
func sayHello(numberOfTimes: Int) {
  	// 传入次数大于0时才打印, 否则直接返回.
    guard numberOfTimes > 0 else { return }
    for _ in 1...numberOfTimes {
        print("Hello!")
    }
}
```
# 2.对可选值进行解包,代替if let..else

```swift
let label: UILabel?

func updateLabelText(_ text: String) {
  guard let label = self.label else { return }
  label.text = text
}
```
# 3.不要用作if的相反情况
guard不是通常意义上的分支语义. 它特别强调在不满足期望条件时,提前退出.

# 4.不要在else语句中放入复杂代码
最好不要多于2-3行代码.

