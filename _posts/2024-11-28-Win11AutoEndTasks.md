---
layout:     post   				    # 使用的布局（不需要改）
title:      Windows 11 应用阻止关机的解决办法			# 标题 
subtitle:   2024年11月28日测试有效 #副标题
date:       2024-11-28 				# 时间
author:     catalysia 						# 作者
header-img: img/postimg/post-bg-2024-0401.webp 	#这篇文章标题背景图片
catalog: true 						# 是否归档
# encryptedpost:                      # 加密内容
tags:								#标签
    - Windows
    - Tips
---
# Windows 11 每次关机都会提示有应用阻止关机，网上搜索到的解决办法比如修改组策略或者单纯在注册表里增加AutoEndTask=1不能解决问题，于是经过研究有了这篇文章。 #

## 第一步 ##
打开注册表，定位到 计算机\HKEY_USERS\.DEFAULT\Control Panel\Desktop

## 第二步 ##
添加字符串值AutoEndTasks 数值数据设置为1。

添加字符串值WaitToKillAppTimeout 数值数据设置为5000。

添加字符串值HungAppTimeout 数值数据设置为5000。

## 第三步 ##
定位到 计算机\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control

WaitToKillServiceTimeout 确定数据设置为5000

### 重启电脑 ###


## 备注 ##

**WaitToKillAppTimeout** 关机后，结束应用的等待时间。**字符串**类型，单位为毫秒。

**HungAppTimeout** 结束应用失败后，强制结束应用的等待时间。**字符串**类型，单位为毫秒。

**WaitToKillAppTimeout** 关机后，强制结束用硬选项。**字符串**类型，0为无效，1为有效。

**计算机\HKEY_USERS\.DEFAULT** 对所有用户生效。

<!--加密用代码
<div id="pwinput">{{ page.tips | default: "请输入密码:" }}<br />
    <input id="inputkey" type="password" /> <button onclick="onbtnDecrypto()">解密</button>
 </div>
 <div id="output"></div>
-->