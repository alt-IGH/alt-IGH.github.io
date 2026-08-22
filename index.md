---
layout: default
title: hi
---

# 📝 

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span style="color: #666; font-size: 0.9rem;">
        ({{ post.date | date: "%Y年%m月%d日" }})
      </span>
    </li>
  {% endfor %}
</ul>

<p style="margin-top: 2rem; color: #888; font-size: 0.9rem;">
  共 {{ site.posts | size }} 篇文章
</p>
