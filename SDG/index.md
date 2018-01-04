---
layout: archive
title: "HTML5的新语义元素"
date: 2017-12-30T11:40:45-04:00
modified:
excerpt: "给div元素赋予一个好理解的标记很有必要"
tags: []
image: 
  feature: timg.jpg
  teaser:
---

##HTML5的新语义元素 

作为网页编写者， 我们会给相应的div元素起个好理解的名字（比如class="Header"）。可是，单纯从代码来看， 任何用户代理（浏览器、屏幕阅读器、搜索引擎爬虫，等等）都不能确定每个div元素中包含的 是什么内容。用户辅助技术也无法区分不同的div。HTML5为此引入了新的语义元素。

1.<main>元素 

main元素用于定义主要内容的区块。

文档的主内容指的是文档中特有的内容，导航链接、版权信息、站点标志、广告 和搜索表单等多个文档中重复出现的内容不算主内容（除非网页或文档的主要内容就是 搜索表单）。

2.<section>元素 

section元素用于定义文档或应用中一个通用的区块。

section包装联系信息、 新闻源，等等。关键是要知道这个元素不是为应用样式而存在的。如果只是为了添加样式而包装 内容，还是像以前一样使用div吧。 

3.<nav>元素 

<nav>元素用于包装指向其他页面或同一页面中不同部分的主导航链接。

但它不一定非要用 在页脚中（虽然用在页脚中是可以的）；页脚中经常会包含页面共用的导航。如果你通常使用无序列表（<ul>）和列表标签（<li>）来写导航，那好改成用nav嵌套 多个a标签。

4.<article>元素 

<article>用于包含一个独立的内容块。

对于嵌套<article>而言，内部的<article>应该与外部<article>相关。
  
<div class="tiles">
{% for post in site.categories.SDG %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 SDG 的列出来-->