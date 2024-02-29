---
layout: default
---

# ニュース

<dl>
  {% for post in site.posts %}
    <dt>{{ post.date　| date: "%Y年%m月%d日" }}</dt>
    <dd>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </dd>
  {% endfor %}
</dl>
