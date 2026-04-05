---
layout: page
title: About
permalink: /about/
---

<style>
body {
  background: #0a0f2c;
  color: #ffffff;
  font-family: 'Segoe UI', sans-serif;
}

/* Container */
.about-container {
  max-width: 900px;
  margin: auto;
  padding: 20px;
}

/* Card Style */
.card {
  background: #111a3a;
  border-radius: 15px;
  padding: 20px;
  margin-bottom: 20px;
  box-shadow: 0 5px 20px rgba(255, 0, 0, 0.2);
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 30px rgba(255, 0, 0, 0.4);
}

/* Title */
h1, h2, h3 {
  color: #ff2e2e;
}

/* Button */
.btn {
  background: linear-gradient(45deg, #ff0000, #8b0000);
  border: none;
  padding: 10px 18px;
  color: white;
  border-radius: 25px;
  cursor: pointer;
  transition: 0.3s;
  margin-top: 10px;
}

.btn:hover {
  background: linear-gradient(45deg, #ff4d4d, #ff0000);
  transform: scale(1.05);
}

/* Image */
.result-img {
  width: 100%;
  max-width: 400px;
  border-radius: 10px;
  margin-top: 10px;
  border: 2px solid #ff2e2e;
}

/* Divider */
hr {
  border: 1px solid #ff2e2e;
  margin: 20px 0;
}
</style>

<div class="about-container">

  <div class="card">
    <h1>👤 About Me</h1>
    <p>
      I am <strong>Salman Zahoor</strong>, son of <strong>Zahoor Ahmad</strong>, 
      a passionate <strong>Computer Engineering student</strong>.
    </p>
  </div>

  <div class="card">
    <h2>🎓 Education</h2>

    <!-- Matric -->
    <div class="card">
      <h3>Matric</h3>
      <p><strong>The Educators School, Kassowal Campus</strong></p>
      <button class="btn" onclick="toggle('matric')">View Result</button>
      <div id="matric" style="display:none;">
        <img src="/assets/images/matric.jpg" class="result-img">
      </div>
    </div>

    <!-- FSC -->
    <div class="card">
      <h3>F.Sc Pre-Medical</h3>
      <p><strong>Superior Group of Colleges, Mian Channu Campus</strong></p>
      <button class="btn" onclick="toggle('fsc')">View Result</button>
      <div id="fsc" style="display:none;">
        <img src="/assets/images/fsc.jpg" class="result-img">
      </div>
    </div>

    <!-- University -->
    <div class="card">
      <h3>University</h3>
      <p><strong>UET Lahore, Faisalabad Campus</strong></p>
      <p>Computer Engineering</p>
    </div>

  </div>

</div>

<script>
function toggle(id){
  var x = document.getElementById(id);
  if (x.style.display === "none" || x.style.display === "") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
