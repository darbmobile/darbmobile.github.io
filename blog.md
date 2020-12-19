---
layout: page
title: Movie Posters
---

# Blog

Usually thoughts on films.

---



  {% for post in site.categories.blog %}
  <article>
    <h2>
      <a href="{{ post.url }}" class="post-title">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}" class="post-date">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}