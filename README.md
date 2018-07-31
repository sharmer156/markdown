# markdown
markdown somthing

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



