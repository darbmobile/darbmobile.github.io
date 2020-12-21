---
layout: home
title: Home
---

# Hi, I'm Sam.

If you'd like to get in contact, you can using the form below. 

<form action="https://formspree.io/f/xeqplbla" method="POST">
  <input type="text" name="name" placeholder="Name">
  <input type="email" name="_replyto" placeholder="Email">
  <textarea name="message" placeholder="Your message"></textarea>
  <input type="submit" value="Send">
</form>

---

# Archive

### Blog

<div>
  {% for post in site.categories.blog %}
      <small class="small-date">{{ post.date | date: "%Y-%m-%d" }} »</small> <a href="{{ post.url }}">{{ post.title }}</a>
      <br>
  {% endfor %}
</div>

### Poster Designs

<div>
  {% for post in site.categories.posters %}
      <a href="{{ post.url }}">{{ post.title }}</a>
      <br>
  {% endfor %}
</div>