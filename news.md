---
layout: page
title: News
---

News and updates from Bath IFG.

<ul>
  {% for post in site.posts %}
    <li>
      <strong>{{ post.date | date: "%-d %B %Y" }}</strong><br>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


