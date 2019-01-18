---
title: Day1-Extension
date: 2019-01-18 11:40:22
tags:
---

```swift
extension UIView {
	func addSubviews(_ subviews: UIView...) {
		subviews.forEach(addSubView)
	}
}

// 向父视图中添加
view.addSubviews(imageView, slider, view, label)
```


