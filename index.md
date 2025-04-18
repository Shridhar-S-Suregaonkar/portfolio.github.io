---
layout: home
title: Shridhar Suregaonkar
subtitle: Computer Science Engineer | Researcher | Developer
---

<div class="profile-section">
  <div class="profile-text">
    <h1>{{ page.title }}</h1>
    <h2>{{ page.subtitle }}</h2>
    <p>Currently pursuing BE in Computer Science at KLE Technological University</p>
  </div>
</div>

<section class="featured-projects">
  <h2>Featured Projects</h2>
  <div class="projects-grid">
    {% for project in site.projects limit:3 %}
    <div class="project-card">
      <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
      <div class="technologies">
        {% for tech in project.technologies %}
        <span class="tech-tag">{{ tech }}</span>
        {% endfor %}
      </div>
      {{ project.excerpt }}
    </div>
    {% endfor %}
  </div>
  <a href="{{ '/projects' | relative_url }}" class="btn">View All Projects</a>
</section>
