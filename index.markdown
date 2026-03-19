---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

# Tianyi Xie

[About](/about/)

<ul>
    {% for post in site.posts %}
      {% if post.categories contains "Public" %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a> - <time datetime="{{ post.date }}">{{ post.date | date: "%B %d, %Y" }}</time>
        </li>
      {% endif %}
    {% endfor %}
  </ul>