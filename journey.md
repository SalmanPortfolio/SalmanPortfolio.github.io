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
}

.folder-btn:hover {
  transform: scale(1.08);
}

/* Article Box */
.article-box {
  display: none;
  background: #111a3a;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(255,0,0,0.2);
  animation: fadeIn 0.4s ease-in-out;
}

.inner-card {
  background: #0f1735;
  padding: 20px;
  border-radius: 12px;
  margin-top: 15px;
  box-shadow: 0 5px 15px rgba(255,0,0,0.2);
}

/* Headings */
h1, h2, h3 {
  color: #ff2e2e;
}

.inner-card h4 {
  color: #ff4d4d;
}

.inner-card h5 {
  color: #ff2e2e;
  margin-top: 15px;
}

/* Button */
.read-btn {
  margin-top: 10px;
  padding: 10px 18px;
  border-radius: 25px;
  border: none;
  background: linear-gradient(45deg, #ff0000, #8b0000);
  color: white;
  cursor: pointer;
  transition: 0.3s;
}

.read-btn:hover {
  transform: scale(1.05);
}

/* Animation */
@keyframes fadeIn {
  from {opacity: 0; transform: translateY(10px);}
  to {opacity: 1; transform: translateY(0);}
}
</style>

<div class="journey-container">

  <h1>🚀 My Journey</h1>

  <!-- Folders -->
  <div class="folders">
    <button class="folder-btn" onclick="openArticle('admission')">📁 Admission</button>
    <button class="folder-btn" onclick="openArticle('sem1')">📁 1st Semester</button>
    <button class="folder-btn" onclick="openArticle('sem2')">📁 2nd Semester</button>
  </div>

  <!-- Admission -->
  <div id="admission" class="article-box">
    {% include 1st_article.html %}
  </div>

  <!-- 1st Semester -->
  <div id="sem1" class="article-box">
    {% include 2nd_article.html %}
    {% include 3rd_article.html %}
    {% include 4th_article.html %}
    {% include 5th_article.html %}
    {% include 6th_article.html %}
    {% include 7th_article.html %}
    {% include 8th_article.html %}
  </div>

  <!-- 2nd Semester -->
  <div id="sem2" class="article-box">
    <p>Content for 2nd semester will go here.</p>
  </div>

</div>

<script>
function openArticle(id){
  document.querySelectorAll('.article-box').forEach(a => a.style.display = 'none');
  document.getElementById(id).style.display = 'block';
}

function toggleArticle(articleId){
  var x = document.getElementById(articleId);
  if(x.style.display === "none" || x.style.display === ""){
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
