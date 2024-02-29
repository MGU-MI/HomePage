---
layout: default
---

# 教員紹介

教員一覧を掲載しています。研究分野/研究内容/想定される卒業研究テーマなどの詳細情報もご覧いただけます。

{% assign sorted = site.faculty_members | sort: "kana" %}
{% for member in sorted %}
  <div class="mi-member-box">
    <img src="{{ member.photo  | relative_url }}" width="100px">
    <div class="mi-member-text">
      <h3><a href="{{ member.url | relative_url }}">{{ member.name }} {{ member.eng_name }}</a></h3>
      <h4>{{ member.field }}</h4>
      {% for key in member.keywords %}
        <span class="mi-keywords">{{ key }}</span>
      {% endfor %}
    </div>
  </div>
{% endfor %}
