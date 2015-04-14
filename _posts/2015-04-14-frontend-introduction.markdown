---
layout: post
title:  "Seajs Study"
date:   2015-04-14 23:34:00
category: frontend
---

前端开发入门
================

基本所有想要进入前端开发领域的人问前端开发人员如何入门的时候，得到的答案都是看w3cschool（ http://www.w3school.com.cn/ ）。就个人感觉而言，w3cschool确实是一个对前端完全没有了解的人一个好的入门去向，它主要的优点是浅显但又完整地向初学者展现了前端最需要掌握的基础知识：HTML，CSS以及javascript。打开网站以后从HTML教程进入，你就打开前端开发的大门（大坑）了。建议的是HTML,HTML5,XHTML,CSS,CSS3一次性读完下来，对基础知识的HTML和CSS有了大概的了解以后，就可以开始找找书籍来进一步学习。


HTML和CSS的书籍其实很多很多，当时在学习的时候也是东看西看的。很多人推荐的第一本HTML和CSS的书籍是《Head first HTML & CSS》，称为最好的入门书。而第二本推荐的推荐的是《CSS权威指南（第三版）》，非常权威的一本CSS的书籍，可以不断翻阅进行学习。而接下来第三本是《精通CSS》，广受前辈推荐的一本书，汇集了不少的CSS的最佳实践。而最后推荐一本比较新的书，《图解CSS3：核心技术和案例实践》，涉及到了最新的CSS3的很多新的属性。前面没有专门提到HTML的书籍，因为单纯的HTML其实在w3cschool就基本了解完毕了，最新的HTML5提供的许多新标签和新的API等等，就不是这个阶段的学习资料了。而上面提到的一些书籍年限比较久远，但是觉得那些最基本的CSS属性一直都是稳定下来了的，看这些书完全可以很好地掌握CSS。当然还有很多非常的CSS书籍。下面提供一个不错的网址，里面提供了很多前端开发书籍的下载：http://www.w3cfuns.com/feres.php?do=picture&listtype=book 。


接下来说说基础知识的javascript部分。这个也是这篇文章比较纠结的地方，是推荐先学javascript还是学习jquery好。原生javascript是一个前端开发人员水平的最主要的评价标准。你原生javascript厉害才能真正的登堂入室，称得上一个比较牛的前端开发工程师。它是一门编程语言，学习曲线也是比较曲折，而学好学精更是难上加难。所以想要比较快速的入门前端开发，能写得出页面和交互，不少人推荐的是jquery框架的学习，而往往很多人学习完jquery以后太过于依赖而没有回归本质学习javascript，对于闭包，原型链，浏览器兼容性问题，继承等等javascript的核心理念都没有认识到。上面说了很多，具体的学习路线就看你自己怎么想了。


Javascript的入门书籍我是比较推荐《javascript DOM编程艺术》的，很好的一本入门书籍，也有符合标准的编程理念，能让你比较轻松地入门javascript。接下来javascript的必读书籍（没有之一）就是《javascript高级编程设计》，这本书籍就是javascript界的一本圣经，非常全面完整权威的展示了javascript又有不少的实际代码可以让读者去实践。而往后的学习推荐《javascript语言精粹》，这书很薄，却是一本让你把javascript写得更完美的不可多得的好书。而学习完javascript，很重要的一点就是要去学习ajax（其实ajax也是javascript的一部分），可以看看《Head First Ajax》进行了解，以及w3cscholl上面也有讲解到，它是我们和后台开发人员进行数据交互不可缺少的一门技巧。


上面提到的jquery，它的介绍就不多说了，一搜一大把。它的入门推荐书籍是《锋利的jquery》，我很喜欢的一本jquery的入门书籍，讲解的非常详细，而且也有不少的案例可以让你进行学习。但是千万别忘了原生的javascript才是前端开发工程师最重要的技能，没有之一。


经过上面几个阶段的学习，基本可以完成企业里面平常的前端开发任务了，这个时候可以去看看高性能网站建设指南及其续篇《高性能网站进阶》，两本非常不错的书籍，可以让你更好地去优化自己创建出来的前端网站。而其实到了这个阶段，你也是基本知道如何去学习和进阶自己的前端开发水平了。


接下来说说如今前端比较热门的框架，当然只是局限于我自己的认识，毕竟在前端开发领域我也只是个菜鸟，还有很多需要学习和深入的地方。后面的部分就是前端开发工程师进阶的个人建议。


Bootstrap，应该是如今最火爆的的前端框架之一了。官网（ http://www.bootcss.com/ ）对它的概括是：简洁、直观、强悍的前端开发框架，让web开发更迅速、简单。它确实也是最近几年基本每个公司都要求前端开发人员掌握的框架之一。其他的就不多说了，提供了很好的兼容性，不错的UI界面以及不少的javascript组件，让一个网站建造起来非常的简单和容易。而且官网的文档非常的详细，把文档看一遍基本就会使用了。另外还有非常多的这样的前端框架，在需要的时候可以一一的去了解，它们学习曲线都很简单。


也许你会被很多重复的CSS代码以及前缀问题所烦恼，Less（SASS等）赋予了CSS动态语言的特性，如变量，继承，运算，函数等等，并且即可以在客户端运行（支持IE6+,Webkit,Firefox)，也可以借助Node.js或者Rhino在服务器运行。这也是我最近用来预处理CSS的主要工具之一，它的官方文档是 http://www.bootcss.com/p/lesscss/ ，你会喜欢上它的。而coffeescript我仅仅是了解并编写了一些案例，它能把javascript写得非常优雅，具体的就不多说了毕竟不是非常了解，免得误人子弟。中文官网网站： http://coffee-script.org/ 。


也许有时候你只是编写简单的前端开发，但是企业站等等页面代码的不断增加，开发人员的不断增多，代码逻辑方面可能越来越混乱，这个时候就需要提供模块化的开发环境了。Sea.js是本人这方面学习并且使用的框架，它的官方地址是： http://seajs.org/docs/ ，另外和它类似的就是require.js（ http://requirejs.org/ ）。选择哪个你可以都充分地阅读它们的文档以后进行学习。为什么使用sea.js？正如官网所说的，追求简单、自然的代码书写和组织方式，它也具有以下的核心特性：简单友好的模块定义规范，遵守着CMD规范并且像node.js一样书写模块代码，而第二点是自然直观的代码组织方式，依赖的自动加载、配置的简洁明晰。


随着前端开发越来越多的数据处理，或者为了更好地分离页面结构和数据，或者是编写单页的应用，MVC，MVVM框架不断涌现。Backbone.js, avalon.js本人都是读了官网文档进行了解，最后选择angular.js来进行学习。毕竟还在学习阶段，这里提提也是提供一个学习方向而已，而推荐的书籍是《angular权威教程》。


而前端开发工程师的继续进阶路线可能是往全栈工程师发展，学习后台开发语言PHP，PYTHON？其实不然，完全可以继续沿用我们学习的javascript，出现了新的一门热火朝天的 node.js ，用javascript来写服务端。Nodejs的学习资源非常多，个人比较推荐的是《node.js实战》


正如上面所说的，随着前端项目的文件结构越来越复杂，以及我们在一个项目完成以后需要进行不少的工作，比如javascript，css文件的合并和压缩，图片的整合和压缩，less等预处理语言的处理等等，我们非常迫切需要有工具来管理我们的文件。这里我自己进行选择的是gulp.js框架（ http://www.gulpjs.com.cn/ ），官方的说明是：用自动化构建工具增强你的工作流程。有另外一个也非常火的框架是grunt （ http://www.gruntjs.net/ ）。个人一开始选择gulp的理由是学习起来比较容易而功能非常强大。学习的话书籍方面的资料肯定不多，在网上进行搜索以及查看官网文档就能不错的入门了。


最后再说一些自己的想法吧。


Github （ https://github.com/ ）是前端学习非常好的一个地方，当然它也是很多编程语言学习的好地方。上面有非常多的开源项目，创建属于自己的一个github账号并且不断地收集不错的前端开发资源，并适当地进行模仿它们的代码编写，发展的空间非常大。个人的github是 https://github.com/cody1991 ，关注了不少的优秀项目，也有自己经常更新的个人前端项目（比如个人简历，个人博客等等）。


Codrops ( http://tympanus.net/codrops/ )是个人非常喜欢的一个外国前端博客。上面有非常多非常不错的前端开发项目，使用了非常多前沿的技术，页面交互也非常酷炫和友好，另外每个项目的代码也是开源的非常容易下载来学习。外国的前端开发水平是非常高的，甚至不少前端开发人员的薪水高于后端，而且很有开源的精神，存在不少非常优秀的前端博客。把英语学好，常常去阅读它们，肯定是你前端进阶非常好的一个手段。


一个前端开发大牛的博客： http://www.cnblogs.com/jikey/ ，感觉他在资源收集方面真的做的非常好，可以认真的看看他的博文来进行资源的收集和学习。 http://www.cnblogs.com/jikey/p/4426105.html 而他所创建的QQ群里面的前端技术讨论氛围也是非常棒的，可以进入和同行的人交流学习。另外非常建议阅读它所创建的群的群规： http://note.youdao.com/share/?id=8a777eda4842aa0f3d7fc6161577ab9b&type=note ，你可以在里面比较条例清理的收集自己想要的资源。


最后的最后，推荐一个非常不错的github库： https://github.com/foru17/front-end-collect ，里面真的收集了非常非常多的资源。另外就是自己最近收集的不少电子书和资料： http://yun.baidu.com/share/link?shareid=1197836167&uk=1443668030 。











	


今天学习了下sea.js，简单的写了一个[demo](http://cody1991.github.io/seajs-study/mydemo/)，下面给出它各部分的代码结构：


	<!doctype html>
	<html>
	<head>
    	<title></title>
    	<meta charset="utf-8" />
	</head>
	<body>
    	<div id="content">
        	<p class="author"></p>
        	<p class="blog">
            	<a href="#">Blog</a>
        	</p>
    	</div>
    	<script src="./app/lib/sea.js"></script>
    	<script src="./app/lib/seajs-css.js"></script>
    	<script>
    	seajs.config({
        	base:'./app/',
        	alias:{
            	'style':'../style/style.css'
        	},
        	charset: 'utf-8'
    	})
    	seajs.use('init');
    	</script>
	</body>
	</html>

可以看到HTML部分只有一个简单的div#content，里面包含着作者名字和博客名和地址。而sea.js当然也和普通的javascript文件是通过script引入的。

接下来发现我们下面还引入了一个seajs-css.js，因为我引入的sea.js是最新的版本3.0，而根据seajs-css.js [github库](https://github.com/seajs/seajs-css)的说明：

	在Sea.js < 2.3.0版本之前是可以加载css文件的，新版本中此功能移除，为了兼容考虑，加载css功能将作为一个插件存在。

	使用方法
	可以在sea.js标签后引入这个插件使用，也可以将插件代码混入sea.js当中

可以知道这个文件是用来处理引入的 css 文件

我们继续往下看，下面的seajs.config是seajs的全局配置，接收一个表示全局配置的配置对象，比如下面的例子：

	seajs.config({
	    base: 'path/to/jslib/',
	    alias: {
	      'app': 'path/to/app/'
	    },
	    charset: 'utf-8',
	    timeout: 20000,
	    debug: false
	});

其中base表示基址寻址时的基址路径。例如base设置为 

	http://example.com/js/3-party/
则:

	var $ = require('jquery');

会载入 

	http://example.com/js/3-party/jquery.js 

而alias可以对较长的常用路径设置缩写

charset表示下载js时script标签的charset属性

timeout表示下载文件的最大时长，以毫秒为单位

debug表示是否工作在调试模式下

最后就是解释下：

	seajs.use('init');

因为我们上面已经设置了基路径，所以这里写init，它会自动需找 

	./app/

下面的init.js文件。没错， seajs.use和后面会提到的require.js引入javascript文件的时候都是不需要写上.js的。而seajs.use主要用于载入入口模块。入口模块相当于C程序的main函数，同时也是整个模块依赖树的根。seajs.use用法如下：

	//单一模式
	seajs.use('./a');
	
	//回调模式
	seajs.use('./a', function(a) {
	  a.run();
	});
	
	//多模块模式
	seajs.use(['./a', './b'], function(a, b) {
	  a.run();
	  b.run();
	});

接下来我们看看我们的入口 init.js 是怎么书写的：

	define(function(require, exports, module) {
	    var $ = require('lib/jquery');
	    var data = require('data');
	    var css = require( 'style');
	
	    $('.author').html(data.author);
	    $('.blog').find('a').attr('href',data.blog);
	    console.log($('.blog').attr('href'))
	});

我们下面来说下seajs的思想。使用SeaJS开发JavaScript的基本原则就是：一切皆为模块。引入SeaJS后，编写JavaScript代码就变成了编写一个又一个模块，SeaJS中模块的概念有点类似于面向对象中的类——模块可以拥有数据和方法，数据和方法可以定义为公共或私有，公共数据和方法可以供别的模块调用。

另外，每个模块应该都定义在一个单独js文件中，即一个对应一个模块。

下面介绍模块的编写和调用。我们来看看seajs里面的模块定义函数define

	/**
	* Defines a module.
	* @param {string=} id The module id.
	* @param {Array.|string=} deps The module dependencies.
	* @param {function()|Object} factory The module factory function.
	*/
	fn.define = function(id, deps, factory) {
	    //code of function…
	}

define可以接收的参数分别是模块ID，依赖模块数组及工厂函数。define对于不同参数个数的解析规则如下：

如果只有一个参数，则赋值给factory。

如果有两个参数，第二个赋值给factory；第一个如果是array则赋值给deps，否则赋值给id。

如果有三个参数，则分别赋值给id，deps和factory。

但是，包括SeaJS的官方示例在内几乎所有用到define的地方都只传递一个工厂函数进去，类似与如下代码：

	define(function(require, exports, module) {
	    //code of the module...
	});

遵循SeaJS官方示例的标准，用一个参数的define定义模块。那么id和deps会怎么处理呢？

id是一个模块的标识字符串，define只有一个参数时，id会被默认赋值为此js文件的绝对路径。如example.com下的a.js文件中使用define定义模块，则这个模块的ID会赋值为 http://example.com/a.js ，没有特别的必要建议不要传入id。

deps一般也不需要传入，需要用到的模块用require加载即可。

------------------

下面来看看工厂函数factory解析：

工厂函数是模块的主体和重点。在只传递一个参数给define时（推荐写法），这个参数就是工厂函数，此时工厂函数的三个参数分别是：

1.require——模块加载函数，用于记载依赖模块。

2.exports——接口点，将数据或方法定义在其上则将其暴露给外部调用。

3.module——模块的元数据。

这三个参数可以根据需要选择是否需要显示指定。下面说一下module。

module是一个对象，存储了模块的元信息，具体如下：

1.module.id——模块的ID。

2.module.dependencies——一个数组，存储了此模块依赖的所有模块的ID列表。

3.module.exports——与exports指向同一个对象。

我们来看看三种不同模式的定义方法：

第一种定义模块的模式是基于exports的模式：

	define(function(require, exports, module) {
	    var a = require('a'); //引入a模块
	    var b = require('b'); //引入b模块
	
	    var data1 = 1; //私有数据
	
	    var func1 = function() { //私有方法
	        return a.run(data1);
	    }
	
	    exports.data2 = 2; //公共数据
	
	    exports.func2 = function() { //公共方法
	        return 'hello';
	    }
	});

上面是一种比较“正宗”的模块定义模式。除了将公共数据和方法附加在exports上，也可以直接返回一个对象表示模块，如下面的代码与上面的代码功能相同：

	define(function(require) {
	    var a = require('a'); //引入a模块
	    var b = require('b'); //引入b模块
	
	    var data1 = 1; //私有数据
	
	    var func1 = function() { //私有方法
	        return a.run(data1);
	    }
	
	    return {
	        data2: 2,
	        func2: function() {
	            return 'hello';
	        }
	    };
	});

如果模块定义没有其它代码，只返回一个对象，还可以有如下简化写法：

	define({
	    data: 1,
	    func: function() {
	        return 'hello';
	    }
	});

第三种方法对于定义纯JSON数据的模块非常合适。


而模块的载入和引用又是怎样的呢？

上文说过一个模块对应一个js文件，而载入模块时一般都是提供一个字符串参数告诉载入函数需要的模块，所以就需要有一套从字符串标识到实际模块所在文件路径的解析算法。SeaJS支持如下标识：

绝对地址——给出js文件的绝对路径。
如:

	require("http://example/js/a");

就代表载入 http://example/js/a.js 。

相对地址——用相对调用载入函数所在js文件的相对地址寻找模块。
例如在 

	http://example/js/b.js 

中载入

	require("./c");

则载入 http://example/js/c.js 。

基址地址——如果载入字符串标识既不是绝对路径也不是以”./”开头，则相对SeaJS全局配置中的“base”来寻址，上面已经讨论过了。

上面在载入模块时都不用传递后缀名“.js”，SeaJS会自动添加“.js”。但是下面三种情况下不会添加：

载入css时，如:

	require("./module1-style.css");

路径中含有”?”时，如:

	require(<a href="http://example/js/a.json?cb=func">http://example/js/a.json?cb=func</a>);

路径以”#”结尾时，如:

	require("http://example/js/a.json#");

根据应用场景的不同，SeaJS提供了三个载入模块的API，分别是seajs.use，require和require.async。前两者已经提到过，我们再来看看最后的require.async函数：

如果想要某个js文件在用到时才下载，可以使用require.async：

	require.async('/path/to/module/file', function(m) {
	    //code of callback...
	});

这样只有在用到这个模块时，对应的js文件才会被下载，也就实现了JavaScript代码的按需加载。

我们回归到我们的案例，在这里再次贴出代码：

	define(function(require, exports, module) {
	    var $ = require('lib/jquery');
	    var data = require('data');
	    var css = require( 'style');
	
	    $('.author').html(data.author);
	    $('.blog').find('a').attr('href',data.blog);
	    console.log($('.blog').attr('href'))
	});

可以看到我们使用的定义模式，在这个函数里面我们首先引入了jquery.js文件。但是一开始的时候发现，使用console.log($)返回的一直都是 null ，百思不得其解，最后上网查了下看到了这篇文章：[传送门:seajs初尝 加载jquery返回null解决学习日志](http://www.tuicool.com/articles/bmuaEb)。里面已经非常详细地说明了原因。而我也是在jquery.js的文件里面进行了下面的修改：

	define(function(){
	    //jquery源代码
	    return $.noConflict();
	});

另外我们还引入了data.js文件，它的结构代码很简单：

	define({
		author:'ZhangYang',
		blog:'http://cody1991.github.io/sysutangzxBlog/'
	})

返回给data变量的值是一个类似json的结构。最后就是使用jquery方法进行操作了，没什么好说的。

sea.js还有很多方法的使用，这篇文章只是看了一些资料，弄了一个demo，然后总结出来的笔记。大概已经找到了 sea.js 的敲门砖。后面还会继续需找资料，力求熟悉使用sea.js并且能用到实际项目中。谢谢！