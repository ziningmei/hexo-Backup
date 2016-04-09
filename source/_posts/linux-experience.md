---
title: linux服务器常用命令
date: 2016-04-09 22:43:54
tags:
- linux 

---
## 入门
### 申请服务器
我使用的是阿里云ECS，系统选的是centos6.5，因为有云翼计划，大学生一个月9.9，配置基本足够实用

### 入门使用
使用ssh工具连接服务器，mac直接使用terminal，命令 <code>ssh root@121.42.166.*</code>
然后会提示输入密码，mac命令行默认是看不见的，正确输入回车就行
建议安装appnode方便管理，目前公测免费的，地址：<https://www.appnode.com/>

<!--more-->

## 常用命令
### 解压，*.tar.gz 文件
```
tar -zxvf *.tar.gz
```
### 安装软件（比如apache）
```
yum install httpd
```