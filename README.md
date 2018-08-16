# markdown
markdown somthing
# 目录
效果：
- **[环境依赖](#环境依赖)**
- **[部署步骤](#部署步骤)**
- **[列表(目录)](#列表(目录))**
- **[链接](#链接)**
- **[图片](#图片)**
- **[文字格式](#文字格式)**
- **[引用](#引用)**
- **[表格](#表格)**
- **[版本更新](#版本更新)**

文字格式


- **[回目录](#普通目录)**

DEMO
===========================

## 环境依赖 ##
1.操作系统
node v0.10.28+
reids ~
2.依赖
3.其他软硬件要求

## 部署步骤 ##
1. 添加系统环境变量
    export $PORTAL_VERSION="production" // production, test, dev


2. npm install  //安装node运行环境

3. gulp build   //前端编译

4. 启动两个配置(已forever为例)
    eg: forever start app-service.js
        forever start logger-service.js
        
## 列表(目录)

# 普通目录
效果：
- **[团队项目](#团队项目)**
- **[原创项目](#原创项目)**
- **[fork项目](#fork项目)**
- **[star项目](#star项目)**
- **[回目录](#目录)**

代码：
```markdown
- **[团队项目](#团队项目)**
- **[原创项目](#原创项目)**
- **[fork项目](#fork项目)**
- **[star项目](#star项目)**
- **[回目录](#普通目录)**
```

### 无序列表
```markdown
* 项目1
  * 子项目1.1
  * 子项目1.2
    * 子项目1.2.1
* 项目2
* 项目3

+ 项目1
  + 子项目1.1
  + 子项目1.2
    + 子项目1.2.1
+ 项目2
+ 项目3

- 项目1
  - 子项目1.1
  - 子项目1.2
    - 子项目1.2.1
- 项目2
- 项目3
```
隐藏说明
<!-- 替换地址 -->
<!-- https://github.com/imhuay/CS_Interview_Notes-Chinese/blob/master/ -->
代码
```markdown
<!-- 替换地址 -->
<!-- https://github.com/imhuay/CS_Interview_Notes-Chinese/blob/master/ -->

```
效果
## RoadMap
- [数学](./数学)
  - [微积分的本质](./数学/微积分的本质.md)
  - [深度学习的核心](./数学/深度学习的核心.md)
- [机器学习-深度学习-NLP](./机器学习-深度学习-NLP)
  - 深度学习
    - [深度学习基础](./机器学习-深度学习-NLP/DL-深度学习基础.md)
    - [《深度学习》整理](./机器学习-深度学习-NLP/DL-《深度学习》整理.md)
    - [CNN专题](./机器学习-深度学习-NLP/DL-CNN.md)
  - 机器学习
    - [机器学习算法](./机器学习-深度学习-NLP/ML-机器学习算法.md)
    - [机器学习实践](./机器学习-深度学习-NLP/ML-机器学习实践.md)
  - 自然语言处理
    - [序列建模](./机器学习-深度学习-NLP/NLP-序列建模.md) TODO
    - [词向量](./机器学习-深度学习-NLP/NLP-词向量.md)
      - [Word2Vec](./机器学习-深度学习-NLP/NLP-词向量.md#word2vec)
      - [GloVe](./机器学习-深度学习-NLP/NLP-词向量.md#glove)
      - [FastText](./机器学习-深度学习-NLP/NLP-词向量.md#fasttext)
      - WordRank TODO
代码
```markdown
## RoadMap
- [数学](./数学)
  - [微积分的本质](./数学/微积分的本质.md)
  - [深度学习的核心](./数学/深度学习的核心.md)
- [机器学习-深度学习-NLP](./机器学习-深度学习-NLP)
  - 深度学习
    - [深度学习基础](./机器学习-深度学习-NLP/DL-深度学习基础.md)
    - [《深度学习》整理](./机器学习-深度学习-NLP/DL-《深度学习》整理.md)
    - [CNN专题](./机器学习-深度学习-NLP/DL-CNN.md)
  - 机器学习
    - [机器学习算法](./机器学习-深度学习-NLP/ML-机器学习算法.md)
    - [机器学习实践](./机器学习-深度学习-NLP/ML-机器学习实践.md)
  - 自然语言处理
    - [序列建模](./机器学习-深度学习-NLP/NLP-序列建模.md) TODO
    - [词向量](./机器学习-深度学习-NLP/NLP-词向量.md)
      - [Word2Vec](./机器学习-深度学习-NLP/NLP-词向量.md#word2vec)
      - [GloVe](./机器学习-深度学习-NLP/NLP-词向量.md#glove)
      - [FastText](./机器学习-深度学习-NLP/NLP-词向量.md#fasttext)
      - WordRank TODO
```
      
**快捷键**: [ctrl + u]
### 有序列表
```markdown
1. 项目1
2. 项目2
3. 项目3
    1. 项目3.1
    2. 项目3.2

1. 项目1
1. 项目2
1. 项目3
    1. 项目3.1
    1. 项目3.2

## 目录结构描述 ##
├── Readme.md                   // help/
├── app                         // 应用

├── config                      // 配置//
│   ├── default.json
│   ├── dev.json                // 开发环境//
│   ├── experiment.json         // 实验
│   ├── index.js                // 配置控制
│   ├── local.json              // 本地
│   ├── production.json         // 生产环境
│   └── test.json               // 测试环境
├── data
├── doc                         // 文档
├── environment
├── gulpfile.js
├── locales
├── logger-service.js           // 启动日志配置
├── node_modules
├── package.json
├── app-service.js              // 启动应用配置
├── static                      // web静态资源加载
│   └── initjson
│   	└── config.js 		// 提供给前端的配置
├── test
├── test-service.js
└── tools
```
## 链接
```markdown
[链接名称](链接地址)
[链接名称][1]
[1] : 链接地址
（?raw=ture）直接链接到文件并且大图显示，如果不加，会有github的框
<br>蓝色加重
```


## 图片
```markdown
![名称](链接地址)
![名称][1]
[1] : 链接地址
```


## 文字格式
```markdown
**这是文字粗体格式**

__这是文字粗体格式__

*这是文字斜体格式*

_这是文字斜体格式_
```


## 引用
```markdown
> 第一行引用文字
> 第二行引用文字
```


## 水平线
```markdown
***
----------
```
## 表格
```markdown（github无法使用）
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell
```

## 表格
```markdown
    markdown
```

## V1.0.0 版本内容更新 ##（仅列出重要更新)
1. 新功能	 aaaaaaaaa
2. 新功能	 bbbbbbbbb
3. 新功能	 ccccccccc
4. 新功能	 ddddddddd



---
title: 2018-6-22 思维脑图语法使用说明 
tags: 思维脑图,语法,小书匠
grammar_cjkRuby: true
grammar_mindmap: true
---

[toc]

[toc!?direction=lr]

小书匠从 6.1.0 版本开始，支持思维脑图语法功能。本文主要讲解思维脑图语法的使用。

## 语法

思维脑图语法与其他扩展语法一样，需要通过 `设置>扩展语法>思维脑图` 或者在每篇文章的元数据里指明使用该语法 。

### 元数据

`grammar_mindmap`

### 说明

1. 父子分支之间以两个空格区分
2. 如果存在多个根分支，系统会自动创建一个名称为 `root` 的虚拟根分支，以保存思维脑图只有一个根分支
3. 可以通过 root 参数，指定系统创建的虚拟 root 分支名称


### 示例

````
``` mindmap!
分支一
  分支一a
  分支一b
分支二
  分支二a
  分支二b
```
````

### 显示效果

``` mindmap!
分支一
  分支一a
  分支一b
分支二
  分支二a
  分支二b
```

## 参数

### theme 主题参数

目前主要有两种主题， `gray` 和 `colorful` ， 默认为 `colorful`

### direction 脑图方向参数

6 种显示方向参数。

1. LR: 从左到右，根节点在最左边
2. RL: 从右到左，根节点在最右边
3. H: 根节点在中间，分支在根节点左右两边水平扩散出来
4. TB: 从上到下，根节点在最上边
5. BT: 从下到上，根节点在最下边
6. V: 根节点在中间，分支在根节点上下两边垂直扩散出来

#### 示例

``` mindmap!?direction=V
大力神杯 W61 VS W62
  W57 VS W58
    W49 VS W50
      A 组第一 VS B 组第二
      C 组第一 VS D 组第二
    W53 VS W54
      E 组第一 VS F 组第二
      G 组第一 VS H 组第二
  W59 VS W60
    W51 VS W52
      B 组第一 VS A 组第二
      D 组第一 VS C 组第二
    W55 VS W56
      F 组第一 VS E 组第二
      H 组第一 VS G 组第二
```

### title 参数

在生成的思维脑图下方，显示一个说明性的文字

#### 示例

``` mindmap!?title=2018世界杯
大力神杯 W61 VS W62
  W57 VS W58
    W49 VS W50
      A 组第一 VS B 组第二
      C 组第一 VS D 组第二
    W53 VS W54
      E 组第一 VS F 组第二
      G 组第一 VS H 组第二
  W59 VS W60
    W51 VS W52
      B 组第一 VS A 组第二
      D 组第一 VS C 组第二
    W55 VS W56
      F 组第一 VS E 组第二
      H 组第一 VS G 组第二
```

### root 参数

当用户输入的根分支有多个时，系统会自动生成一个虚拟的根分支，用户可以通过该参数指定该虚拟分支的名称。

#### 示例

``` mindmap!?root=虚拟分支
分支一
  分支一a
  分支一b
分支二
  分支二a
  分支二b
```

### 多种参数结合

支持多种参数结合使用，多个参数之间以 `&` 连接

#### 示例

``` mindmap!?title=2018世界杯&direction=v&theme=gray
大力神杯 W61 VS W62
  W57 VS W58
    W49 VS W50
      A 组第一 VS B 组第二
      C 组第一 VS D 组第二
    W53 VS W54
      E 组第一 VS F 组第二
      G 组第一 VS H 组第二
  W59 VS W60
    W51 VS W52
      B 组第一 VS A 组第二
      D 组第一 VS C 组第二
    W55 VS W56
      F 组第一 VS E 组第二
      H 组第一 VS G 组第二
```


## 大纲思维脑图语法

小书匠除了支持**思维脑图语法**外，还增加了**大纲思维脑图语法**。

该语法使用当前文章的章节标题做为数据来源，不同的标题等级确定不同的分支层级。

### 语法

只要在原有的 `[toc]` 里加上感叹号，系统就会自动生成大纲思维脑图。

```
[toc!]
```

### 参数

除了思维脑图语法提供的参数外，大纲思维脑图语法还增加了几个额外的参数

#### depth 参数

用来控制思维脑图最深显示到第几级的标题

##### 示例

比如 depth 为 4, 就只会显示 `h1, h2, h3,h4` 等级的标题

[toc!?depth=4&title=只显示前面4级别的标题]

[toc!?depth=5&title=只显示前面5级别的标题]

#### root 参数

如果文章内存在多个一级标题 `h1`, 系统会自动创建虚拟的根标题，并且自动使用当前文章的主标题做为根标题来显示。用户可以通过该参数，修改虚拟根标题的名称。

- **[回目录](#目录)**
