
---
title: Day1-Extension
date: 2019-01-16 09:38:49 +0800
tags: []
categories: 
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



