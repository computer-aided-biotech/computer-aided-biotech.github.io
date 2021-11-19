---
layout: page
title: News
permalink: /news/
---

<div class="container">
  {% for post in site.posts %}
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
  {% endfor %}
</div>