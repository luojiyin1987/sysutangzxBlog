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

>From 《angular.js权威指南》第一章

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

> From 《angular.js权威指南》第二章

Hello World
---

写一个Hello world是学习angular最基本途径。

    <!DOCTYPE html>
    <html ng-app>
    <head>
        <title>demo</title>
    </head>
    <body>
        <div class="container">
            <input ng-model="name" type="text" placeholder="Your name" />
            <h1>{{name}}</h1>
        </div>
        <script type="text/javascript" src="http://cody1991.github.io/angular-study/lib/angular.min.js"></script>
    </body>
    </html>

[Ch1.1 源码地址](https://github.com/cody1991/angular-study/tree/gh-pages/ch1.1)

这个案例不是最佳实践，但是可以看出最主要的思想：数据绑定。

***

angular采用创建实时模块来代替视图，而不是将数据合并进模板后更新DOM。任何一个独立视图组件中的值都是动态替换的。这个功能是angular最重要的功能之一。而实现这个功能需要我们引入angular文件，在某个DOM元素上明确设置ng-app属性即可。ng-app属性声明所有被包含的内容都输入这个angular应用，这也是我们在web应用中嵌套angular应用的原因。只有具有ng-app属性的DOM元素包含的元素才收angular影响。

自动数据绑定使我们可以将视图理解为模型状态的映射.当客户端的数据模型发生变化时，视图就能反映出这些变化，不需要写任何自定义的代码就可以工作了。在MVC的世界里，控制器可以不必当心牵扯到渲染视图的工作，这样我们就不必当心如何分离视图和控制器逻辑了，并且使测试会既简单又愉快。

angular认为某个值可能发生变化时会运行自己的事件循环来检查这个值是否变“脏”，如果该值从上次事件循环运行后发生了变化则认为该值是“脏”值，这是angular跟踪和响应应用变化的方式。这个过程叫做脏检查。

为了表示内部和内置的库函数，angular使用$来预定义对象，尽管这类似于全局的jquery对象$，但是它们没有关系。只要遇到$我们可以把它当做一个angular对象。

    注：接下来使用ng来表示angular

审查我们 [Ch1.1 源码地址](https://github.com/cody1991/angular-study/tree/gh-pages/ch1.1) 的代码，我们使用ng-model指令将内部数据模型对象($scope)中的name属性绑定在了文本输入字段上。意味着无论在文本输入字段输入了什么，都会同步到数据模型中。

数据模型对象（model object)指的是$scope对象，它是一个简单的js对象，其中的属性可以被视图访问，也可以和控制器进行交互。双向数据绑定意味着如果视图改变了某个值，数据模型会通过脏检查观察到这个变化，而如果数据模型改变了某个值，视图也会根据变化而重新渲染。

正如ng-app声明包含的元素都属于ng应用一样，DOM元素上的ng-controller声明它包含的元素都属于某个控制器。

一个简单的实例：

index.html

    <!DOCTYPE html>
    <html ng-app="myapp">
    <head>
        <title>demo</title>
    </head>
    <body>
        <div ng-controller="myController">
            <p>{{clock}}</p>
        </div>
        <script type="text/javascript" src="http://cody1991.github.io/angular-study/lib/angular.min.js"></script>
        <script type="text/javascript" src="js/common.js"></script>
    </body>
    </html>

common.js

    var myapp = angular.module('myapp', []);
    myapp.controller('myController', function($scope, $timeout) {
        var updateClock = function() {
            $scope.clock = new Date();
            $timeout(function() {
                updateClock();
            }, 1000);
        }
        updateClock();
    })
