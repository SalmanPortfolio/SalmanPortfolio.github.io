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

      <h5>1. Searching for Direction in Pre-Medical Studies</h5>
      <p>
      My academic journey began with F.Sc Pre-Medical, a decision shaped more by expectation than personal understanding. Like many students, I selected this field without fully exploring my interests or long-term goals. At the time, it seemed like a safe and respected academic path, but as my studies progressed, I realized something was missing. Although I worked hard and remained dedicated to my coursework, I struggled to feel genuinely connected to the subjects.

      The learning process felt repetitive and heavily focused on memorization rather than creativity or logical exploration. I often found myself questioning whether I truly belonged in this field. While my classmates appeared confident about becoming doctors or pursuing medical careers, I felt uncertain about my own future. Those two years became a period of self-reflection, where I slowly recognized that success is not only about effort but also about alignment between passion and purpose. This realization planted the first seeds of change, even though I did not yet know where my path would lead.
      </p>

      <h5>2. The Turning Point: Challenges, Risks, and Persistence</h5>
      <p>
      A major turning point came when a friend encouraged me to attempt the ECAT entry test. Initially, I treated it as an experiment rather than a serious career decision. Without preparation, I appeared for the exam simply to understand its structure and difficulty. My performance was not strong, but the experience introduced me to analytical thinking and problem-solving — skills that immediately captured my interest.

      Curious about this new direction, I attempted ECAT again with greater seriousness. Despite improved effort, my score remained lower than expected, which deeply affected my confidence. I began to doubt my abilities and decided not to apply for admission, believing that my chances were limited. However, life presented an unexpected opportunity when admissions reopened, offering students a second chance.

      Choosing to apply became one of the most difficult decisions of my journey. The process itself was filled with obstacles: technical issues, slow websites, network failures, and increasing deadline pressure. At the same time, emotional stress at home due to my results made the situation even more challenging. Yet, instead of giving up, I continued working persistently. Late nights and repeated attempts tested my patience, but they also strengthened my determination. That phase taught me an important lesson — resilience is built during moments when quitting feels easier than continuing.
      </p>

      <h5>3. Discovering Purpose Through Computer Engineering</h5>
      <p>
      My persistence was finally rewarded when I secured admission to UET Faisalabad in Computer Engineering. This achievement marked more than academic success; it symbolized clarity after years of uncertainty. For the first time, I felt excited about learning. Subjects involving technology, logic, and innovation aligned naturally with my interests and abilities.

      As I progressed in my studies, I began to see education differently. Computer Engineering allowed me to think creatively while solving real-world problems, combining technical knowledge with analytical reasoning. The field challenged me to grow intellectually and personally, transforming my earlier doubts into confidence.

      Looking back, I realize that my journey was not defined by perfect decisions but by continuous learning and adaptation. Moving from pre-medical confusion to engineering clarity taught me that failure and uncertainty are not obstacles but essential steps toward growth. Today, I carry forward the lessons of perseverance, self-belief, and courage to take risks. My journey reminds me that sometimes the path we never planned becomes the one that leads us exactly where we are meant to be.
      </p>

    </div>
  </div>

  <!-- Semester 1 -->
  <div id="a2" class="article-box">
    <h3>🎓 1st Semester</h3>

    <div class="inner-card">
      <h4>📄 2nd Article</h4>
      <h5>My First Days at University: Challenges, Discovery, and Growth</h5>

      <h5>1. Arrival and First Impressions</h5>
      <p>
      On September 5, 2025, I arrived at UET Faisalabad, full of excitement but uncertain about what awaited me. Being new to the city, I had no idea where the campus, hostel, or classrooms were located. The large university and unfamiliar surroundings made the first few hours overwhelming. Despite this, I was determined to embrace this new chapter in my life.

      The first challenge was navigating registration and the campus layout. Visiting a nearby café with other students helped me connect with peers facing similar experiences. Sharing stories and guidance created a sense of community, which eased the initial anxiety and gave me my first taste of university life.
      </p>

      <h5>2. Adapting to University Life</h5>
      <p>
      Hostel life and the first day of classes presented practical challenges. Facilities were not always organized, schedules were confusing, and I had to learn to manage my time efficiently. Orientation sessions with senior students tested our knowledge and problem-solving skills. Making friends helped me navigate the campus, understand rules, and adjust to academic expectations more easily.
      </p>

      <h5>3. Growth Through Challenges</h5>
      <p>
      By the end of the first week, I realized that each difficulty — from finding classrooms to managing daily routines — was strengthening my adaptability and independence. These experiences taught me patience, persistence, and responsibility. Looking back, those early days of uncertainty shaped my resilience, preparing me for future academic and personal growth at university.
      </p>
    </div>
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
</script>
