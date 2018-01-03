---
layout: archive
title: "信息可视化作品集"
date: 2018-1-1T14:25:45-04:00
modified:
excerpt: 
tags: []
image: 
  feature: 
  teaser:
---

在此展示信息可视化的作品

<div class="tiles">
{% for post in site.categories.tableau %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 tableau 的列出来-->
