---
layout: default
title: 首页
---

<h2>文章列表</h2>
<ul class="post-list">
{% for post in site.posts %}
    <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
{% endfor %}
</ul>