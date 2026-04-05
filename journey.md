---
layout: page
title: My Journey
permalink: /journey/
---

# 🚀 My Journey

Click a folder to open article:

<div style="display:flex;gap:15px;flex-wrap:wrap;">

<button onclick="openArticle('a1')">📁 First Article</button>
<button onclick="openArticle('a2')">📁 1st Semester</button>
<button onclick="openArticle('a3')">📁 2nd Semester</button>

</div>

<hr>

<div id="a1" class="box">
<h3>First Article</h3>
<p>👉 Paste your article here later...</p>
</div>

<div id="a2" class="box">
<h3>1st Semester</h3>
<p>👉 Paste your semester content here...</p>
</div>

<div id="a3" class="box">
<h3>2nd Semester</h3>
<p>👉 Paste your semester content here...</p>
</div>

<style>
.box{
  display:none;
  border:1px solid #ccc;
  padding:10px;
  margin-top:10px;
}
</style>

<script>
function openArticle(id){
  document.getElementById('a1').style.display = "none";
  document.getElementById('a2').style.display = "none";
  document.getElementById('a3').style.display = "none";

  document.getElementById(id).style.display = "block";
}
</script>
