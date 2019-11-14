# 框架简介

BBuilder内置axicompiler框架，该框架包含编译器、DSL定义规范和内置组件/API等部分。

## DSL定义与编译器

axicompiler编译器原理是将各个平台运行环境抽象出一个模型，在该模型的基础上设计统一DSL规范。

该DSL规范类似于VUE，但是分为页面代码和组件代码两部分，结构和生命周期略有区别。详情请移步至：<a href="./page.html" target="_blank">页面定义</a>、<a href="./component.html" target="_blank">组件定义</a>

需要注意的是，目前DSL规范还不支持template，统一使用组件代替。

## 内置组件

框架内置了一些基础组件，这些组件都是经过二次封装，如果代码明确运行在固定平台，比如小程序，可以直接在代码中使用小程序的组件。

也就是说，当有明确运行的平台时，可以同时写内置组件和目标平台组件。

## 内置API

内置API提供了跨平台的JS API支持，但并不是每个平台的API都会封装，特别是比较个性化的API。

特别的，从内置API中可以获取当前运行的大环境（浏览器、微信小程序、阿里小程序），还可以获取当前运行的小环境（普通浏览器、微信X5、支付宝小程序、钉钉小程序）等。

可以根据运行的环境可以调用目标平台的API。


## MVVM语法支持

框架内置了MVVM，MVVM支持的指令请参考：<a href="https://github.com/nandy007/agile-ce/blob/master/docs/parser.md" target="_blank">MVVM指令</a>。

需要注意的是，上述列出的指令中，<code>v-html</code>和<code>v-xhtml</code>在小程序中不支持，仅在h5中支持。