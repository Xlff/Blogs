# Day1-Extension


```swift
extension UIView {
	func addSubviews(_ subviews: UIView...) {
		subviews.forEach(addSubView)
	}
}

// 向父视图中添加
view.addSubviews(imageView, slider, view, label)
```


