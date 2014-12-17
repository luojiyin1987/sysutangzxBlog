---
layout: post
title:  "Mobile Debug"
date:   2014-12-17 15:22:00
category: frontend
---

看到的一篇文章，主要是移动前端开发中的坑和填坑（bug and debug）。


1.设置页面的高度`height:100%;`产生的问题有页面底端和浏览器自带的导航条重合了（自带的导航条挡住了页面的底部），我们可以通过`document.documentElement.style.height = window.innerHeight + 'px';`来修复

2.安卓手机点击的时候会出现秒闪的黄色框，我们可以给一个CSS的样式来重置 `-webkit-tap-highlight-color: rgba(0, 0, 0, 0);`来解决

3.安卓手机4.0以下的CSS `:active` 伪类效果不兼容，我们可以给这个元素touch事件(touchstart/touchend/touchmove)绑定一个空匿名方法:`var element=documentgetElementsById(”btnShare”);
element.addEventListener(‘touchstart’,function(){},false);`

4.HTML5的audio元素的预加载、自动播放的有效性受操作系统、浏览器（webview）、版本等的影响，苹果官方规定必须由用户手动触发才会载入音频，那么我们捕捉一次用户输入后，让音频加载实现预加载:`document.addEventListener('touchstart', function () {document.getElementsByTagName('audio')[0].play();document.getElementsByTagName('audio')[0].pause();
});`

5.  在部分android 机型中的输入框可能会出现如图怪异的多余的浮出表单，经过观察与测试发现只有input:password类型的输入框存在，那么我们只要使用input:text类型的输入框并通过样式-webkit-text-security: disc; 隐藏输入密码从而解决。

...等等

上面几条是我想收集起来的，更多的看↓链接吧
<a href="http://tgideas.qq.com/webplat/info/news_version3/804/808/811/m579/201411/290576.shtml">原地址</a>