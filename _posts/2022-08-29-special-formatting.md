---
title: 特殊的格式
layout: post
categories: [Tips, Markdown, 排版]
image: /assets/img/forest-snow.jpg
description: "一些关于如何设置文本格式的技巧."
customexcerpt: "让你更快上手这个主题还有这些精细配置"
---
在这篇文章中，将展示这个主题的一些“特殊”功能。

我们从目录开始.

### 目录
* random line to make it work. This will be removed.
{:toc}

Code:
### 语法高亮
在YAMT中，您可以以各种方式突出显示代码.

Basic example:
``` java
public static void main (String[] args){
    System.out.println("Hello World!");
}
```
Code:

``` 
    `` lang
        //你的代码
        
```
```    
<br>

Example:
{% highlight java %}
public static void main (String[] args){
    System.out.println("Hello World!");
}
{% endhighlight %}
Code:
```
    {/% highlight lang %}
        //your code 
    {/% endhighlight java %}
    //把这个 "/" 还有这个 "java"换到上面的lang 拿掉就能显示了.
```

<br>

显示行号:
{% highlight java linenos%}
public static void main (String[] args){
    System.out.println("Hello World!");
}
{% endhighlight %}
例子如下:
```
    {/% highlight lang linenos%}
        //your code 
    {/% endhighlight java %}
    //把这个 "/" 还有这个 "java"换到上面的lang 拿掉就能显示了.
```

<br>

如果整太多了，可以添加水平滚动条:
{% highlight java linenos%}
public static void main (String[] args){
    System.out.println("Hello World! This is a very long line of code, perharps too long...");
}
{% endhighlight %}

<br>
ruby这个语言也可以用用: [Rouge Wiki](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers).

**Note**: In /assets/css/syntax.  css这个文件里面的第一个声明可以选择是否需要滚到条或者文本换行！

### MathJAX and LaTeX
咱们可以使用LaTeX和MathJax来编写数学公式啥的，有三种写数学公式的方法，下面是用伯努利原理写的一个小例子.
>在流体动力学中，伯努利原理指出 
>流体的速度与静压或流体势能的降低同时发生.具体可以看看这个网址  
><cite><a href="https://en.wikipedia.org/wiki/Bernoulli%27s_principle">Wikipedia</a></cite>  


模板1:  

$$  \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant $$
{% highlight tex %}
$$  \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant $$
{% endhighlight %}

连续模式lnline: $$  \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant $$
{% highlight tex %}
$$  \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant $$
{% endhighlight %}  

另一种模板:
\\[ \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant \\]
{% highlight tex %}
\\[ \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant \\]
{% endhighlight %}  

另一种连续模式lnline: \\( \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant \\)
{% highlight tex %}
\\( \frac{v^2} {2} + {g}{z} + \frac{p} {ρ} = constant \\)
{% endhighlight %}  


### 警报样式
<span class = "alert r">Warning!</span>
​``` html
<span class = "alert r"></span>
```
<span class = "alert g">Solved.</span>
``` html
<span class = "alert g"></span>
```
<span class = "alert y">Careful.</span>
``` html
<span class = "alert y"></span>
```

### 动图
这个主题可以使用优化过的gif，建议使用这个网站 [Convertio](https://convertio.co/it/) 把你的gif图片转换成webM或者Mp4格式的 webM是建议格式，所以把Mp4当作一种备用 把这两种都放在gif文件夹种，并在你的帖子种插入gif

``` liquid
{_% include gif.html file = "mygif" %}
```
删除下划线，就可以让上面这段代码运行起来了。

如果您想使用gif作为特色图像，删除“图像”标签在前面的事项，并使用“gif”标签代替。作为参数，使用不带扩展名的文件名。.