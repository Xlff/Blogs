
---
title: Day5-滚动TableView时收起键盘
date: 2019-01-23 15:20:19 +0800
tags: []
categories: 
---

```swift
// 滚动时不收起
tableView.keyboardDismissMode = .none
// 滚动开始就收起
tableView.keyboardDismissMode = .onDrag
// 交互型, 可跟随滚动收起或向上滑动取消收起
tableView.keyboardDismissMode = .interactive

```


