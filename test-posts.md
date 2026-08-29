---
layout: default
permalink: /test-posts/
---
<h2>All Posts (Without Pagination)</h2>
<ul>
  {% for post in site.posts %}
    <li>{{ post.title }}</li>
  {% endfor %}
</ul>
