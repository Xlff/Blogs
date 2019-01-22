
---
title: Day3: UIColor便利方法
date: 2019-01-22 10:24:24 +0800
tags: []
categories: 
---

```swift
extension UIColor {
  	// 重定义rgb
    convenience init(r: Int, g: Int, b: Int, a: CGFloat) {
        self.init(red: CGFloat(r) / 255.0, green: CGFloat(b) / 255.0, blue: CGFloat(g) / 255.0, alpha: a)
    }
    convenience init(r: Int, g: Int, b: Int) {
        self.init(r: r, g: g, b: b, a: 1.0)
    }
    // 使用十六进制
    convenience init(hex: Int) {
        self.init(r: (hex >> 16) & 0xff, g: (hex >> 8) & 0xff, b: hex & 0xff)
    }
}

UIColor.init(r: 151, g: 151, b: 151)
UIColor.init(r: 200, g: 100, b: 199, a: 0.5)

UIColor.init(hex: 0x5fc7dc)
```

![day3-1.jpg](https://cdn.nlark.com/yuque/0/2019/jpeg/241566/1548124726816-f55bfed5-149e-4d4a-9cd1-896bede5f206.jpeg#align=left&display=inline&height=61&linkTarget=_blank&name=day3-1.jpg&originHeight=194&originWidth=2366&size=15104&width=746)

