---
layout: default
---
<h1>Welcome to My Blog</h1>

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date_to_string }}</p>
  {{ post.excerpt }}
{% endfor %}
