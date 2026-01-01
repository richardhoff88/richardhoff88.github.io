---
layout: page
permalink: /
title: Home
---

## Latest Blog Posts

{% for post in site.posts limit:3 %}
<div class="card mb-4">
  <div class="card-body">
    <h3 class="card-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
    <p class="card-text">
      <small class="text-muted">
        {{ post.date | date: "%B %-d, %Y" }}
        {% if post.read_time %} • {{ post.read_time }} min read{% endif %}
      </small>
    </p>
    {% if post.description %}
      <p class="card-text">{{ post.description }}</p>
    {% endif %}
    <a href="{{ post.url | relative_url }}" class="btn btn-primary">Read More</a>
  </div>
</div>
{% endfor %}

<div class="text-right">
  <a href="{{ '/blog/' | relative_url }}" class="btn btn-outline-primary">View All Posts</a>
</div>
