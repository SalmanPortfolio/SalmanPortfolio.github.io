---
layout: page
title: My Journey
permalink: /journey/
---

# My Journey

<div class="folders">
  <button onclick="openArticle('a1')">📁 Admission</button>
  <button onclick="openArticle('a2')">📁 1st Semester</button>
  <button onclick="openArticle('a3')">📁 2nd Semester</button>
</div>

<div id="a1" class="article-box">
  <h3>Admission</h3>
  <p>👉 Paste your first article content here.</p>
</div>

<div id="a2" class="article-box">
  <h3>1st Semester</h3>
  <p>👉 Paste 1st semester content here.</p>
</div>

<div id="a3" class="article-box">
  <h3>2nd Semester</h3>
  <p>👉 Paste 2nd semester content here.</p>
</div>

<style>
.folders button{
  background:#3498db; color:#fff; border:none; padding:12px 18px; border-radius:6px; margin:5px; cursor:pointer; transition:0.3s;
}
.folders button:hover{background:#2980b9; transform:scale(1.05);}
.article-box{display:none; border:1px solid #555; padding:15px; margin-top:10px; border-radius:5px; background:#1e1e1e; color:#eee;}
@media screen and (max-width:480px){.folders button{width:100%; margin:5px 0;}}
</style>

<script>
function openArticle(id){
  ['a1','a2','a3'].forEach(function(e){document.getElementById(e).style.display='none';});
  document.getElementById(id).style.display='block';
}
</script>
