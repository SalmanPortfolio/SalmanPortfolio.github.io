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
  <p>Content goes here.</p>
</div>

<div id="a2" class="article-box">
  <h3>1st Semester</h3>
  <p>Content goes here.</p>
</div>

<div id="a3" class="article-box">
  <h3>2nd Semester</h3>
  <p>Content goes here.</p>
</div>

<script>
function openArticle(id){
  ['a1','a2','a3'].forEach(function(e){document.getElementById(e).style.display='none';});
  document.getElementById(id).style.display='block';
}
</script>
