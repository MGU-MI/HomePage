---
layout: default
---

# 教員紹介

教員一覧を掲載しています。
研究分野/研究内容/想定される卒業研究テーマなどの詳細情報もご覧いただけます。

{% for member in site.faculty_members %}
  <h2>{{ member.name }} / {{ member.eng_name }}</h2>
  {{ member.field }}
  {{ member.keywords }}
{% endfor %}
