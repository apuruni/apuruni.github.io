---
layout: post
title: "SwiftのstructをNSCoderでエンコードできない"
modified:
categories: 
excerpt:
tags: [swift NSCoder struct]
image:
  feature:
date: 2015-03-13T13:35:12+09:00
---

SwiftのstructがAnyObjectではない。
decoder.decodeObjectForKey("stuct_name") as StructA
で
'AnyObject' is not convertible to [StructA?]'
のコンパイルエラーが発生する。

## 結論
Cocoa Frameworkのクラスを使うなら、swiftのstructを避けるべき。