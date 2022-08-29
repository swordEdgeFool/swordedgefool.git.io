---
title: 排版
layout: post
categories: [Typography, Markdown]
image: /assets/img/rose.jpg
description: "Basic typography and styling for your posts."
customexcerpt: "主题的一些基础文本样式和格式."
---
Reference: [GitHub flavored Markdown](https://help.github.com/en/github/writing-on-github).

* random line to make it work. This will be removed.
{:toc}



## 样式文本
**加粗**
{% highlight markdown %}
**加粗**
{% endhighlight %}

*斜体*
{% highlight markdown %}
 *斜体*
{% endhighlight %}

~~加删除线~~
{% highlight markdown %}
~~加删除线~~
{% endhighlight %}

***加粗斜体***
{% highlight markdown %}
***加粗斜体***
{% endhighlight %}

## 引用
>This is a quote
{% highlight markdown %}
>This is a quote
{% endhighlight %}

>This is a quote with author   
><cite><a href="#">The author</a></cite>

{% highlight markdown %}
>This is a quote with author  
><cite><a href="#">The author</a></cite>
{% endhighlight %}

## 链接
主题设计来自 [Alessio Franceschi](https://alessiofranceschi.me).
{% highlight markdown %}
Theme designed by [Alessio Franceschi](https://alessiofranceschi.me).
{% endhighlight %}

链接也可以来自自我引用跳转. [Like this one](/contact.html).
{% highlight markdown %}
Links can also be relative. [Like this one](/contact.html).
{% endhighlight %}

## 列表
unordered:
- this
- is
- unordered
{% highlight markdown %}
- this
- is
- unordered
{% endhighlight %}  

Ordered:
1. but
2. this
3. is
4. ordered
{% highlight markdown %}
1. but
2. this
3. is
4. ordered
{% endhighlight %}  

嵌套:
1. First point
    - but also this
    - and also this
        - and this one too
2. Second point
{% highlight markdown %}
1. First point
    - but also this
    - and also this
        - and this one too
2. Second point
{% endhighlight %}  


## 任务列表
- [x] Write some CSS 
- [ ] Fix bugs
- [ ] Add related posts
{% highlight markdown %}
- [x] Write some CSS 
- [ ] Fix bugs
- [ ] Add related posts
{% endhighlight %}  

## 语法高亮
[瞅这](/tips/markdown/排版/2020/05/19/special-formatting.html#syntax-highlight).

## MathJAX 和LaTeX
[瞅这](/tips/markdown/排版/2020/05/19/special-formatting.html#mathjax-and-latex).

## Alerts
[瞅这](/tips/markdown/排版/2020/05/19/special-formatting.html#alerts).

## 标题

# 大一点的标题
## 小一点的标题
###### 最小的标题


{% highlight markdown %}
# 大一点的标题
## 标题
###### 最小的标题
{% endhighlight %}