
---
title: Day12-InoutParameter
date: 2019-03-04 09:50:09 +0800
tags: []
categories: 
---
如果想要一个函数修改参数的值,并且修改后的值保存到函数被调用完成.那么用in-out参数来代替这个参数.<br />例子:  有时复杂的问题可能需要用到递归,使用inout参数可以在许多递归中共享参数

```swift
func x(depth: inout Int) {
	depth += 1
  if (depth < 10) {
  	x(depth: &depth)
  }
}
var depth = 0
x(depth: &depth)
print(depth) //10 
```

注意: <br />inout修饰的参数不能是不可变参数(let)<br />调用的时候,必须使用&符号, 指向原地址

