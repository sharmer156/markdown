
#  [原来Github上的README.md文件这么有意思——Markdown语言详解](http://www.cnblogs.com/manyiString/p/6803071.html) #

<div class="postBody">

<div id="cnblogs_post_body" class="blogpost-body">

 转载请注明出处：[http://blog.csdn.net/zhaokaiqiang1992](http://blog.csdn.net/zhaokaiqiang1992)

之前一直在使用github，也在上面分享了不少的项目和Demo，每次创建新项目的时候，使用的都是默认的README.md文件，也不曾对这个文件有过什么了解。但是在看到别人写的项目的README.md里面竟然有图片、链接什么的，就感到很好奇，这效果是什么加上去的？于是便查了一下资料，结果，竟迁出了一门从来没有了解过的语言— —Markdown！

    github上的README.md文件就是使用的Markdown语言编写的，我们先简单介绍下这门语言的来龙去脉，然后再介绍一些基本的语法和使用。

#     1.来龙去脉和语法特点

    Markdown 是一种轻量级标记语言，创始人为约翰·格鲁伯（John Gruber）。它允许人们“使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或者HTML)文档”。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。

   Markdown 的目标是实现「易读易写」。可读性，无论如何，都是最重要的。一份使用 Markdown 格式撰写的文件应该可以直接以纯文本发布，并且看起来不会像是由许多标签或是格式指令所构成。Markdown 语法受到一些既有 text-to-HTML 格式的影响，包括Setext、atx、Textile、reStructuredText、Grutatext 和 EtText，而最大灵感来源其实是纯文本电子邮件的格式。总之， Markdown 的语法全由一些符号所组成，这些符号经过精挑细选，其作用一目了然。比如：在文字两旁加上星号，看起来就像*强调*。Markdown 的列表看起来，嗯，就是列表。Markdown 的区块引用看起来就真的像是引用一段文字，就像你曾在电子邮件中见过的那样。

    Markdown 语法的目标是：成为一种适用于网络的书写语言。Markdown 不是想要取代 HTML，甚至也没有要和它相近，它的语法种类很少，只对应 HTML 标记的一小部分。Markdown 的构想不是要使得 HTML 文档更容易书写。在我看来， HTML 已经很容易写了。Markdown 的理念是，能让文档更容易读、写和随意改。HTML 是一种发布的格式，Markdown 是一种书写的格式。就这样，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

    正是因为Markdown的这些特点，而且功能比纯文本更强，因此有很多人用它写博客。世界上最流行的博客平台WordPress和大型CMS如joomla、drupal都能很好的支持Markdown。

#           2.编辑软件

<div>    如果我们要写Markdown代码的话，我们首先需要一个编辑器，因为我使用的是Mac，所以推荐使用Mou，非常的强大，非常的好用。</div>

<div>    下面是Mou的界面，左边是Markdown代码，右边是实时的展示效果，而且可以选择不同的主题色，非常的漂亮！</div>

<div>!![](http://img.blog.csdn.net/20141121162048979?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvemhhb2thaXFpYW5nMTk5Mg==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)</div>

<div>    当然，如果你使用的是其他的平台的话，你可以选择在线的编辑器，效果也非常棒。</div>

<div>    给出两个在线的Markdown编辑器</div>

<div>    [http://mahua.jser.me/](http://mahua.jser.me/)</div>

<div>    [http://maxiang.info/](http://maxiang.info/)</div>

<div>    第一个是个人开发的，免费使用，非常赞！</div>

<div>    第二个是一个已经发布的产品，可以免费在线编辑。除此之外，还可以将内容同步到印象笔记，不过只能试用10天，之后需要79/年，还是非常不错的。</div>

#     3.常用语法介绍

<div>      这里只介绍最常用和最常见的功能，若想查看全部的语法，请移步[http://wowubuntu.com/markdown/index.html](http://wowubuntu.com/markdown/index.html)</div>

<div>（1）标题</div>

<div>    标题使用不同数量的"#"来标识是什么层级，可以对应于HTML里面的H1-H6，下面是示例代码和效果</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121163201450)</div>

<div>    “========”风格的也可以，但是我不喜欢，赶不上"#"的好用</div>

<div>   （2）图片</div>

<div>    我们可以使用下面的语法，添加一个图片</div>

<div>    ![Alt text](/path/to/img.jpg)</div>

<div>    详细叙述如下：
    一个惊叹号 !
    接着一个方括号，里面放上图片的替代文字
    接着一个普通括号，里面放上图片的网址</div>

<div>    下面是一个示例</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121163821625)</div>

<div>    （3）强调</div>

<div>    我们可以使用下面的方式给我们的文本添加强调的效果</div>

<div>*强调* 或者 _强调_  (示例：斜体)
**加重强调** 或者 __加重强调__ (示例：粗体)
***特别强调*** 或者 ___特别强调___ (示例：粗斜体)</div>

<div>    下面是一个示例：</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121164141381)</div>

<div>    （4）代码</div>

<div>    如果我们想在文章中添加代码，我们有两种方式</div>

<div>    第一种方式是使用反引号(esc键下面的按钮)将代码包裹起来</div>

<div>    下面是一个示例代码</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121165433515)</div>

<div>    第二种方式则是使用制表符或者至少4个空格进行缩进的行</div>

<div>    下面是一个示例代码</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121165602671)</div>

<div>    （5）换行</div>

<div>    如果我们想把一行文本进行换行，我们可以在需要换行的地方输入至少两个空格，然后回车即可，注意，如果不回车，是没有效果的，就像下面这样</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121170040687)</div>

<div>   （6）引用</div>

<div>   如果我们在文章中引用了资料，那么我们可以通过一个右尖括号">"来表示这是一段引用内容。我们可以在开头加一个，也可以在每一行的前面都加一个。我们还可以在引用里面嵌套其他的引用，下面是一个示例：</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121170507567)</div>

<div>（7）链接</div>

<div>    如果我们文章中加入一个链接，那么我们通过下面的方式添加</div>

<div>[链接文字](链接地址)
例子： [Markdown](http://blog.csdn.net/zhaokaiqiang1992)</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121170908609)</div>

<div>    （8）分割线</div>

<div>    如果我们想用分割线对内容进行分割，我们可以在单独一行里输入3个或以上的短横线、星号或者下划线实现。短横线和星号之间可以输入任意空格。以下每一行都产生一条水平分割线。</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121171114184)</div>

<div>    （9）列表标记</div>

<div>    如果我们的内容需要进行标记，那么我们可以使用下面的方式</div>

<div>![](./原来Github上的README.md文件这么有意思——Markdown语言详解 - 彭满意 - 博客园_files/20141121171601583)</div>

<div>    好了，这些东西完全够用了，休息，休息一下...</div>

</div>

</div>

</div>
