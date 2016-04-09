---
title: nginx遇到的问题
date: 2016-04-10 00:10:20
tags:
- nginx

---
## 403 forbidden，
### 日志显示 Permission denied 
在nginx.conf 的第一行加上一句话 user  root;使当前用户拥有权限

<!--more-->