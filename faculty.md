---
layout: default
---

# 教員紹介

教員一覧を掲載しています。研究分野/研究内容/想定される卒業研究テーマなどの詳細情報もご覧いただけます。

{% assign sorted = site.faculty_members | sort: "kana" %}
{% for member in sorted %}
  <h2><a href="{{ member.url | relative_url }}">{{ member.name }} {{ member.eng_name }}</a></h2>
  {{ member.field }}
  <table>
    <tr>
      {% for key in member.keywords %}
        <td>{{ key }}</td>
      {% endfor %}
    </tr>
  </table>
{% endfor %}
