---
layout: default
permalink: /blog/
title: unsolicited
---

<div class="container">
  <header class="post-header">
    <h1 class="post-title">{{ site.blog_name }}</h1>
    <p class="desc">{{ site.blog_description }}</p>
  </header>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        {% if post.description %}<p>{{ post.description }}</p>{% endif %}
        <p class="post-meta">
          {{ post.date | date: "%B %-d, %Y" }}
          {%- if post.tags and post.tags.size > 0 %} &middot;
            {% for tag in post.tags %}<span class="tag">{{ tag }}</span>{% unless forloop.last %} {% endunless %}{% endfor %}
          {%- endif %}
        </p>
      </li>
    {% endfor %}
  </ul>
</div>
