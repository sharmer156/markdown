# markdown语法之如何插入图片
* [markdown语法之如何插入图片](#markdown语法之如何插入图片)
	* [大面积及多条链接的处理](#大面积及多条链接的处理)
		* [常用](#常用)
		* [文末附加型](#文末附加型)
	* [目录](#目录)
	* [正文](#正文)
	* [图片上传方式](#图片上传方式)
	* [插入在线图片](#插入在线图片)
	* [插入本地图片](#插入本地图片)
	* [图片链接方式](#图片链接方式)
		* [行内式图片链接](#行内式图片链接)
	* [参考式图片链接](#参考式图片链接)
	* [几个问题探讨](#几个问题探讨)
		* [问题1：图片上传和图片链接两种方式的区别](#问题1图片上传和图片链接两种方式的区别)
		* [问题2：Markdown中如何指定图片的高和宽？](#问题2markdown中如何指定图片的高和宽)
		* [问题3：Markdown中如何指定图片的对齐方式？](#问题3markdown中如何指定图片的对齐方式)
* [jupyter中插入图片时的经验](#jupyter中插入图片时的经验)
* [youtube 视频链接](#youtube-视频链接)


## 大面积及多条链接的处理
### 常用
   [花瓣网](http://huaban.com/favorite/web_app_icon/?md=bdwzshejidaren)
    *   [站酷](http://zcool.com.cn/)
    *   [包图网](http://ibaotu.com/tupian/haibao.html?spm=shejidaren)
    *   [Designer News](https://www.designernews.co/)
    *   [iStock中国](http://www.veer.com/?utm_source=shejidaren&utm_medium=leftbanner&chid=8191)
    *   [Awwwards](http://www.awwwards.com/)
    *   [abduzeedo](http://abduzeedo.com/)
  网站和博客中多页面的链接，比较适用的链接类型，效果如下
![](https://i.imgur.com/fRI8PCx.jpg)
![](https://i.imgur.com/zBrH5GX.jpg)

理想的加说明的链接类型，效果如下：（鼠标停留就能显示链接网址的具体说明内容）
[Easy icon](http://easyicon.net "图标搜索引擎(中英)")
* [Icon Finder](http://www.iconfinder.com "图标搜索引擎(英)")

* [Logo EPS](http://www.logoeps.com "可以免费下载矢量LOGO模板的网站")

### 文末附加型

[说明][1]

在文章最后
[1]:https://github.com/suziwen/blogxiaoshujiang/blob/master/2018-6-22%20%E6%80%9D%E7%BB%B4%E8%84%91%E5%9B%BE%E8%AF%AD%E6%B3%95%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md



在Markdown编辑器中插入图片有两种方式：

*   使用工具栏上的图片上传功能

*   自己动手写图片链接的方式

下面分别介绍它们的使用方法。

## 图片上传方式

这种方式最简单，属图形化方式。大家可以很容易的在CSDN Markdown编辑器的工具栏那里找到图片上传的图标：![图片上传图标](https://img-blog.csdn.net/20150315205208680)

或者直接使用快捷键Ctrl + G，会弹出一个图片上传的对话框，可以看出既可以插入网上的在线图片也可以上传本地图片插入。

## 插入在线图片

![图片上传图标](https://img-blog.csdn.net/20150315210818959)

上面已经给出图片的书写格式：

<pre>在线图片地址 + 若干个空格 + 可选的用双引号括起来的图片提示   

*   1
*   2

</pre>

## 插入本地图片

对话框中切换到“上传图片”的标签后如下：

![图片上传对话框](https://img-blog.csdn.net/20150315205803398)

使用方式更简单：

<pre>选择本地图片 — 上传 — 下面方框里显示图片预览 — 最后确认插入  

*   1
*   2

</pre>

## 图片链接方式

如果插入的是在线图片，即只有图片URL，那么除了上面用图形化方式操作之外，还可以使用图片链接的方式。

Markdown使用一种和「[普通文本链接](http://blog.csdn.net/lanxuezaipiao/article/details/44307757#textlink)」很相似的语法来标记图片，同样也允许两种样式： **行内式**和**参考式**。

### 行内式图片链接

**行内式的图片链接语法如下：**

<pre>![Alt text](/path/to/img.jpg)    ![Alt text](/path/to/img.jpg "Optional title")  

*   1
*   2
*   3
*   4

</pre>

**详细叙述各个组成部分：**

*   一个惊叹号 !
*   接着一个方括号，里面放上图片的替代文字，也就是当图片还未加载成功时显示的替换文本
*   接着一个普通括号，里面放上图片的网址，以及可选的用双引号（或单引号或括弧）包住的’title’文字，两者之间用若干个空格分割开来，如果加上了’title’文字，那么鼠标移到该图片上就会显示出该文字

**一个实例：**

下面我在网上找了个在线图片，复制它的URL按上面的语法格式写即可成功插入图片。

<pre>![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg "这是CSDN的图标")  

*   1
*   2

</pre>

**效果为：**

![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg "这是CSDN的图标")

## 参考式图片链接

**参考式的图片链接语法则如下面这样：**

<pre>![Alt text][id]    

*   1
*   2
*   3

</pre>

其中「id」是图片参考的标签，图片参考的定义方式和链接参考一样，**可以放在文档的任何位置。**

**详细叙述各个组成部分：**

*   一个惊叹号 !
*   接着一个方括号，里面放上图片的替代文字，也就是当图片还未加载成功时显示的替换文本
*   接着另一个方括号，里面是图片参考的标签id，id可以是数字、英文字符，也可以是中文
*   最后在文档的任何位置处写上标签id的内容定义，内容定义的形式为： 

    *   一个方括号（前面可以选择性地加上至多三个空格来缩进），里面输入所要定义的标签id
    *   接着一个冒号
    *   接着一个以上的空格或制表符
    *   接着图片的网址
    *   最后选择性地接着title内容，可以用单引号、双引号或是括弧包着，与上面一样

**例子：**

还是以上面那个图片URL为例，改写成参考式链接如下：

<pre>![CSDN图标][csdn]    

*   1
*   2
*   3

</pre>

**效果：**

![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg "这是CSDN的图标")

## 几个问题探讨

下面针对Markdown插入图片的方式提出几个大家可能会问的问题，并根据自己的经验进行探讨解答。

### 问题1：图片上传和图片链接两种方式的区别

不管是利用图片上传的方式还是图片链接的方式插入图片，最终形成的都是Markdown内部的图片链接语法，**因此两种方式在本质上是一样的。**

比如我上传一张本地图片，成功插入后Markdown对应内容如下：

<pre>![这里写图片描述](https://img-blog.csdn.net/20150316184625949)  

*   1
*   2

</pre>

可以看出在我们上传本地图片成功后，CSDN-markdown编辑器会将服务器上该图片的地址取出来，然后用Markdown图片链接的语法插入图片。因此我们在上传图片后，还可以在对应的Markdown内容上进行修改，加上图片描述和图片的title。

### 问题2：Markdown中如何指定图片的高和宽？

到目前为止， Markdown还没有办法指定图片的宽高，如果需要的话，**你可以使用普通的 <img> 标签，利用它的width和height属性来定制宽高。**

还是以上面那个图片URL为例，如果我们希望把它的大小改为300*120，则可以这么做：

<pre><img src="http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg" width = "300" height = "120" alt="CSDN图标" />  

*   1
*   2

</pre>

**效果：**

![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg)

### 问题3：Markdown中如何指定图片的对齐方式？

大家可能也注意到了，CSDN-markdown编辑器显示的图片默认都是左对齐，那能不能将其改为居中对齐或右对齐呢？

答案是Markdown做不到，但跟「2」一样，**我们可以借助html语法来实现，html中让一个元素居中的方式也有很多，**下面给出两种方式供参考。

**方法一（推荐）：**

如果只是居中对齐，则可以使用html中的<center>...</center>标签，包围在Markdown图片链接内容的外面即可，如下：

<pre><center>  ![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg "这是CSDN的图标")  </center>  

*   1
*   2
*   3
*   4

</pre>

**效果**：

<center>
![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg "这是CSDN的图标") 
</center>

**当然，上面也说了，该方法只能用于居中对齐，不能进行右对齐。**

**方法二：**

使用html中的div标签，它有个对齐属性align，可以指定为left、center和right以实现左对齐、居中对齐和右对齐。**不过经我实验，这种方式div标签之间不能放Markdown图片链接语法，而只能是html的语法格式，因此还要配合<img>标签使用。**

下面是居中对齐的写法示例：

<pre><div align="center">  <img src="http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg"  alt="CSDN图标" />   </div>  

*   1
*   2
*   3
*   4

</pre>

**效果：**

![CSDN图标](http://imgtech.gmw.cn/attachement/jpg/site2/20111223/f04da22d7ba7105e1d7507.jpg)

**注意：** 这里如果大家仔细看的话可以发现上面**闭合标签</div>缩进了一个空格**，因为经我尝试，这里如果不缩进一个空格就达不到想要的效果，会造成某些Markdown语法失效。

# jupyter中插入图片时的经验

**效果：**
![day01](Info-graphs/Day1.jpg) <!-- 说明 图片中不要含有空格 -->
![day02](Info-graphs/Day%202.jpg)  <!--  说明 图片名称中尽量有空格，如果有空格使用%20代替 -->
![Data Science Venn Diagram](figures/Data_Science_VD.png)
<!-- ![Day%201.jpg](attachment:Day%201.jpg) --> <!--  说明 jupyter中 insert image相当于直接添加了附件会增加文件的大小（带附件的ipynb文件在github中可能无法读取图片而且无法在线编辑，使用markdown的隐藏代码或删除后，恢复正常-->

**代码：**
```markdown
![day01](Info-graphs/Day1.jpg) <!-- 说明 图片中不要含有空格 -->
![day02](Info-graphs/Day%202.jpg)  <!--  说明 图片名称中尽量有空格，如果有空格使用%20代替 -->
![Data Science Venn Diagram](figures/Data_Science_VD.png)\n
<!-- ![Day%201.jpg](attachment:Day%201.jpg) --> <!--  说明 jupyter中 insert image相当于直接添加了附件会增加文件的大小（带附件的ipynb文件在github中可能无法读取图片而且无法在线编辑，使用markdown的隐藏代码或删除后，恢复正常>
```

# youtube 视频链接
**效果：**

<a href="https://www.youtube.com/watch?v=hUnRCxnydCc" target="_blank"><img src="https://raw.githubusercontent.com/marcotcr/lime/master/doc/images/video_screenshot.png" alt="KDD promo video"/>

**代码：**

```markdown
<a href="https://www.youtube.com/watch?v=hUnRCxnydCc" target="_blank"><img src="https://raw.githubusercontent.com/marcotcr/lime/master/doc/images/video_screenshot.png" alt="KDD promo video"/>
```
