---
layout: default
title: Meet the Officers
permalink: /officers/
---

<!-- Top Title Banner -->
<div class="hero-black-box">
  <div>
    <h2>MEET THE OFFICERS</h2>
    <p class="hero-intro-text">
      Get to know the dedicated team behind the JALT Performance in Education Special Interest Group.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Detailed Bios Grid -->
<div class="officers-bio-grid">
  {% for officer in site.data.officers.detailed %}
    <div class="officer-bio-card">
      <h2>{{ officer.name }}</h2>
      <h3>{{ officer.role }}</h3>
      {% for paragraph in officer.bio %}
        <p>{{ paragraph }}</p>
      {% endfor %}
    </div>
  {% endfor %}
</div>

<!-- Compact Additional Officers Directory Grid -->
<h2 class="section-title">ADDITIONAL OFFICERS & ROLES</h2>

<div class="additional-officers-grid">
  {% for officer in site.data.officers.additional %}
    <div class="additional-officer-card">
      <strong>{{ officer.name }}</strong>
      <span>{{ officer.role }}</span>
    </div>
  {% endfor %}
</div>