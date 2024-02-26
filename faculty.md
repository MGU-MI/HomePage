---
layout: default
---

# 教員紹介

教員一覧を掲載しています。
研究分野/研究内容/想定される卒業研究テーマなどの詳細情報もご覧いただけます。

{% for member in site.faculty_members %}
<h1>{{ member.name }}</h1>
<h2>{{ member.eng_name }}</h2>
<h3>学位</h3>
{{ member.degree }}
<h3>研究分野</h3>
{% endfor %}
