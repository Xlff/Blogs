
---
title: Day4-方法的缩写
date: 2019-01-23 15:15:03 +0800
tags: []
categories: 
---

```swift
let view = UIView()
// 设置背景颜色UIColor.white
view.backgroundColor = .white
// 设置frame时 CGRect.zero
view.frame = .zero

let tableView : UITableView?
// 当我们知道对象的具体类型时,可以缺省类名  如:UITableView
tableView = .init(frame: .zero, style: .plain)
```


