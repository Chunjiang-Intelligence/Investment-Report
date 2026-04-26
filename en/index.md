---
layout: default
title: Research Reports
lang: en
---

# Chunjiang Quantitative Research Reports

Here are our latest research reports, please click to download:

<ul>
{% for file in site.static_files %}
  {% if file.path contains '/static/' and file.extname == '.pdf' %}
    <li><a href="{{ file.path | relative_url }}">{{ file.basename }}</a></li>
  {% endif %}
{% endfor %}
</ul>

<p><a href="/Investment-Report/zh/">切换到中文</a></p>