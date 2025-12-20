---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

# Tianyi Xie

[About](/about/)

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span>({{ post.date | date: "%Y-%m-%d" }})</span>
    </li>
  {% endfor %}
</ul>