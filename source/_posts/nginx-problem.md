---
title: nginx遇到的问题
date: 2016-04-10 00:10:20
tags:
- nginx

---
## nginx遇到的问题
### 网页403 forbidden，日志显示 Permission denied 
在nginx.conf 的第一行加上一句话 user  root;使当前用户拥有权限

<!--more-->

### mac 安装nginx
1. <code>brew install nginx</code> 

2. 制作软连接
<code>sudo ln /usr/local/Cellar/nginx/1.8.1/bin/nginx /usr/local/bin/nginx 
</code>

3. 配置文件地址/usr/local/nginx/conf/nginx.conf

4. 控制命令
```
nginx 			  //别样的启动命令
nginx -s stop
nginx -s quit
nginx -s reopen
nginx -s reload
```
