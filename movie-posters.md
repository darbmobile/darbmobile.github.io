---
layout: page
title: Movie Posters
---

# Alternative Movie Posters

These are usually created using images from the brilliant [Movie Stills Database](https://www.moviestillsdb.com). It's an awesome resource for high resolution, film related images.

I also commonly use [Open Foundry](https://open-foundry.com) for typefaces. They really know how to present typefaces in a way that inspires instead of just creating decision fatigue like say, Google Fonts.

---

 {% for post in site.categories.posters %}
  <article>
    <h2>
      <a href="{{ post.url }}" class="post-title">
        {{ post.title }}
      </a>
    </h2>
    {{ post.content }}
  </article>
  <br>
{% endfor %}