# 开始使用


## 第一步：环境安装

1. 获取BBuilder安装包并安装。

2. 安装依赖程序：nodejs

3. 安装微信小程序IDE（按需）

4. 安装阿里小程序IDE（按需）

安装后IDE的结构如下：

<img src="./ide.png"/>




## 第二步：新建应用

点击<code>新建应用</code>菜单，在弹出面板中输入<code>项目名称</code>和<code>工作空间</code>，点击确定即可完成应用的创建。

基础目录说明：

<code>.bbuilder</code>目录：工程配置目录，请勿改动

<code>build</code>目录：构建资源目录，所有平台的模板均在此目录，可根据实际情况修改，一般情况无需改动

<code>src</code>目录：源码目录，编写的所有代码均在此处，外部无效。内部一般根据功能分为pages、components、assets、resources等目录。

<code>package.json</code>文件：项目基本配置文件，该文件主要用于构建，如果是小程序里的依赖包，请单独在小程序内安装。

构建产物目录说明：

<code>node_modules</code>目录：构建所需的依赖模块目录。

<code>out-browser</code>目录：浏览器代码输出目录。

<code>out-miniprogram</code>目录：微信小程序代码输出目录。

<code>out-aliapp</code>目录：阿里小程序代码输出目录。


## 第三步：安装依赖

可以使用<code>ctrl + ~</code>快捷键打开终端面板，在终端中如下指令完成安装

```bash

npm install

```

也可以点击<code>开发管理</code>菜单，在弹出面板的<code>启动本地服务</code>中选择<code>安装</code>，点击确定即可完成安装。

日志位于与终端同分类的tab中<code>output面板-bridge分类</code>。下面涉及启动本地服务的，日志均在此处查看。


## 第三步：启动服务

### H5：

编译命令：<code>npm run watch browser</code>

启动web服务：<code>npm run browser default</code>，启动后访问:http://localhost:8000 可以查看页面。其中default可以换成wx，则页面必须在微信中访问，如果仅执行<code>npm run browser</code>，则同时在浏览器和微信中均可访问。 

也可以点击<code>开发管理</code>菜单，在弹出面板的<code>启动本地服务</code>中选择<code>浏览器</code>，点击确定即可完成编译和web服务启动。

### 微信小程序

编译命令：<code>npm run watch miniprogram</code>启动页面监听，然后使用微信官方的开发工具打开out-miniprogram目录。

也可以点击<code>开发管理</code>菜单，在弹出面板的<code>启动本地服务</code>中选择<code>小程序</code>，点击确定即可完成微信小程序的编译。

### 钉钉小程序

编译命令：<code>npm run watch aliapp</code>启动页面监听，然后使用阿里官方的开发工具IDE打开out-aliapp目录（该IDE内部可切换钉钉和支付宝小程序环境）。

也可以点击<code>开发管理</code>菜单，在弹出面板的<code>启动本地服务</code>中选择<code>钉钉/支付宝</code>，点击确定即可完成阿里小程序的编译。

## 说明

### VSCODE 扩展关联
打开任意axc文件,点击右下角的“纯文本”按钮，然后点击AUI。axp文件同样操作一次。        
<img src="./start.png"/>

### 起始页面

应用启动的起始页面固定为/src/pages/index/index.axp。

