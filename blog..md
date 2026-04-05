---
layout: page
title: Blog
permalink: /blog/
---

<style>
.blog-container {
  max-width: 1000px;
  margin: auto;
  padding: 20px;
}

.post-card {
  background: #111a3a;
  padding: 20px;
  border-radius: 15px;
  margin-bottom: 20px;
  box-shadow: 0 10px 25px rgba(255,0,0,0.2);
  transition: 0.3s;
}

.post-card:hover {
  transform: translateY(-5px);
}

.post-title {
  color: #ff2e2e;
}

.tag {
  display: inline-block;
  background: #ff0000;
  padding: 5px 10px;
  margin: 5px;
  border-radius: 20px;
  font-size: 12px;
}
</style>

<div class="blog-container">

<h1>📝 My Blog</h1>

{% for post in site.posts %}
<div class="post-card">

  <h2 class="post-title">
    <a href="{{ post.url }}">{{ post.title }}</a>
  </h2>

  <p>{{ post.description }}</p>

  <div>
    {% for tag in post.tags %}
      <span class="tag">{{ tag }}</span>
    {% endfor %}
  </div>

</div>
{% endfor %}

</div>
