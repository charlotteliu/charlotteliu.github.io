---
layout: post
title: markdown�﷨�ܽ�
category������
tags��markdown
description���ܽ�д����ʱ�õ���markdown�﷨
---

##markdown�﷨�ܽ�

###����

Markdown ֧�����ֱ�����﷨���� Setext ���� atx ��ʽ��  

    this is a H1
    ============
    
    this is a H2
    ------------
    
�� Atx ��ʽ���������ײ��� 1 �� 6 �� # ����Ӧ������ 1 �� 6 �ף����磺

    # ����H1
    ## ����H2
    ...
    ######����H6

###����ͻ���

һ�� Markdown ��������һ�������������ı�����ɣ�����ǰ��Ҫ��һ�����ϵĿ��У����еĶ�������ʾ�Ͽ��������ǿյģ���ᱻ��Ϊ���С�
�ȷ�˵����ĳһ��ֻ�����ո���Ʊ���������Ҳ�ᱻ��Ϊ���У�����ͨ���䲻���ÿո���Ʊ����������

����һ�������������ı�����ɡ���仰��ʵ��ʾ�� Markdown ��������ڵ�ǿ�Ȼ��У����뻻�з�����������Ժ������󲿷ֵ� text-to-HTML ��ʽ��һ��
������ Movable Type �ġ�Convert Line Breaks��ѡ��������ĸ�ʽ���ÿ�����з���ת�� <br /> ��ǩ��
�����ȷʵ��Ҫ���� Markdown ������\<\br /> ��ǩ�Ļ����ڲ��봦�Ȱ���*�������ϵĿո�Ȼ��س�*��

###�б�

�����б�ʹ���Ǻš��ӺŻ��Ǽ�����Ϊ�б���

    *   red
    *   green
    *   blue
��ͬ��

    +   Red
    +   Green
    +   Blue
    
��ͬ��

    -   Red
    -   Green
    -   Blue
    
����б���Ŀ���ÿ��зֿ�������� HTML ʱ Markdown �ͻὫ��Ŀ������ <p> ��ǩ��������������˵��

*   Bird

*   Magic

�б���Ŀ���԰���������䣬ÿ����Ŀ�µĶ��䶼�������� 4 ���ո���� 1 ���Ʊ����

    1.  This is a list item with two paragraphs. Lorem ipsum dolor
        sit amet, consectetuer adipiscing elit. Aliquam hendrerit
        mi posuere lectus.

        Vestibulum enim wisi, viverra nec, fringilla in, laoreet
        vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
        sit amet velit.

    2.  Suspendisse id sem consectetuer libero luctus adipiscing.
    
###��������

    > This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,  
    > consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.  
    > Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.  
    > 
    > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse  
    > id sem consectetuer libero luctus adipiscing.  

Ч����
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,  
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.  
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.  
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse  
> id sem consectetuer libero luctus adipiscing.  

�������ÿ���Ƕ�ף����磺�����ڵ����ã���ֻҪ���ݲ�μ��ϲ�ͬ������ > ��

    > This is the first level of quoting.
    >
    > > This is nested blockquote.
    >
    > Back to the first level.
    
Ч����
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

###��������

Ҫ�� Markdown �н�����������ܼ򵥣�ֻҪ�򵥵����� 4 ���ո���� 1 ���Ʊ���Ϳ��ԣ����磬��������룺

    ����һ����ͨ���䣺

        ����һ���������顣

Ч����

����һ����ͨ���䣺

    ����һ���������顣
    
###�ָ���
�������һ�������������ϵ��Ǻš����š�����������һ���ָ��ߣ����ڲ���������������
��Ҳ�������ǺŻ��Ǽ����м����ո�����ÿ��д�������Խ����ָ��ߣ�
    * * *

    ***

    *****
    
    - - -
    
    ---------------------------------------
    
Ч����
* * *

***

*****

- - -

---------------------------------------

###����

Markdown ֧��������ʽ�������﷨�� ����ʽ�Ͳο�ʽ������ʽ����������һ�֣��������ֶ����� [������] ����ǡ�


*����ʽ*�����ӣ�ֻҪ�ڷ������ź��������Բ���Ų�������ַ���Ӽ��ɣ�
����㻹��Ҫ�������ӵ� title ���֣�ֻҪ����ַ���棬��˫���Ű� title ���ְ��������ɣ����磺

    This is [an example](http://example.com/ "Title") inline link.
    
This is [an example](http://example.com/ "Title") inline link.


*�ο�ʽ*�����������������ֵ����ź����ٽ�����һ�������ţ����ڵڶ�������������Ҫ�������Ա�ʶ���ӵı�ǣ�

    This is [an example][id] reference-style link.
    [id]: http://example.com/  "Optional Title Here"
    
Ч����

This is [an example][id] reference-style link.

������һ���ο�ʽ���ӵķ�����

    [id]: http://example.com/  "Optional Title Here"
    I get 10 times more traffic from [Google] [1] than from
    [Yahoo] [2] or [MSN] [3].

      [1]: http://google.com/        "Google"
      [2]: http://search.yahoo.com/  "Yahoo Search"
      [3]: http://search.msn.com/    "MSN Search"
      
Ч����
I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"

###ͼƬ

markdown��ͼƬ�Ĵ������������ƣ�ͬ��Ҳ����������ʽ�� ����ʽ�Ͳο�ʽ��

    ![Alt text](/path/to/img.jpg)

    ![Alt text](/path/to/img.jpg "Optional title")
    
ʵ����

    ![douban book](http://img5.douban.com/lpic/s27197149.jpg)
    
    
![douban book](http://img5.douban.com/lpic/s27197149.jpg)

���²ο���[Markdown �﷨˵�� (�������İ�)](http://wowubuntu.com/markdown)

