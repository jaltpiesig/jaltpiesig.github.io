---
layout: default
title: Best of PIE SIG
permalink: /best-of-pie/
---

<!-- Hero Header -->
<div class="hero-black-box">
  <div>
    <h2>BEST OF PIE SIG</h2>
    <p class="hero-intro-text">
      Recognizing excellence in Performance in Education presentations, workshops, and student performances over the past decade.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Intro Card -->
<div class="awards-intro-card">
  <p>
    PIE SIG has been giving awards for over 10 years to PIE SIG presenters who have demonstrated excellence in their presentations. Some of these individuals and their contributions have been recognized through JALT's <strong>Michele Steele Best of JALT Awards</strong>, and others through our own <strong>PIE SIG Best Presentation, Best Performance, and Best Student Performance awards</strong>.
  </p>
</div>

<!-- Grid Layout for Award Categories -->
<div class="awards-grid">

  <!-- Section 1: Best of JALT Awards -->
  <div class="awards-card">
    <h2 class="awards-card-title">PIE SIG Best of JALT Awards</h2>
    <ul class="awards-list">
      {% for award in site.data.awards.best_of_jalt %}
        <li>
          <strong>{{ award.year }}:</strong> {{ award.recipient }}
          {% if award.title != "" %}
            — <em>{{ award.title }}</em>
          {% endif %}
        </li>
      {% endfor %}
    </ul>
  </div>

  <!-- Section 2: Presentation and Performance Awards -->
  <div class="awards-card">
    <h2 class="awards-card-title">PIE SIG Presentation & Performance Awards</h2>
    {% for item in site.data.awards.presentation_and_performance %}
      <div class="award-sub-block">
        <h3>{{ item.category }}</h3>
        <p><strong>{{ item.year }}:</strong> {{ item.recipient }}</p>
      </div>
    {% endfor %}
  </div>

</div>