---
layout: home
title: 首页
---

# 欢迎访问我的博客

这里是我的个人博客，分享我的想法和经验。

## 最新文章

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%Y-%m-%d" }}</p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>