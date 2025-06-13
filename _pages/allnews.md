---
title: "News"
layout: textlay
excerpt: "Cheng Lab at Yale University"
sitemap: false
permalink: /allnews.html
---

# News



<ul>
  {% for article in site.data.news %}
    <li>
      <strong>{{ article.date }}</strong><br>
      {{ article.headline | markdownify }}
    </li>
  {% endfor %}
</ul>