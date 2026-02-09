---
layout:     post   				    # 使用的布局（不需要改）
title:      罗技Options+软件自定义安装			# 标题 
subtitle:   2026年2月9日测试有效 #副标题
date:       2026-02-09 				# 时间
author:     catalysia 						# 作者
header-img: img/postimg/post-bg-2024-0401.webp 	#这篇文章标题背景图片
catalog: true 						# 是否归档
# encryptedpost:                      # 加密内容
tags:								#标签
    - Windows
    - Tips
---
安装鼠标驱动罗技Options+，不安装一些没用功能的方法

## 第一步 ##
下载任意版本的logioptionsplus_installer，去罗技官网下载就行，[https://www.logitech.com/zh-cn/software/logi-options-plus.html](https://www.logitech.com/zh-cn/software/logi-options-plus.html)
下载后放到任意文件夹，打开cmd定位到下载的文件夹。

## 第二步 ##
在cmd输入 logioptionsplus_installer.exe /help
会得到命令行参数列表

/quiet
                         在没有 UI 的情况下静默安装应用程序。

/analytics
                         Yes（或）No
                         显示或隐藏用户分享应用程序使用情况和诊断数据的选项。默认值为 Yes。

/flow
                         Yes（或）No
                         显示或隐藏 Flow 功能。默认值为 Yes。

/sso
                         Yes（或）No
                         显示或隐藏用户登录应用程序的功能。默认值为 Yes。

/update
                         Yes（或）No
                         启用或禁用应用程序更新。默认值为 Yes。

/dfu
                         Yes（或）No
                         启用或禁用设备固件更新。默认值为 Yes。

/backlight
                         Yes（或）No
                         启用或禁用支持的键盘上的键盘背光。默认值为 Yes。

/log <directory path>
                         在安装失败时捕获指定路径中的日志文件。

/logivoice
                         Yes（或）No
                         启用或禁用罗技语音功能。默认值为 Yes。

/aipromptbuilder
                         Yes（或）No
                         启用或禁用 AI Prompt Builder 功能。默认值为 Yes。

/device-recommendation
                         Yes（或）No
                         启用或禁用设备推荐功能。默认值为 Yes。

/smartactions
                         Yes（或）No
                         启用或禁用 Smart Actions 功能。默认值为 Yes。

/actions-ring
                         Yes（或）No
                         启用或禁用 Actions Ring 功能。默认值为 Yes。

/install-msoffice-plugins
                         安装所有 Microsoft Office 插件（Excel、PowerPoint 和 Word）。

/install-adobe-plugins
                         安装所有 Adobe 插件（Lightroom、Illustrator、Photoshop 和 Premiere Pro）。

/uninstall
                         静默卸载应用程序。

/help
                         显示可用的参数。


## 第三步 ##
根据需求在cmd输入对应的参数就行。
比如这样：
logioptionsplus_installer.exe /analytics no /flow yes /sso yes /update yes /dfu yes /backlight yes /logivoice no /aipromptbuilder no /device-recommendation no /smartactions no /actions-ring no /install-msoffice-plugins /install-adobe-plugins

<!--加密用代码
<div id="pwinput">{{ page.tips | default: "请输入密码:" }}<br />
    <input id="inputkey" type="password" /> <button onclick="onbtnDecrypto()">解密</button>
 </div>
 <div id="output"></div>
-->