---
layout: post
title:  "翻书效果（未完待续）"
date:   2014-10-8 13:52:00
categories: frontend
---

以前很好奇那种，比如一张图片右半边可以实现翻书效果的特效。一开始还以为是有什么CSS3的属性可以做到这点（想太多），今天自己看到一个案例还不错就弄下来了 [demo][demoSite] 。

<img src="{{site.url}}sysutangzxBlog/source/2014-10-08-book-effect-1.png">


HTML的结构非常简单，如下：


	<div class="cover">
		<div class="inner-controls">
			<ul>
				<li>
					<a href="#">
						<span class="entypo-play"></span>
					</a>
				</li>
				<li>
					<a href="#">
						<span class="entypo-download"></span>
					</a>
				</li>
				<li>
					<a href="#">
						<span class="entypo-share"></span>
					</a>
				</li>
			</ul>
		</div>
	</div>




[demoSite]:    http://cody1991.github.io/onlineTest/cssdesk/4/index.html

