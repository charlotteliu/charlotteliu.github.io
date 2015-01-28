---
layout: post
title: markdown语法总结
category：技术
tags：markdown
description：总结写博客时用到的markdown语法
---

##markdown语法总结

###标题

Markdown 支持两种标题的语法，类 Setext 和类 atx 形式。  

    this is a H1
    ============
    
    this is a H2
    ------------
    
类 Atx 形式则是在行首插入 1 到 6 个 # ，对应到标题 1 到 6 阶，例如：

    # 这是H1
    ## 这是H2
    ...
    ######这是H6

###段落和换行

一个 Markdown 段落是由一个或多个连续的文本行组成，它的前后要有一个以上的空行（空行的定义是显示上看起来像是空的，便会被视为空行。
比方说，若某一行只包含空格和制表符，则该行也会被视为空行）。普通段落不该用空格或制表符来缩进。

「由一个或多个连续的文本行组成」这句话其实暗示了 Markdown 允许段落内的强迫换行（插入换行符），这个特性和其他大部分的 text-to-HTML 格式不一样
（包括 Movable Type 的「Convert Line Breaks」选项），其它的格式会把每个换行符都转成 <br /> 标签。
如果你确实想要依赖 Markdown 来插入\<\br /> 标签的话，在插入处先按入*两个以上的空格然后回车*。

###列表

无序列表使用星号、加号或是减号作为列表标记

    *   red
    *   green
    *   blue
等同于

    +   Red
    +   Green
    +   Blue
    
等同于

    -   Red
    -   Green
    -   Blue
    
如果列表项目间用空行分开，在输出 HTML 时 Markdown 就会将项目内容用 <p> 标签包起来，举例来说：

*   Bird

*   Magic

列表项目可以包含多个段落，每个项目下的段落都必须缩进 4 个空格或是 1 个制表符：

    1.  This is a list item with two paragraphs. Lorem ipsum dolor
        sit amet, consectetuer adipiscing elit. Aliquam hendrerit
        mi posuere lectus.

        Vestibulum enim wisi, viverra nec, fringilla in, laoreet
        vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
        sit amet velit.

    2.  Suspendisse id sem consectetuer libero luctus adipiscing.
    
###区块引用

    > This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,  
    > consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.  
    > Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.  
    > 
    > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse  
    > id sem consectetuer libero luctus adipiscing.  

效果：
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,  
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.  
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.  
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse  
> id sem consectetuer libero luctus adipiscing.  

区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 > ：

    > This is the first level of quoting.
    >
    > > This is nested blockquote.
    >
    > Back to the first level.
    
效果：
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

###代码区块

要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以，例如，下面的输入：

    这是一个普通段落：

        这是一个代码区块。

效果：

这是一个普通段落：

    这是一个代码区块。
    
###分隔线
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。
你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：
    * * *

    ***

    *****
    
    - - -
    
    ---------------------------------------
    
效果：
* * *

***

*****

- - -

---------------------------------------

###链接

Markdown 支持两种形式的链接语法： 行内式和参考式两种形式。不管是哪一种，链接文字都是用 [方括号] 来标记。


*行内式*的链接，只要在方块括号后面紧接着圆括号并插入网址链接即可，
如果你还想要加上链接的 title 文字，只要在网址后面，用双引号把 title 文字包起来即可，例如：

    This is [an example](http://example.com/ "Title") inline link.
    
This is [an example](http://example.com/ "Title") inline link.


*参考式*的链接是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记：

    This is [an example][id] reference-style link.
    [id]: http://example.com/  "Optional Title Here"
    
效果：

This is [an example][id] reference-style link.

下面是一个参考式链接的范例：

    [id]: http://example.com/  "Optional Title Here"
    I get 10 times more traffic from [Google] [1] than from
    [Yahoo] [2] or [MSN] [3].

      [1]: http://google.com/        "Google"
      [2]: http://search.yahoo.com/  "Yahoo Search"
      [3]: http://search.msn.com/    "MSN Search"
      
效果：
I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"

###图片

markdown对图片的处理与链接类似，同样也允许两种样式： 行内式和参考式。

    ![Alt text](/path/to/img.jpg)

    ![Alt text](/path/to/img.jpg "Optional title")
    
实例：

    ![douban book](http://img5.douban.com/lpic/s27197149.jpg)
    
    
![douban book](http://img5.douban.com/lpic/s27197149.jpg)

文章参考：[Markdown 语法说明 (简体中文版)](http://wowubuntu.com/markdown)

