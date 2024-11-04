---
layout: default  # Ensure this points to a valid layout
title: "News"
---

# News

<ul>
  {% for item in site.news %}
    <li>
      <a href="{{ item.url }}">{{ item.title }}</a> - <small>{{ item.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>