---
layout: default
---

## Hi, I'm Carrie.

I am a student in the Master of Data Science program at the University of British Columbia and ~~will make it out alive~~ graduate in July 2019.

This is a compilation of my thoughts on data science-related (and not so related) topics by day, and a personal blog of my journey as a Data Scientist by night.

Shameless Self-Plug-Type Stuff:
[My LinkedIn](https://ca.linkedin.com/in/ccheung2)
[My GitHub](https://github.com/carrieklc)

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
  {% endfor %}
</ul>
