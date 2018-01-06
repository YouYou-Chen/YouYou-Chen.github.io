---
layout: archive
title: "信息可视化笔记"
date: 2018-1-1T11:40:45-04:00
modified:
excerpt: 
tags: []
image: 
  feature: tableau.gif
  teaser:
---

在此展示Tableau的笔记

<div class="tiles">
{% for post in site.categories.tableau %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 tableau 的列出来-->