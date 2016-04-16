# 一个前端的MAC

经常遇到配MAC后不知道如何配环境，或者是要到处在网上找需要安装什么，所以此处列出一个清单。

## 通用

### 1.修改MAC主机名

用惯了terminal, 不想看到XXX@localhost， 可以修改一下主机名

修改为主机名为Superman:

```
sudo scutil --set HostName Superman
```

### 2.修改MAC共享机器名:

不想别人AirDrop时看到的XXX’MAC, 可以设置一下共享机器名 

system -> preference -> sharing

系统 -> 偏好设置 -> 共享

### 3.Dock栏加入最近使用的app

打开Terminal, 输入defaults write com.apple.dock persistent-others -array-add
'{ "tile-data" = { "list-type" = 1; }; "tile-type" = "recents-tile"; }';
killall Dock回车

### 4.触摸板

MAC的触摸半绝对是pc中最好用的, 用好了可以不用鼠标了(前端，其它就不清楚了)

**至少我现在是可以不用鼠标了，哈哈**

- 开启单击轻触
- 双指轻触右击及滚动
- 三指选取移动
- 四指换屏, 选择程序
- 五指显示桌面, 显示所有程序

## 软件

### 常用

- vmware
- evernote
- qq
- wechat
- xcode
- NeteaseMusic
- thunder
- vlc
- office for mac
- mindnode pro
- lanscan pro   // 扫描局域网
- istat menus   // 电脑状态
- moom          // 窗口调整,更喜欢spectacle
- beyondcompare // 文件对比
- tuxerantfs    // mac读写移动硬盘
- tickeys       // 按键声
- noizio        // 环境声模拟
- licecap       // 大爱的一个生成git录制工具
- pocket

### 偏向开发

- git
- robomongo
- navicat
- opera
- chrome
  - 插件
  - switchyomega,可在网上下crx离线文件
  - aka switcher
  - ublock
  - postman,api测试很好的工具
  - google账号一个，同步方便
  - [二维码生成器](https://github.com/wungqiang/qrome)
  - pocket,大爱
  - wappalyzer, 显示当前网站所用技术栈
- firefox
  - 插件
  - autoproxy
  - ublock
  - firebug
- mou
- charles
- alfred 2
- iterm 2
- spectacle
- photoshop
- dash
- cheatsheet
- tower
- parallels desktop
- sketch

## 开发使用

安装前请先弄清楚每个是做什么的，然后有选择性的安装

### 1.MAC上的软件管理器

- Homebrew

### 2.MAC数据库

- mysql

- mongodb

- redis

### 3.Web服务器

- apache

- nginx // 我较偏爱

### 4.Terminal

- iterm2 // 分屏等，找个好看的主题

- on my zsh

### 5.编辑器

- vim // 我较喜欢, 注意升级最新的, 多多的插件

- sublime

- webstorm

### 6.python环境配置

- pip

- virtualenv

### 7. node相关模块

- cnpm // 经常有网络问题(你懂的), 不能下包，可用这个

- node/npm

- webpack

- grunt-cli

- gulp

- bower

- yo

- nvm

- http-server

- node-inspector // 调试node代码

- weinre // 调试webview的样式及请求很好的一个工具

- phantomjs

- express

- lodash // tool utilities

- request // http request client

- pm2/forever/supervisor

- async/when/promise/bluebird

- socket.io

- moment

- pdfkit

- redis // redis node driver

- mongo

- mongoose

- node-mkdirp

- debug/morgan

- ssh2

- shelljs

- node-xml2js

- nconf

- nodemailer

- jsonwebtoken

- node-uuid

### 8.跨平台开发

- electron

- nwjs

### 9.hybird框架(传说中的全栈全平台前端)

- cordova

- ionic

- phonegap

### 10.css预编译框架

- sass

- less

- compass

__安装compass不成功时可修改安装源__:

```
gem sources --remove https://rubygems.org/
gem sources -a https://ruby.taobao.org/
gem sources -l // 如果修改为taobao的安装源则可以重新安装了
```
