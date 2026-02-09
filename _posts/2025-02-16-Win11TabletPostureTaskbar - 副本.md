---
layout:     post   				    # 使用的布局（不需要改）
title:      Windows 11 24h2强制平板模式			# 标题 
subtitle:   2025年2月17日测试有效 #副标题
date:       2025-02-16 				# 时间
author:     catalysia 						# 作者
header-img: img/postimg/post-bg-2024-0401.webp 	#这篇文章标题背景图片
catalog: true 						# 是否归档
# encryptedpost:                      # 加密内容
tags:								#标签
    - Windows
    - Tips
---
Windows 11 24h2更新后**开启Win11平板模式(视频中任务栏)的教程**：[https://www.bilibili.com/read/cv23620489](https://www.bilibili.com/read/cv23620489)的强制进入平板模式的方法失效

所以有了新的修改方法，此方法仅打开任务栏的平板模式
## 第一步 ##
打开注册表，定位到 HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer

## 第二步 ##
新建一个名为TabletPostureTaskbar的DWORD32类型值，数据为1。

## 第三步 ##
使用任务管理器重启资源管理器。

<!--加密用代码
<div id="pwinput">{{ page.tips | default: "请输入密码:" }}<br />
    <input id="inputkey" type="password" /> <button onclick="onbtnDecrypto()">解密</button>
 </div>
 <div id="output"></div>
-->