---
layout: page
title: About Me
---

<section class="education">
  <h2>Education</h2>
  {% for edu in site.education %}
  <div class="education-item">
    <h3>{{ edu.university }}</h3>
    <p>{{ edu.degree }}</p>
    <p>
      {% if edu.cgpa %}CGPA: {{ edu.cgpa }}{% endif %}
      {% if edu.percentage %}Percentage: {{ edu.percentage }}{% endif %}
    </p>
    <p class="duration">{{ edu.duration }}</p>
  </div>
  {% endfor %}
</section>

<section class="skills">
  <h2>Technical Skills</h2>
  <div class="skills-grid">
    <div class="skill-category">
      <h3>Languages</h3>
      <ul>
        <li>Python</li>
        <li>C/C++</li>
        <li>JavaScript</li>
        <li>HTML/CSS</li>
        <li>Arduino</li>
      </ul>
    </div>
    
    <div class="skill-category">
      <h3>Libraries</h3>
      <ul>
        <li>PyTorch</li>
        <li>OpenCV</li>
        <li>Pandas/NumPy</li>
        <li>scikit-learn</li>
        <li>Ultralytics</li>
      </ul>
    </div>
    
    <div class="skill-category">
      <h3>Frameworks</h3>
      <ul>
        <li>React</li>
        <li>Node.js</li>
        <li>Express</li>
        <li>MongoDB</li>
      </ul>
    </div>
  </div>
</section>
