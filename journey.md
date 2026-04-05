---
layout: page
title: My Journey
permalink: /journey/
---

# My Journey

<div class="folders">
  <button onclick="openArticle('a1')">📁 First Article</button>
  <button onclick="openArticle('a2')">📁 1st Semester</button>
  <button onclick="openArticle('a3')">📁 2nd Semester</button>
</div>

<div id="a1" class="article-box">
  <h3>First Article</h3>
  <p>👉 Paste your content here later...</p>
</div>

<div id="a2" class="article-box">
  <h3>1st Semester</h3>
  <p>👉 Paste your 1st semester content...</p>
</div>

<div id="a3" class="article-box">
  <h3>2nd Semester</h3>
  <p>👉 Paste your 2nd semester content...</p>
</div>

<style>
.folders button{
  background:#3498db; color:white; border:none; padding:10px 15px; border-radius:5px;
  margin:5px; cursor:pointer; transition:0.3s;
}
.folders button:hover{ background:#2980b9; }
.article-box{ display:none; border:1px solid #ccc; padding:15px; margin-top:10px; border-radius:5px; background:#f8f8f8; }
</style>

<script>
function openArticle(id){
  ['a1','a2','a3'].forEach(function(e){document.getElementById(e).style.display='none';});
  document.getElementById(id).style.display='block';
}
</script>
