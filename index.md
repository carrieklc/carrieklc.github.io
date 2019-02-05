---
layout: default
---

<ul>
  {% for post in site.pages%}
    {% if post.tags == "post" %}
      <a href="{{ post.url }}">
        <H1>{{ post.title }}</H1>
      </a>
      &nbsp; <em>{{ post.date | date_to_long_string }}</em>
      <p><div>{{ post.content |truncatehtml | truncatewords: 181 | markdownify }}<a href="{{ post.url }}">Read More</a> </div></p>
    {% endif %}
  {% endfor %}
</ul>


[home](https://carrieklc.github.io)
