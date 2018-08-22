# 区块元素
## 段落和换行

* [区块元素](#区块元素)
	* [段落和换行](#段落和换行)
* [This is an H1](#this-is-an-h1)
	* [This is an H2](#this-is-an-h2)
* [这是 H1](#这是-h1)
	* [这是 H2](#这是-h2)
					* [这是 H6](#这是-h6)
* [这是 H1](#这是-h1)
	* [这是 H2](#这是-h2)
		* [这是 H3](#这是-h3)
	* [这是一个标题。](#这是一个标题)
* [首行缩进（仅中文）](#首行缩进仅中文)
	* [方法一：](#方法一)
	* [方法二：](#方法二)
	* [方法三：](#方法三)
	* [方法四：](#方法四)

一个 Markdown 段落是由一个或多个连续的文本行组成，它的前后要有一个以上的空行（空行的定义是显示上看起来像是空的，便会被视为空行。比方说，若某一行只包含空格和制表符，则该行也会被视为空行）。普通段落不该用空格或制表符来缩进。

「由一个或多个连续的文本行组成」这句话其实暗示了 Markdown 允许段落内的强迫换行（插入换行符），这个特性和其他大部分的 text-to-HTML 格式不一样（包括 Movable Type 的「Convert Line Breaks」选项），其它的格式会把每个换行符都转成 <br /> 标签。

如果你确实想要依赖 Markdown 来插入 <br /> 标签的话，在插入处先按入两个以上的空格然后回车。

的确，需要多费点事（多加空格）来产生 <br /> ，但是简单地「每个换行都转换为 <br />」的方法在 Markdown 中并不适合， Markdown 中 email 式的 区块引用 和多段落的 列表 在使用换行来排版的时候，不但更好用，还更方便阅读。

标题
Markdown 支持两种标题的语法，类 Setext 和类 atx 形式。

类 Setext 形式是用底线的形式，利用 = （最高阶标题）和 - （第二阶标题），例如：

This is an H1
=============

This is an H2
-------------
任何数量的 = 和 - 都可以有效果。

类 Atx 形式则是在行首插入 1 到 6 个 # ，对应到标题 1 到 6 阶，例如：

# 这是 H1

## 这是 H2

###### 这是 H6
你可以选择性地「闭合」类 atx 样式的标题，这纯粹只是美观用的，若是觉得这样看起来比较舒适，你就可以在行尾加上 #，而行尾的 # 数量也不用和开头一样（行首的井字符数量决定标题的阶数）：

# 这是 H1 #

## 这是 H2 ##

### 这是 H3 ######
区块引用 Blockquotes
Markdown 标记区块引用是使用类似 email 中用 > 的引用方式。如果你还熟悉在 email 信件中的引言部分，你就知道怎么在 Markdown 文件中建立一个区块引用，那会看起来像是你自己先断好行，然后在每行的最前面加上 > ：

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
Markdown 也允许你偷懒只在整个段落的第一行最前面加上 > ：

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 > ：

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
引用的区块内也可以使用其他的 Markdown 语法，包括标题、列表、代码区块等：

> ## 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");
任何像样的文本编辑器都能轻松地建立 email 型的引用。例如在 BBEdit 中，你可以选取文字后然后从选单中选择增加引用阶层。

列表
Markdown 支持有序列表和无序列表。

无序列表使用星号、加号或是减号作为列表标记：

*   Red
*   Green
*   Blue
等同于：

+   Red
+   Green
+   Blue
也等同于：

-   Red
-   Green
-   Blue
有序列表则使用数字接着一个英文句点：

1.  Bird
2.  McHale
3.  Parish
很重要的一点是，你在列表标记上使用的数字并不会影响输出的 HTML 结果，上面的列表所产生的 HTML 标记为：

<ol>
<li>Bird</li>
<li>McHale</li>
<li>Parish</li>
</ol>
如果你的列表标记写成：

1.  Bird
1.  McHale
1.  Parish
或甚至是：

3. Bird
1. McHale
8. Parish
你都会得到完全相同的 HTML 输出。重点在于，你可以让 Markdown 文件的列表数字和输出的结果相同，或是你懒一点，你可以完全不用在意数字的正确性。

如果你使用懒惰的写法，建议第一个项目最好还是从 1. 开始，因为 Markdown 未来可能会支持有序列表的 start 属性。

列表项目标记通常是放在最左边，但是其实也可以缩进，最多 3 个空格，项目标记后面则一定要接着至少一个空格或制表符。

要让列表看起来更漂亮，你可以把内容用固定的缩进整理好：

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.
但是如果你懒，那也行：

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.
如果列表项目间用空行分开，在输出 HTML 时 Markdown 就会将项目内容用 <p> 标签包起来，举例来说：

*   Bird
*   Magic
会被转换为：

<ul>
<li>Bird</li>
<li>Magic</li>
</ul>
但是这个：

*   Bird

*   Magic
会被转换为：

<ul>
<li><p>Bird</p></li>
<li><p>Magic</p></li>
</ul>
列表项目可以包含多个段落，每个项目下的段落都必须缩进 4 个空格或是 1 个制表符：

1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.
如果你每行都有缩进，看起来会看好很多，当然，再次地，如果你很懒惰，Markdown 也允许：

*   This is a list item with two paragraphs.

    This is the second paragraph in the list item. You're
only required to indent the first line. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit.

*   Another item in the same list.
如果要在列表项目内放进引用，那 > 就需要缩进：

*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.
如果要放代码区块的话，该区块就需要缩进两次，也就是 8 个空格或是 2 个制表符：

*   一列表项包含一个列表区块：

        <代码写在这>
当然，项目列表很可能会不小心产生，像是下面这样的写法：

1986. What a great season.
换句话说，也就是在行首出现数字-句点-空白，要避免这样的状况，你可以在句点前面加上反斜杠。

1986\. What a great season.
代码区块
和程序相关的写作或是标签语言原始码通常会有已经排版好的代码区块，通常这些区块我们并不希望它以一般段落文件的方式去排版，而是照原来的样子显示，Markdown 会用 <pre> 和 <code> 标签来把代码区块包起来。

要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以，例如，下面的输入：

这是一个普通段落：

    这是一个代码区块。
Markdown 会转换成：

<p>这是一个普通段落：</p>

<pre><code>这是一个代码区块。
</code></pre>
这个每行一阶的缩进（4 个空格或是 1 个制表符），都会被移除，例如：

Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell
会被转换为：

<p>Here is an example of AppleScript:</p>

<pre><code>tell application "Foo"
    beep
end tell
</code></pre>
一个代码区块会一直持续到没有缩进的那一行（或是文件结尾）。

在代码区块里面， & 、 < 和 > 会自动转成 HTML 实体，这样的方式让你非常容易使用 Markdown 插入范例用的 HTML 原始码，只需要复制贴上，再加上缩进就可以了，剩下的 Markdown 都会帮你处理，例如：

    <div class="footer">
        &copy; 2004 Foo Corporation
    </div>
会被转换为：

<pre><code>&lt;div class="footer"&gt;
    &amp;copy; 2004 Foo Corporation
&lt;/div&gt;
</code></pre>
代码区块中，一般的 Markdown 语法不会被转换，像是星号便只是星号，这表示你可以很容易地以 Markdown 语法撰写 Markdown 语法相关的文件。

分隔线
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：

* * *

***

*****

- - -

---------------------------------------
# 首行缩进（仅中文）

markdown是老外搞的，英文没有段首缩进这个问题，但到了中文，你要是不缩进一下，看起来就很痛苦，所以，还是得缩进一下。之前想自己搞一下，结果，不伦不类。markdown本身是对一般空格忽略的，在某些格式下，空格是作为格式必要组成部分存在的，如星号后面的空格之类，四个连续空格之类。
## 方法一：
不废话了，在oschina上找到了解决方法，觉得还不错，就是

p{ white-space:pre-wrap;}

很简单吧。基本上是把空格都解决了。但是问题是对于那些大拇指经常抽搐，多敲空格的人来说，这个可能就会造成些许麻烦了。


## 方法二：
直接写
半方大的空白&ensp;或&#8194;
全方大的空白&emsp;或&#8195;
不断行的空白格&nbsp;或&#160;

## 方法三：

　Markdonw不支持行首空格缩进，以前要是想空格，我采用的方法是手动输入空格：

&nbsp;
1
1
　在逛知乎的时候，发现了这种方法：来源链接http://www.zhihu.com/question/21420126

## 方法四：
推荐全角空格，切换到全角模式下（一般的中文输入法都是按 shift + space）输入两个空格就行了。这个相对   来说稍微干净一点，而且宽度是整整两个汉字，很整齐

　　　　　　　　　试了下上面的方法，确实可以（看看这句话的前面就是这样做的）。 
　　　　　　　　　想要多少个空格，就在“全角”模式下，敲多少个空格就ＯＫ了。这种方法比我最上面的那个方法要好多了。