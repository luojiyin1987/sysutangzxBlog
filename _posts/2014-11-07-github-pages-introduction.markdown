---
layout: post
title:  "github pages introduction!"
date:   2014-11-07 14:06:40
categories: github
tags: github pages
---
github pages是用来搭建免费的，不限流量的个人网站，可以把自己的东西托管在二级域名 *.github.io 下，本教程就是来简单的说明github pages的使用。

友情链接：
[github pages 官网][githubpages]，英文网站。
[git简易指南][gitintro]，git的使用简单教程。

在看本教程前，英文水平OK的可以看看github pages的官网，另外教程中不会涉及github的使用说明，可以在上面的git简明指南中查看，所以默认你是会使用git的。

首先，进入[github.com][gitsite]，登陆以后进入到自己的个人空间，点击 Repositories ，选择 new ，创建新的git仓库。如图所示：

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/1.png">

之后这一步很重要，创建的仓库的名字一定要是 yourname.github.io 的格式，前面是你自己的github名字。接下来可以选择下面的"initialize this repository with a readme"，创建原始的readme，最后选择 "create repository"，创建仓库即可 。如图，由于我已经创建过这个 域名了，所以提示我这个仓库名已经存在。

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/2.png">

创建成功以后，会进入到自己的仓库的主页，接下来我们选择右边sidebar里面的 "settings" 选项。如图所示，当然刚创建成功的话，仓库里面只有Readmm.md一个文件。（接下来用另外一个github的账号sysutangzx来说明好了）

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/3.png">

我们进入到settings界面以后，滚动到下面的Github Pages栏。点击 Automatic page generator 按钮。如图所示：

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/4.png">

进去以后，如果没有特别需要设置的话，因为构造个人网站你不需要太多的原来github pages提供的东西，可以直接选择 Continue to layouts 按钮。如图：

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/5.png">

之后任意选择一个模板，点击Publish page按钮，你的个人网站域名就生成了。不过不要着急，大概十分钟后左右才可以访问。如图：

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/6.png">

在等待的时间，我们就可以回到原来的仓库首页去设置一下仓库的介绍了。如图：

<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/7.png">

下面就是我们原始的github pages首页了。如图：
<img src="{{site.url}}sysutangzxBlog/source/2014.11.07/8.png">

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby linenos%}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[有帮助的图片]({{site.url}}sysutangzxBlog/source/test_pic.jpg)

<img src="{{site.url}}sysutangzxBlog/source/test_pic.jpg">


[githubpages]: https://pages.github.com/
[gitintro]: http://www.bootcss.com/p/git-guide/
[gitsite]:https://github.com/
[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
