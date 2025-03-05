---
layout: "../../layouts/MarkdownPostLayouts.astro"
title: "将 deepseek 接入微信实现自动聊天"
date: 2025-02-27
description: "将 deepseek 接入微信实现自动聊天"
tags: ["deepseek"]
author: "zjb"
image:
  url: "https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227194116466.png"
  alt: "微信自动聊天"
---

# 将 deepseek 接入微信实现自动聊天

### 1、打开 GitHub 链接：

[Releases · iwyxdxl/WeChatBot_WXAUTO_SE](https://github.com/iwyxdxl/WeChatBot_WXAUTO_SE)

点击下载：

![image-20250227194116466](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227194116466.png)

![image-20250227194258321](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227194258321.png)

### 2、下载之后将压缩包解压

双击打开 run.bat：（前提是要有 python 版本大于 3.8 小于 3.12 安装时需要包含路径和 pip）

![image-20250227233127154](C:\Users\zjb13\AppData\Roaming\Typora\typora-user-images\image-20250227233127154.png)

打开之后会自动给你安装依赖，等他安装完会跳出一个页面，如果没有跳出来就手动访问网页 http://localhost:5000/：

![image-20250227233242430](C:\Users\zjb13\AppData\Roaming\Typora\typora-user-images\image-20250227233242430.png)

### 3、进入配置编辑器的页面

准备俩个微信号，电脑上登录你的小号，手机上登录大号（小号不要给大号备注，大号的微信名也不要带特殊符号，不然识别会有问题）

让 ai 附身到你的小号上实现和你的大号自动聊天

填写用户列表：微信昵称是大号的微信名，最好就填写一个或俩个用户，用户太多会出 bug

![image-20250227195021752](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227195021752.png)

### 4、deepseek 的配置

点击硅基流动的网址

![image-20250227195444404](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227195444404.png)

点击 api 密钥----新建-----命名-----保存：

然后复制密钥，把密钥粘贴到上一张截图的 API Key 那里

![image-20250227195840679](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227195840679.png)

### 5、图片/表情包识别配置

和上一步同理，点击申请网站的链接

![image-20250227200128487](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200128487.png)

![image-20250227200229163](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200229163.png)

点击确定之后会生成密钥（关闭之后这个密钥无法再次查看）：

![image-20250227200318012](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200318012.png)

复制这串密钥粘贴到：

![image-20250227200452327](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200452327.png)

### 6、保存配置

滑到页面最下面进行保存

![image-20250227200547409](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200547409.png)

### 7、prompt 管理

![image-20250227200630220](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200630220.png)

可以点击编辑查看它默认的内容示例，可以复制过来

![image-20250227200709788](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200709788.png)

我们新建一个 prompt：

可以把默认的内容粘贴过来，文件名是你前面填写的微信昵称

备注部分不要进行修改，也不要删除，点击保存

![image-20250227200941796](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227200941796.png)

### 8、启动机器人

返回配置之后点击 start bot：
![image-20250227201124742](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227201124742.png)

此时微信会自动弹出对话框，不要关闭

用手机的大号给微信小号发信息，等待几秒，就会收到小号的自动回复

![image-20250227201632906](https://cdn.jsdelivr.net/gh/biliiiiii/blogimageee@main/image-20250227201632906.png)
