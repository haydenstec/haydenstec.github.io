---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: "Home"
---

Under construction. Thank you for bearing with me.

<h2>News</h2>
<table style="width:100%; border-collapse: collapse;">
  <tbody>
    {% assign recent_news = site.news | sort: 'date' | reverse | limit: 5 %}
    {% for article in recent_news %}
      <tr>
        <td style="text-align: left; vertical-align: middle; padding: 10px; border: 1px solid #ddd;">
          <img src="{{ '/assets/images/' | append: article.category | append: '.png' }}" alt="{{ article.category }}" style="width:20px; height:20px; vertical-align: middle;">
            <strong>{{ article.date | date: "%m/%Y" }}:</strong> {{ article.description }}
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>

