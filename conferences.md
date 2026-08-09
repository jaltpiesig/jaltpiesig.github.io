---
layout: default
title: Conferences & Events
permalink: /conferences/
---

<!-- Hero Banner -->
<div class="hero-black-box mb-35">
  <div>
    <h2>PIE SIG CONFERENCES & EVENTS</h2>
    <p class="hero-intro-text">
      Join our active community of educators at national JALT conferences, regional workshops, and international performance-in-education symposia.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Section 1: Upcoming Events -->
<section class="mb-40">
  <h2 class="section-title">Upcoming Conferences & Workshops</h2>
  <div class="conf-grid">
    {% if site.data.conferences.upcoming %}
      {% for event in site.data.conferences.upcoming %}
        <div class="conf-card conf-card-upcoming">
          <div class="conf-badge-date">{{ event.date }}</div>
          <h3 class="conf-title">{{ event.title }}</h3>
          <div class="conf-location">📍 {{ event.location }}</div>
          <p class="conf-description">{{ event.description }}</p>
          {% if event.url %}
            <a href="{{ event.url }}" class="conf-btn" target="_blank" rel="noopener">Learn More & Register →</a>
          {% endif %}
        </div>
      {% endfor %}
    {% else %}
      <div class="conf-card">
        <p class="conf-description">Check back soon for upcoming conference announcements and call for proposals!</p>
      </div>
    {% endif %}
  </div>
</section>

<!-- Section 2: Past / Archive Events -->
<section class="mb-40">
  <h2 class="section-title">Past Events & Conference Archives</h2>
  <div class="conf-grid">
    {% for event in site.data.conferences.past %}
      <div class="conf-card">
        <div class="conf-badge-date conf-badge-past">{{ event.date }}</div>
        <h3 class="conf-title">{{ event.title }}</h3>
        <div class="conf-location">📍 {{ event.location }}</div>
        {% if event.summary %}
          <p class="conf-description">{{ event.summary }}</p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>

<!-- Section 3: Proposal / Callout Box -->
<div class="res-callout-box">
  <h3 class="res-callout-title">Presenting with PIE SIG</h3>
  <p class="res-callout-text">
    Interested in hosting a workshop or presenting a performance-based paper under the PIE SIG banner? Contact our events coordinator or keep an eye out for our annual JALT National Call for Papers.
  </p>
</div>