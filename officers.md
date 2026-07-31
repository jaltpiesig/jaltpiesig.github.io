---
layout: default
title: Meet the Officers
---
## PIE SIG Officers (2026)

<div class="officer-grid">
  {% for officer in site.data.officers %}
    <div class="officer-card">
      <img src="{{ officer.image }}" alt="{{ officer.name }}" class="profile-circle">
      <h3>{{ officer.name }}</h3>
      <h4>{{ officer.role }}</h4>
      <p>{{ officer.bio }}</p>
    </div>
  {% endfor %}
</div>