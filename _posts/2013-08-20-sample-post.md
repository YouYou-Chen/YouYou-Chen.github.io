---
layout: post
title: Flexbox弹性布局
tags: [code, syntax]
categories:
- blog
---

# 关于网页设计中Flexbox弹性布局的学习笔记

Flexbox:方向、对齐、次序、弹性。
Flexbox的使用在网页设计中非常普遍，也是老师在网页设计这门课中一直关注的考点。
在CSS编辑中，使用Flexbox的属性有；display:flex;align-items;justify-content。
align-items是沿交叉轴对齐。align-items:stretch(默认。拉伸元件以适应容器)/center(中心元素)/flex-start(位于元素在容器的开头)/flex-end(位于元素在容器的末端)/baseline(位于容器基线)/initial(默认值)/inherit(从其父元素承此属性)
justify-content是沿主轴对齐。stretch(默认。拉伸元件以适应容器)/center(中心元素)/flex-start(位于元素在容器的开头)/flex-end(位于元素在容器的末端)/space-between(位于各行之间留有空白容器内)/space-around(各行之前，之间，之后空白内)/initial(默认值)
Flexbox使用可以调整一个网站页眉的导航的移动。能很方便地进行调整。可以运用上面我所列举的进行偏移。
除了可以偏移，我们还可以对这些模块进行反序。
flex-direction:row是从左到右排序，如果要相反方向，则是row-reverse;flex-direction:column是从上到下，如果相反方向则是column-reverse;所以相反方向只要在后面加上reverse即可。
我们可以把一整个的东西进行不同方向的对齐，如果我们只需要其中某一个元素按不同方向对齐，那么我们需要的是align-self。
如下例子：.Flexinner{display:flex;}   .Flexwapper{display:flex;}   .Alignself{align-self:flex-end;}
这个例子意思是现在HTML档建一个Alignself类，然后在CSS档里就可以对父级元素下子元素按不同方向的对齐。
Flex-item伸缩项定义宽度，还可通过flex属性定义宽度，伸缩性（flexiness）
flex:1(伸展flex-grow) 1（收缩flex-shrink） 100px(基准flex-basis)。
我也发现了一样有趣的事情就是，在一个网站里，可以用order来排序，进行flexbox的偏移和对齐。
