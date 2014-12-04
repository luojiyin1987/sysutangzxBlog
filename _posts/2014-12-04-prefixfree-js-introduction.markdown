---
layout: post
title:  "Prefixfree.js Introduction"
date:   2014-12-04 13:35:00
category: frontend
---
发现好久没写博客了...

因为是专注于移动前端的开发，特别是微信端的，而又需要各自各样的动画之类的，CSS3的不少属性需要加上 -webkit- 的前缀，（比如box-shadow啦，transition啦）真心有点感觉是无用功。。。

以前就发现prefixfree.js这个，它是“一个 JavaScript 工具库，用于帮助你从 CSS 前缀的地狱中解脱出来。你编写的 CSS 代码无需填写浏览器前缀，在需要的时候，prefixfree.js 会帮助你自动添加当前浏览器需要的前缀。” （引用别人的话~~）。官方的描述是“-prefix-free lets you use only unprefixed CSS properties everywhere. It works behind the scenes, adding the current browser’s prefix to any CSS code, only when it’s needed.”

下面先给出几个链接吧~

[prefixfree官网][prefixfreeHome]

[prefixfree Github 地址][prefixfreeGit]

根据官网，草草的翻译几段话吧。

特性上，它都可以在需要的时候给`<link>`引入的CSS或者`<style>`里面的CSS属性或者行内CSS属性加上前缀；也可以在动态引入的CSS属性在需要的时候加入前缀，不过需要它们的一个插件（有兴趣可以到官网的plugins栏目下看~）；而用`jquery.css()`设置的属性也同样生效，不过也需要另外多一个插件。

特效上也有它的局限性，在CSS文件里面使用`import`引入的CSS属性不支持前缀添加（那就不要这样用了~又增加请求神马的），跨域名的CSS样式表也是不支持的，比如在本地直接打开引入了这个插件的文件，会有报错“ Cross origin requests are only supported for protocol schemes: http, data, chrome-extension, https, chrome-extension-resource.”，所以一般我会用apache来看，你也可以在官网的FAQ下看看，给chrome或者firefox浏览器添加点参数神马的来解决。另外行内的CSS属性的前缀添加在firefox < 3.6下和IE中也不是支持的很好。

DEMO？官网左上角的圆圈（或者其他一些元素）就是很好的案例了，在引入的CSS文件中都没有写前缀，但在F12控制台下可以看到添加了 -webkit- 或者 -moz- 的前缀。

而使用的方法也是非常方便，只需要引入prefixfree.js文件就够了，不需要写其他任何的东西。你可以放在任何地方，但是推荐放在最后引入的css文件的后面，我也是这样做的。

兼容性方面，官网的说法是支持“IE9+, Opera 10+, Firefox 3.5+, Safari 4+ and Chrome on desktop and Mobile Safari, Android browser, Chrome and Opera Mobile on mobile.”

更多的内容就到官网查看吧~这几天接到手上的项目我都引入这个库了，以后再也不用写前缀了，是一种解脱！

另外预告下下一篇博文的内容，就是[idangerous.swiper][swiperSite]的使用，感觉这个插件真心强大。之前有提到过的我的几个轮播插件[pagePiling][pagePilingSite]、[fullpage][fullpage]和[owl.carousel.fullpage][owl.carousel.fullpage]，或多或少存在点问题：pagePiling和fullpage更适合全屏的滚动，要改成纯轮播非全屏的会改变它很多原生的CSS代码，感觉费劲。而owl.carousel在轮播元素是图片的时候总是存在滑动到下一屏的时候图片的空白，用户体验很不好。

所以找了个新的插件idangerous.swiper，现在各种测试都过得去，而且它功能真心强大，参数和函数调用也是非常的多，在最新的项目中会使用它，如果表现不错的话就写一篇博文吧，介绍下它的使用，有兴趣的可以前往idangero.us网站观看，它们的framework7也是很强大的移动前端开发框架，一直想学可是没时间。。。

另外最近也是各种忙东西啊，写了自己最新的两个网站[recentlyProject][recentlyProjectSite]和[codyLib][codyLibSite]。

recentlyProject，写这个的缘由是想要收集起自己做过的项目，过往的就不收集了，以后面试什么的方便展示。截图如下：

<img src="{{site.url}}sysutangzxBlog/source/2014.12.04/2.png">

而codyLib是和recentlyProject配套做出来的网页，也是收集最近做的项目中使用到的HTML模板，CSS文件和JS工具库，而在新的项目需要的使用直接引入它们的绝对域名URL。（如果新的页面引入的文件，在以前访问旧的页面的时候也用到的话，cache缓存还存在的时候就可以加快页面加载速度了，和cdn类似吧，方便你我他）。截图如下：

<img src="{{site.url}}sysutangzxBlog/source/2014.12.04/1.png">

The end ~ 谢谢观看 ~ 欢迎留言 ~

中午没睡觉啊摔。。要上班了。。困=_=

<img src="{{site.url}}sysutangzxBlog/source/2014.12.04/3.jpg">

[prefixfreeHome]:http://leaverou.github.io/prefixfree/
[prefixfreeGit]:https://github.com/LeaVerou/prefixfree
[swiperSite]:http://www.idangero.us/sliders/swiper/
[fullpage]:    http://cody1991.github.io/fullpage/index.html
[owl.carousel.fullpage]: http://cody1991.github.io/owl.carousel.fullpage/index.html
[pagePilingSite]:http://cody1991.github.io/pagepiling/
[recentlyProjectSite]:http://cody1991.github.io/recentlyProject/
[codyLibSite]:http://cody1991.github.io/mylib/