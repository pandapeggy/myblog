---
layout: post
title: 独立域名配置
category: other
tags: [other]
excerpt: 差点成了我的拦路虎
---
&emsp;独立域名需要购买，我选择的是腾讯云的，获取其独立域名的价格和续费详细信息，购买了一个最便宜的域名。
## 1.登陆[腾讯云](https://buy.cloud.tencent.com/domain?price=1)
&emsp;选择域名，比对其续费价格和注册价格，结合自己的经济能力，挑选一个合适的域名。
&emsp;输入想要注册的域名，购买
### 2.根据网页指引进行域名认证与备案
## 3.进行解析域名
&emsp;差点就栽在这里了···
&emsp;点击页面中<https://console.cloud.tencent.com/domain>的解析选项，添加两条记录。
&emsp;一个是CNAME类型的记录，对应的主机类型填写www，记录值为github的项目名称
&emsp;一个是A类型的记录，对应的主机类型填写@，记录值写服务器ID(这个让我折腾了大半天，幸好一猿拔刀相助，帮我获取了一个地址：185.199.108.153)