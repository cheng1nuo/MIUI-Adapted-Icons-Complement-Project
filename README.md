# MIUI 完美图标补全计划

[![Subscribe](https://img.shields.io/badge/Telegram-Subscribe-blue.svg?logo=telegram)](https://t.me/miuiicons)
[![Chat](https://img.shields.io/badge/Telegram-Chat-blue.svg?logo=telegram)](https://t.me/miui_icons_dev)
[![Stars](https://img.shields.io/github/stars/pzcn/MIUI-Adapted-Icons-Complement-Project)](https://github.com/MIUI-Adapted-Icons-Complement-Projectreleases/)
[![Download](https://img.shields.io/github/downloads/pzcn/MIUI-Adapted-Icons-Complement-Project/total)](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/releases)
[![GitHub release](https://img.shields.io/github/v/release/pzcn/MIUI-Adapted-Icons-Complement-Project)](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/releases)
[![](https://data.jsdelivr.com/v1/package/gh/pzcn/IconsCDN/badge?style=rounded)](https://www.jsdelivr.com/package/gh/pzcn/IconsCDN)

使用 Magisk 模块和 mtz 主题包的形式，补全/修复 MIUI12 中未适配以及适配不佳的图标。基于官方图标去除牛皮癣，制作成分层图标。

----

### 下载地址

# 模块安装已经更改为安装器方式，旧版本模块不再提供更新。
# 安装器 下载地址 https://www.coolapk.com/apk/dev.miuiicons.pedroz

### 项目介绍

自 MIUI 12 起，MIUI 新增加了完美图标的特性。其依赖于 MIUI 绘制的部分图标以及图标自身的 Adapted Icon。除可以实现分层效果外，还可以去除部分图标的牛皮癣。但这需要APP按照标准适配 Adapted Icon，或者 MIUI 进行单独绘制。为了让更多 APP 获得这个特性，诞生了本项目。

在 MIUI12 的早期版本里，MIUI 绘制的第三方桌面图标有较高的优先级。但是某次更新后，若 APP 有了 Adapted Icon 则优先调用自带图标，这就造成了部分显示效果不佳，包括但不限于支付宝、淘宝等，表现为包含牛皮癣（双十一、购物节等）、不按照规则适配（整张图片只有一层，底层为纯色等）。为解决图标显示优先级问题，简化目录结构，本项目已采用 Github Action 自动生成模块，目前显示均为最高优先级。

目前包含了 MIUI默认主题、探·界主题、Flyme9主题、LRONE主题，Luck7主题、完美曲线主题，未来可能会添加更多其他主题。

#### 适配版本
Android 10 及以上的 MIUI 12

#### 图标数量

![](https://img.shields.io/badge/dynamic/json?color=brightgreen&label=Icon%20count&query=%24.count&url=https%3A%2F%2Fmiui.netlify.app%2Fcount.json)

#### Magisk模块（推荐）

模块包内包含默认主题和图标。安装过程支持多主题选择，除默认主题外的其他主题需要在线下载。包含联网检查、网速检查等多项措施。主题包会在线获取最新版本。

#### Mtz主题包（不推荐）
同其他Mtz主题一样，MIUI国内版需要设计师账号或主题破解才可以正常使用。mtz使用相关问题请自行解决。

*注意：部分机型和MIUI版本可能出现手势问题，参考下方常见问题。*

*注意：仅默认主题提供mtz。为保护设计师利益，虽然我们取得了授权，第三方主题也不会提供mtz版本，请使用magisk模块。*

#### 自定义附加模块

（仅供Magisk模块版本使用）搭配MIUI完美图标补全模块，优先使用自己绘制的图标。[详细说明](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/wiki/%E9%99%84%E5%8A%A0%E6%A8%A1%E5%9D%97)

#### 图标存档

提供部分图标其他样式，有需要的话解压后放入附加模块刷入使用[详细说明](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/wiki/%E5%9B%BE%E6%A0%87%E5%AD%98%E6%A1%A3)

----

### 下载地址

[Release](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/releases)页面下载

[下载导航站](https://miui.iconsx.tech)

----

### 常见问题

1. Q：mtz主题包出现了返回手势结束时直角变圆角现象，如何解决？

   A：似乎是MIUI系统版本问题，目前发现的两种解决方法：①使用稳定版桌面，卸载内测桌面（部分机型依然无效）②不使用mtz，换用magisk模块。
   

2. Q：为什么xxx这个图标和原图标不太一样？

   A：一部分图标去除了活动banner，另外图标是手动修改的，为了保证良好的显示效果进行了重新绘制，无法保证和原图标完全一致。


3. Q：能把xx图标换成xx样式吗？

   A：参考适配指南自行绘制，然后使用[附加模块](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/wiki/%E9%99%84%E5%8A%A0%E6%A8%A1%E5%9D%97)（针对Magisk版本）。

----

### 参与模块建设

您可以依据适配规则，申请适配或自行适配后提交。欢迎加入群组讨论参与模块建设。

#### 适配规则

对以下三种情况进行适配

1. MIUI完全没有对其进行适配的图标，且应用自身没有进行 Adapted Icon 的适配（即静态图标的效果）。

2. MIUI适配后不完美，整个图标都是前景的图标（移动图标即可看出），百度地图 前后景不分的图标

3. MIUI适配后有牛皮癣，比如 联通手机营业厅 包含有5G牛皮癣。

#### 申请适配

目前采用免费+付费的方式进行适配

热门应用免费适配，其他应用按照0.5元/个的方式收费适配

热门应用指酷安下载量高于10万的app

在QQ群 561180493 私聊群主进行适配 先适配后付款

#### 适配指南、提交适配

适配指南见 [Wiki](https://github.com/pzcn/MIUI-Adapted-Icons-Complement-Project/wiki/适配指南)

提交适配 提交PR或将文件发送至 [Telegram 群组](https://t.me/miui_icons_dev) 或QQ群内

#### 参与讨论

[![Subscribe](https://img.shields.io/badge/Telegram-Subscribe-blue.svg?logo=telegram)](https://t.me/miuiicons)
[![Chat](https://img.shields.io/badge/Telegram-Chat-blue.svg?logo=telegram)](https://t.me/miui_icons_dev)

QQ群：561180493

----

### 致谢

#### 主题授权：

[LRONE主题](http://zhuti.xiaomi.com/detail/share/41f02867-78b0-457c-a134-b9eab07d7ac9?miref=share&packId=fcc4e5ff-1667-4689-a399-c5538c60f349)授权：
[@江户川Conan](http://www.coolapk.com/u/1091207) 

[Luck7主题](http://zhuti.xiaomi.com/detail/share/508a77a8-11ee-448c-9a1a-b51b0253de76?miref=share&packId=ca2c0d02-f34e-464b-818e-35063507afc2)授权：
[@JellyBeans](http://www.coolapk.com/u/1375535) 

[完美曲线主题](http://zhuti.xiaomi.com/detail/share/6b9b4e54-9c13-4ee3-b5db-66daf0928bcf?miref=share&packId=fceeed6a-45dc-4a58-be11-12b2d370c315)授权：
[@栗子汤圆Ria](http://www.coolapk.com/u/1375535) 

#### 图标绘制：

[@潮留美海かり](http://www.coolapk.com/u/3701042) 自项目雏形起，合作绘制了大量图标

[@Yife Playte](http://www.coolapk.com/u/2222314) 绘制了大量图标，校对了之前历史遗留的问题图标

[@Eirperuier](http://www.coolapk.com/u/1780934) Luck7、完美曲线申请授权、累计自动化绘制了3000+图标

[@Mastiff Li](http://www.coolapk.com/u/1305926) [@世界第一小莲儿](http://www.coolapk.com/u/1780934)  @Shahzaib Ahmed

#### 技术支持：

[@相见即是缘](http://www.coolapk.com/u/1614257) [@dwhsmcb](http://www.coolapk.com/u/1662815) [@余空_YuK](http://www.coolapk.com/u/680367) [@薛定谔の鼠](http://www.coolapk.com/u/1261690)
