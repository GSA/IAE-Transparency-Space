---
published: true
layout: blog
navigation: blog
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="/iae-global/{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
