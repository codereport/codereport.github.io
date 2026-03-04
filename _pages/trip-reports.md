---
layout: page
permalink: /trip-reports/
title: Trip Reports
---

<div class="posts">
  {% for post in site.categories["Trip Report"] %}
  <a href="{{ site.baseurl }}{{ post.url }}" class="post-listing">
    <span class="post-listing-title">{{ post.title }}</span>
    <span class="post-listing-date">{{ post.date | date: "%B %e, %Y" }}</span>
  </a>
  {% endfor %}
</div>
