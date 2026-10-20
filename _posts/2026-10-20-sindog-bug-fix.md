---
layout:     post
title:      签到狗自定义脚本
subtitle:   无法自动执行的bug修复
date:       2026-10-20
author:     Catalysia
header-img: img/postimg/post-bg-2024-0401.webp
catalog:    true
tags:
    - 路由器
    - koolshare
---

直接上传的自定义脚本会上传到 **/jffs/.koolshare/configs/signdog/qd_store/scripts/1/** 文件夹。
但是自动执行时要求的目录是 **/jffs/.koolshare/configs/signdog/qd_store/scripts/1/** 。

此时自动执行就会提示：
> node:internal/modules/cjs/loader:1143
>   throw err;
>   ^

> Error: Cannot find module '/jffs/.koolshare/configs/signdog/脚本名.js'
>     at Module._resolveFilename (node:internal/modules/cjs/loader:1140:15)
>     at Module._load (node:internal/modules/cjs/loader:981:27)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:128:12)
>     at node:internal/main/run_main_module:28:49 {
>   code: 'MODULE_NOT_FOUND',
>   requireStack: []
> }

> Node.js v18.20.2
> exit status 1
> q===END===d

**所以需要将两者连接起来**

`ln -sf /jffs/.koolshare/configs/signdog/qd_store/scripts/1/脚本名.js /jffs/.koolshare/configs/signdog/脚本名.js`
