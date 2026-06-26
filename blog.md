---
layout: page
title: Blog
permalink: /blog/
---

<style>
body { background: #f8f9fa; }

.blog-wrapper {
  max-width: 760px;
  margin: 0 auto;
  padding: 20px 20px 60px;
}

.blog-header {
  text-align: center;
  margin-bottom: 30px;
}
.blog-header h1 {
  font-size: 26px;
  font-weight: 600;
  color: #111;
  margin-bottom: 6px;
}
.blog-header p {
  font-size: 14px;
  color: #6b7280;
}

/* Filter tabs */
.filter-bar {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
  margin-bottom: 24px;
}
.filter-btn {
  padding: 6px 16px;
  border-radius: 20px;
  border: 1px solid #e5e7eb;
  background: #fff;
  color: #6b7280;
  font-size: 13px;
  cursor: pointer;
  transition: all 0.2s;
}
.filter-btn:hover, .filter-btn.active {
  background: #2563eb;
  color: #fff;
  border-color: #2563eb;
}

/* Post Cards */
.post-card {
  background: #fff;
  border: 1px solid #e5e7eb;
  border-radius: 14px;
  padding: 22px 24px;
  margin-bottom: 16px;
  transition: all 0.2s;
}
.post-card:hover {
  border-color: #93c5fd;
  box-shadow: 0 4px 16px rgba(37,99,235,0.08);
  transform: translateY(-2px);
}
.post-card h2 {
  font-size: 17px;
  font-weight: 600;
  margin: 0 0 8px;
}
.post-card h2 a {
  color: #111;
  text-decoration: none;
}
.post-card h2 a:hover {
  color: #2563eb;
}
.post-card .excerpt {
  font-size: 14px;
  color: #6b7280;
  line-height: 1.6;
  margin-bottom: 12px;
}
.post-footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 8px;
}
.post-tags { display: flex; gap: 6px; flex-wrap: wrap; }
.tag {
  display: inline-block;
  background: #eff6ff;
  color: #2563eb;
  font-size: 11px;
  padding: 3px 10px;
  border-radius: 10px;
}
.post-date {
  font-size: 12px;
  color: #9ca3af;
}
.read-link {
  font-size: 13px;
  color: #2563eb;
  text-decoration: none;
  font-weight: 500;
}
.read-link:hover { text-decoration: underline; }

.no-posts {
  text-align: center;
  padding: 50px 20px;
  color: #9ca3af;
  border: 1px dashed #e5e7eb;
  border-radius: 14px;
}
</style>

<div class="blog-wrapper">

  <div class="blog-header">
    <h1>📝 My Blog</h1>
    <p>Experiences, lessons, and reflections from my Computer Engineering journey at UET Lahore.</p>
  </div>

  <div class="filter-bar">
    <button class="filter-btn active" onclick="filterPosts('all', this)">All Posts</button>
    <button class="filter-btn" onclick="filterPosts('student-life', this)">Student Life</button>
    <button class="filter-btn" onclick="filterPosts('database', this)">Database</button>
    <button class="filter-btn" onclick="filterPosts('programming', this)">Programming</button>
    <button class="filter-btn" onclick="filterPosts('Dr-Bilal-Ahmad', this)">Dr. Bilal Ahmad</button>
  </div>

  {% if site.posts.size > 0 %}
    {% for post in site.posts %}
    <div class="post-card" data-tags="{{ post.tags | join: ' ' | downcase }}">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p class="excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <div class="post-footer">
        <div class="post-tags">
          {% for tag in post.tags limit:3 %}
            <span class="tag">{{ tag }}</span>
          {% endfor %}
        </div>
        <span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>
        <a href="{{ post.url }}" class="read-link">Read more →</a>
      </div>
    </div>
    {% endfor %}
  {% else %}
    <div class="no-posts">
      <p style="font-size:16px;margin-bottom:8px;">Posts coming soon!</p>
      <p style="font-size:13px;">Check back shortly for articles from my semester.</p>
    </div>
  {% endif %}

</div>

<script>
function filterPosts(tag, btn) {
  document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  document.querySelectorAll('.post-card').forEach(card => {
    if (tag === 'all' || card.dataset.tags.includes(tag)) {
      card.style.display = 'block';
    } else {
      card.style.display = 'none';
    }
  });
}
</script>
