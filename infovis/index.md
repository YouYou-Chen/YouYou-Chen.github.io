---
layout: archive
title: "信息可视化作品集"
date: 2017-12-30T11:40:45-04:00
modified:
excerpt: 
tags: []
image: 
  feature: 
  teaser:
---

在此展示Tableau教程视频笔记

<div class="tiles">
{% for post in site.categories.infovis%}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 infovis 的列出来-->