---
layout: default
title: 研报列表
lang: zh
---

# 春江量化研报列表

以下是我们的最新研报，请点击下载：

<ul>
{% for file in site.static_files %}
  {% if file.path contains '/static/' and file.extname == '.pdf' %}
    <li><a href="{{ file.path | relative_url }}">{{ file.basename }}</a></li>
  {% endif %}
{% endfor %}
</ul>

<p><a href="/Investment-Report/en/">Switch to English</a></p>