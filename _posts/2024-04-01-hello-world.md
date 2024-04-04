---
layout:     post   				    # 使用的布局（不需要改）
title:      你好~世界！ 				# 标题 
subtitle:   Hello!World~ #副标题
date:       2024-04-01 				# 时间
author:     catalysia 						# 作者
header-img: img/postimg/post-bg-2024-0401.webp 	#这篇文章标题背景图片
catalog: true 						# 是否归档
encryptedpost: 35f802676dba001f0807c5bdab5f3139222b5217412697031878c393076982e281d66e8439fae56bd37a860aa9a690e7fd5935f603d1bf67dd0191e7c4c7e2fa5797b88b83e5e9de155cbb279b02dadee222f01aa58dafe6782759ed8c9d3196a4afdc050863bb870cfcf6574b03d5d066716ac7a16dbcdc0229fd9a42d0b32fa61194cd8bb9e218a465262cfaaea6558c5692dd3cab172e243543c95d3d57be5eae57421a60dbc5b870a44bfa2cbe77f4b5696738b55f200a8607a2be6627a9c4c7f969f58e4592dca5100ac1bd3b049ee0a6da60d0c42fa11b7ce4799b47f6fc0b5c98cbebd3b0067b7c1ce00910864aa278d5ba9ec2603281af9f9640fd21e0d234e2cbb090597eb1bcf81ad0e77d37e2a71c2cb48a4cb2ad646ac3ffa2996bb2d8875ef521ff922c7cafcd653d1697ccdca2f5ddb6682156aa62b7cfabb558dee7f0a94cfde3411adf223eb7e6e8b0dbe3bf9cfb19a9441b9cf2ed912077a80aa721e77102db569f6c1282d3fee8
tags:								#标签
    - test
---

## Hey
>这是我的第一篇博客。

主要用于测试博客上的各种功能，所以你每次进来都可能有那么一点点不一样。甚至会有可能出现奇怪的bug和不可名状的景象。

有些时候需要按Ctrl+F5强制刷新，才能看到改变。

有一些需要密码才能访问的Post可能能在这里找到密码。

比如下面这个就是需要一个流传在互联网上的古老的二次元密码。

<div id="pwinput">{{ page.tips | default: "请输入密码:" }}<br />
   <input id="inputkey" type="password" /> <button onclick="onbtnDecrypto()">解密</button>
</div>
<div id="output"></div>