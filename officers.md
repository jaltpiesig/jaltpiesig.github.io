---
layout: default
title: Officers
permalink: /officers/
---

<!-- Hero Banner -->
<div class="hero-black-box mb-35">
  <div>
    <h2>PIE SIG OFFICERS</h2>
    <p class="hero-intro-text">
      Meet the dedicated team of officers driving the Performance in Education SIG across Japan and beyond.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Section 1: Executive Officers -->
<section class="mb-40">
  <h2 class="section-title">Executive Officers</h2>
  <div class="officers-grid">
    {% for officer in site.data.officers.executives %}
      <div class="officer-card">
        <span class="officer-role">{{ officer.role }}</span>
        <h3 class="officer-name">{{ officer.name }}</h3>
        {% if officer.affiliation %}
          <div class="officer-affiliation">{{ officer.affiliation }}</div>
        {% endif %}
        {% if officer.bio %}
          <p class="officer-bio">{{ officer.bio }}</p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>

<!-- Section 2: General & Regional Officers -->
<section class="mb-40">
  <h2 class="section-title">Officers & Coordinators</h2>
  <div class="officers-grid">
    {% for officer in site.data.officers.general %}
      <div class="officer-card">
        <span class="officer-role">{{ officer.role }}</span>
        <h3 class="officer-name">{{ officer.name }}</h3>
        {% if officer.affiliation %}
          <div class="officer-affiliation">{{ officer.affiliation }}</div>
        {% endif %}
        {% if officer.bio %}
          <p class="officer-bio">{{ officer.bio }}</p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>

<!-- Section 3: Joining / Contact Callout -->
<div class="res-callout-box">
  <h3 class="res-callout-title">Interested in Joining the Team?</h3>
  <p class="res-callout-text">
    PIE SIG is always looking for enthusiastic educators to help organize events, curate publications, or manage communications. Reach out through our social media channels or contact any officer at an upcoming JALT conference!
  </p>
</div>