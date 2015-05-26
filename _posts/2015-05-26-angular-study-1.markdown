---
layout: post
title:  "Angular Study (1)"
date:   2015-05-26 20:12:00
category: angular
---

Angular 学习 (1) 草稿
=====================

前言：
---

接下来就跟着《angular.js权威指南》一步步来学习augular.js吧。按心情来进行分章。

这个不是一个教程，只是学习笔记，所以不系统也不完整。学习进度会很慢，但是至少踏实。

***

资源列表
---
[配套的github仓库 -- cody1991 / angular-study](https://github.com/cody1991/angular-study)
[最新稳定版本 AngularJS v1.3.15](http://cody1991.github.io/angular-study/lib/angular.min.js)

*** 

Chapter 1 (开始于《angular.js权威指南》第一章)
---

> From 《angular.js权威指南》第一章

angular.js的官网文档是这样定义它的：

>完全使用javascript编写的客户端技术。同其他历史悠久的WEB技术（HTML,CSS和javascript）配合使用，是WEB应用开发比以往更加简单。

而angular开发团队将它描叙为一种构建动态web应用的结构化框架。

angular提供了一系列高级功能，比如：

1. 解耦应用逻辑、数据模型和视图
2. ajax服务
3. 依赖注入
4. 浏览历史（书签的前进、后退按钮可以像普通web应用一样工作
5. 测试
6. 更多

*** 

angular通过原生的Model-view-controller,MVC功能增强了HTML，结果表明这样可以快捷愉悦地构造出令人印象深刻和极富表现力的客户端应用。利用它，开发者可以把页面一部分封装为一个应用，并且不强迫整个页面使用angular开发。这个特性在某些情况下非常有用：比如工作流程中已经包含另外一个框架，或者希望页面中某一部分是动态的，而其他部分是静态或者由其他js框架来控制的时候。

angular压缩以后不会付出太大的额外代价，上面提到的 [最新稳定版本 AngularJS v1.3.15](http://cody1991.github.io/angular-study/lib/angular.min.js) ,大小只有123KB，非常适合开发功能原型。



