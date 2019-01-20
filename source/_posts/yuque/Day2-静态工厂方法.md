
---
title: Day2-静态工厂方法
date: 2019-01-16 09:50:11 +0800
tags: []
categories: 
---

```swift
extension UILabel {
    //MARK: 标题静态工厂方法
    static func initForTitle() -> UILabel {
        let label = UILabel()
        label.font = .boldSystemFont(ofSize: 18)
        label.textColor = .darkGray
        label.numberOfLines = 1
        label.adjustsFontSizeToFitWidth = true
        label.minimumScaleFactor = 0.75
        return label
    }
    
    //MARK: 副标题静态工厂方法
    static func initForDescription() -> UILabel {
        let label = UILabel()
        label.font = .systemFont(ofSize: 14)
        label.textColor = .black
        label.numberOfLines = 0
        return label
    }
}

class ContentViewController: UIViewController {
    lazy var titleLabel = UILabel.initForTitle()
    lazy var detailLabel = UILabel.initForDescription()
}
```


