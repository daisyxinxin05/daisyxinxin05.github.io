---
layout: default
---

# 欢迎来到我的花园

你好，世界。你好，思思。

这里是我记录生活与思考的地方。

---

## 最新文章
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>
