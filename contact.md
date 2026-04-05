---
layout: page
title: Contact
permalink: /contact/
---

<style>
body {
  background: #0a0f2c;
  color: #ffffff;
  font-family: 'Segoe UI', sans-serif;
}

/* Container */
.contact-container {
  max-width: 800px;
  margin: auto;
  padding: 20px;
}

/* Card */
.contact-card {
  background: #111a3a;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(255,0,0,0.25);
  transition: 0.3s;
}

.contact-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 35px rgba(255,0,0,0.4);
}

/* Heading */
h1 {
  color: #ff2e2e;
  margin-bottom: 15px;
}

/* Info Items */
.info {
  margin: 15px 0;
  font-size: 16px;
}

/* Links */
a {
  color: #ff4d4d;
  text-decoration: none;
  font-weight: bold;
}

a:hover {
  text-decoration: underline;
}

/* Button Style (WhatsApp Highlight) */
.whatsapp-btn {
  display: inline-block;
  margin-top: 10px;
  padding: 10px 18px;
  border-radius: 25px;
  background: linear-gradient(45deg, #ff0000, #8b0000);
  color: white;
  text-decoration: none;
  transition: 0.3s;
}

.whatsapp-btn:hover {
  transform: scale(1.05);
  background: linear-gradient(45deg, #ff4d4d, #ff0000);
}

/* Divider */
hr {
  border: 1px solid #ff2e2e;
  margin: 20px 0;
}
</style>

<div class="contact-container">

  <h1>📞 Contact Me</h1>
  <hr>

  <div class="contact-card">

    <div class="info">
      📍 <strong>Address:</strong><br>
      8/14L Kassowal, Tehsil Chichawatni, District Sahiwal
    </div>

    <div class="info">
      📞 <strong>Phone / WhatsApp:</strong><br>
      <a href="https://wa.me/923024927525" target="_blank">0302-4927525</a><br>
      <a href="https://wa.me/923024927525" target="_blank" class="whatsapp-btn">
        💬 Chat on WhatsApp
      </a>
    </div>

    <div class="info">
      📧 <strong>Email:</strong><br>
      <a href="mailto:salmanzahoor.uet@example.com">
        salmanzahoor.uet@example.com
      </a>
    </div>

  </div>

</div>
