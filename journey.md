---
layout: page
title: My Journey
permalink: /journey/
---

<style>
body {
  background: #0a0f2c;
  color: #ffffff;
  font-family: 'Segoe UI', sans-serif;
}

/* Container */
.journey-container {
  max-width: 1000px;
  margin: auto;
  padding: 20px;
}

/* Folder Buttons */
.folders {
  display: flex;
  gap: 15px;
  flex-wrap: wrap;
  margin-bottom: 20px;
}

.folder-btn {
  background: linear-gradient(45deg, #ff0000, #8b0000);
  border: none;
  padding: 12px 20px;
  color: white;
  border-radius: 30px;
  cursor: pointer;
  transition: 0.3s;
  box-shadow: 0 5px 15px rgba(255,0,0,0.3);
}

.folder-btn:hover {
  transform: scale(1.08);
  background: linear-gradient(45deg, #ff4d4d, #ff0000);
}

/* Article Cards */
.article-box {
  display: none;
  background: #111a3a;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(255,0,0,0.2);
  animation: fadeIn 0.4s ease-in-out;
}

/* Active Card */
.active {
  display: block;
}

/* Heading Colors */
h1, h3 {
  color: #ff2e2e;
}

/* Animation */
@keyframes fadeIn {
  from {opacity: 0; transform: translateY(10px);}
  to {opacity: 1; transform: translateY(0);}
}

/* Divider */
hr {
  border: 1px solid #ff2e2e;
  margin: 20px 0;
}
</style>

<div class="journey-container">

  <h1>🚀 My Journey</h1>
  <hr>

  <div class="folders">
    <button class="folder-btn" onclick="openArticle('a1')">📁 First Article</button>
    <button class="folder-btn" onclick="openArticle('a2')">📁 1st Semester</button>
    <button class="folder-btn" onclick="openArticle('a3')">📁 2nd Semester</button>
  </div>

  <!-- Article 1 -->
  <div id="a1" class="article-box">
    <h3>📌 First Article</h3>
    <p>
      This is your first journey article. You can write about your starting phase,
      motivation, and how you entered the field of Computer Engineering.
    </p>
  </div>

  <!-- Article 2 -->
  <div id="a2" class="article-box">
    <h3>🎓 1st Semester</h3>
    <p>
      Share your experience of first semester, subjects, challenges, and what you learned.
    </p>
  </div>

  <!-- Article 3 -->
  <div id="a3" class="article-box">
    <h3>💡 2nd Semester</h3>
    <p>
      Describe your growth, projects, skills improvement, and achievements.
    </p>
  </div>

</div>

<script>
function openArticle(id){
  const articles = document.querySelectorAll('.article-box');
  articles.forEach(a => a.classList.remove('active'));
  document.getElementById(id).classList.add('active');
}
</script>
