---
layout: post
title: UIView与CALayer
categories: [iOS]
description: UIView与CALayer的关系学习笔记
keywords: UIView, CALayer
---

## UIView与CALayer的关系
1. UIView为CALayer提供内容，负责触摸等事件，参与事件响应链。
2. CALayer负责其内容的显示。CALayer管理着基于图像的内容并且允许在该内容上执行动画。 

## UIView与CALayer的关系设计
1. UIView与CALayer之间的分工体现了单一职责原则设计原则
2. UIView作为CALayer的代理，体现了代理模式。

## 开发中注意事项
1. 由于UIView为其属性layer的代理，所以不要将UIView设置为其他CALayer对象的代理；另外也不要修改UIView的layer属性的代理。
