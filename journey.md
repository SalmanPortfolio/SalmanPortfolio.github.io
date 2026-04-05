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

.active {
  display: block;
}

/* Inner Card */
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
    <button class="folder-btn" onclick="openArticle('a1')">📁 Admission</button>
    <button class="folder-btn" onclick="openArticle('a2')">📁 1st Semester</button>
    <button class="folder-btn" onclick="openArticle('a3')">📁 2nd Semester</button>
  </div>

  <!-- Admission -->
  <div id="a1" class="article-box">
    <h2>📂 Admission</h2>

    <div class="inner-card">
      <h3>📄 1st Article</h3>
      <h4>From Uncertainty to Innovation: My Journey into Computer Engineering</h4>

      <button class="read-btn" onclick="toggleArticle()">Read Full Article</button>

      <div id="fullArticle" style="display:none; margin-top:15px;">

        <h5>1. Searching for Direction in Pre-Medical Studies</h5>
        <p>
        My academic journey began with F.Sc Pre-Medical, a decision shaped more by expectation than personal understanding...
        </p>

        <p>
        The learning process felt repetitive and heavily focused on memorization rather than creativity...
        </p>

        <h5>2. The Turning Point: Challenges, Risks, and Persistence</h5>
        <p>
        A major turning point came when a friend encouraged me to attempt the ECAT entry test...
        </p>

        <p>
        Choosing to apply became one of the most difficult decisions of my journey...
        </p>

        <h5>3. Discovering Purpose Through Computer Engineering</h5>
        <p>
        My persistence was finally rewarded when I secured admission to UET Faisalabad in Computer Engineering...
        </p>

        <p>
        Looking back, I realize that my journey was not defined by perfect decisions but by continuous learning...
        </p>

      </div>

    </div>
  </div>

  <!-- Semester 1 -->
  <div id="a2" class="article-box">
    <h3>🎓 1st Semester</h3>
    <p>Add your semester content here.</p>
  </div>

  <!-- Semester 2 -->
  <div id="a3" class="article-box">
    <h3>💡 2nd Semester</h3>
    <p>Add your semester content here.</p>
  </div>

</div>

<script>
function openArticle(id){
  document.querySelectorAll('.article-box').forEach(a => a.style.display = 'none');
  document.getElementById(id).style.display = 'block';
}

function toggleArticle(){
  var x = document.getElementById("fullArticle");
  if(x.style.display === "none" || x.style.display === ""){
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
