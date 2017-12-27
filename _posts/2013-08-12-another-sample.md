---
layout: post
title: 媒体查询
tags: [code, syntax]
categories:
- blog
---


# 关于网页设计中媒体查询的学习笔记
媒体查询是根据设备显示器特性设定CSS样式
断点是重点，是由内容和设计本身决定。
有多种方式来增加媒体查询
第一种方法是在CSS中插入。如：@media screen and (min-width:50em){} 意思是在屏幕最小宽度为50em时可以发生CSS的样式变化
例子如下：body{background-color:grey;}
@media screen and (min-width:50em){body{background-color:red;}}
第二种方法是在link标签中使用媒体查询。如<link rel="stylesheet" type='css' media='screen' href='....css'>在HTML中插入媒体查询，只需使用属性Link即可使用。
第三种方法是用@import导入CSS时使用媒体查询
但这种方法要谨慎使用
媒体查询也有几种，有组合媒体查询、悬停媒体、环境媒体、指针媒体
组合媒体查询
如：<link rel='stylesheet' media='screen and (orientation:portrait)and(min-width:80px),projection'href='800'/>这里的组合媒体查询意思是说在一行代码里用逗号就可以增加多个媒体查询属性，只要其中任何一个媒体查询表达式为值，可应用。
指针媒体查询是指指针设备代表触摸屏设备中手指，指针设备可能是鼠标。指针媒体的三个值为none\coarse和fine。格式如下；
@media(pointer:coarse){}
悬停媒体，也是网站上最常见的媒体查询。悬停（hover）
@media(hover:none){}无悬停
@media(hover:no-demand){}可悬停但要启动
@media(hover){}可悬停
环境媒体查询
环境媒体查询用于调节屏幕亮度
@media(light-level:normal){}标准
@media(light-level:dim){}暗光
@media(light-level:washed){}强光
这里还有一些媒体查询特性，也是重点
width视口宽度，height视口高度，device-width渲染表面宽度，device-height渲染表面高度，orientation设备方向是水平还是垂直，aspect-ratio视口宽高比，monochrome单色祯缓冲表示每个像素位数，值必是数值，resolution屏幕打印分辨率，scan针对电视逐行扫描，grid设备基于位图。


