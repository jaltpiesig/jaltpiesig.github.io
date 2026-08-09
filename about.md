---
layout: default
title: About Us
permalink: /about/
---

<!-- Hero Banner -->
<div class="hero-black-box mb-30">
  <div>
    <h2>ABOUT PIE SIG</h2>
    <p class="hero-intro-text">
      {{ site.data.about.tagline }}
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Overview Section -->
<div class="about-card mb-30">
  <h2 class="about-card-title">Who We Are</h2>
  <div class="about-card-body">
    {% for paragraph in site.data.about.overview %}
      <p>{{ paragraph }}</p>
    {% endfor %}
  </div>
</div>

<!-- Mission & Focus Grid -->
<div class="about-grid mb-35">
  
  <div class="about-card">
    <h3 class="about-card-title">Our Mission</h3>
    <ul class="about-list">
      {% for item in site.data.about.mission %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </div>

  <div class="about-card">
    <h3 class="about-card-title">Areas of Focus</h3>
    <div class="about-tags">
      {% for area in site.data.about.focus_areas %}
        <span class="about-tag">{{ area }}</span>
      {% endfor %}
    </div>
  </div>

</div>

<!-- Callout / Get Involved Box -->
<div class="res-callout-box">
  <h3 class="res-callout-title">Get Involved with PIE SIG</h3>
  <p class="res-callout-text">
    Whether you are an experienced drama educator or just curious about integrating music, speech, or roleplay into your language classes, we welcome you! Explore our <a href="/resources/" class="res-callout-link">Resources</a> or join the conversation on our social media channels.
  </p>
</div>