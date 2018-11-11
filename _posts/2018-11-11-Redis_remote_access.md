---
layout: post
title: "Redis"
categories: Redis
tags: Redis
author: TangPing
---
* content
{:toc}
##myeclise远程访问失败问题解决方法
	redis+端口.conf文件中bind 127.0.0.1 是否注释，protected-mode yes改为no，如果还是连接不上，那应该是linux防火墙未关闭。
	CentOS7关闭防火墙方法：
	查看防火墙状态

	firewall-cmd --state

	停止防火墙

	systemctl stop firewalld.service

	禁止防火墙开机启动

	systemctl disable firewalld.service