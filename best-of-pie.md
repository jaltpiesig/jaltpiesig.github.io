---
layout: default
title: Best of PIE SIG
permalink: /best-of-pie-sig/
---

<!-- Hero Banner -->
<div class="hero-black-box mb-35">
  <div>
    <h2>BEST OF PIE SIG</h2>
    <p class="hero-intro-text">
      A curated collection celebrating outstanding research, creative lesson ideas, and teacher reflections published across 10+ years of Performance in Education.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Main Publication Card -->
<div class="pub-journal-card mb-40">
  <h2 class="pub-journal-title">The Best of Performance in Education</h2>
  <div class="pub-issn">Special Commemorative Anthology Series</div>
  
  <p class="pub-description">
    Bringing together benchmark papers, innovative drama frameworks, and practical speech & debate guides into landmark collections. Available for free download in PDF format.
  </p>

  <div class="pub-metadata-grid">
    <div><strong>Publisher:</strong> JALT Performance in Education SIG</div>
    <div><strong>Format:</strong> Digital PDF (Open Access)</div>
  </div>

  <!-- Volume 1 -->
  <div class="pub-volume-card">
    <div class="pub-volume-header">
      <h3 class="pub-volume-title">Volume 1 (10th Anniversary Issue)</h3>
      {% if site.data.best_of_pie.vol1_pdf %}
        <a href="{{ site.data.best_of_pie.vol1_pdf }}" class="pub-pdf-btn" target="_blank" rel="noopener">Download PDF</a>
      {% endif %}
    </div>

    <ul class="pub-chapter-list">
      {% for chapter in site.data.best_of_pie.vol1_chapters %}
        <li class="pub-chapter-item">
          <div class="pub-chapter-title">{{ chapter.title }}</div>
          <div class="pub-chapter-author">by {{ chapter.author }}</div>
          <div class="pub-chapter-meta">
            <span class="pub-tag">{{ chapter.category | default: "Article" }}</span>
            {% if chapter.pages %}<span class="pub-pages">pp. {{ chapter.pages }}</span>{% endif %}
          </div>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<!-- Callout / Submission Box -->
<div class="res-callout-box">
  <h3 class="res-callout-title">Submit to Future Editions</h3>
  <p class="res-callout-text">
    Have you published an article in our publications or presented at a PIE SIG event? Contact our publications chair to learn about upcoming anthology selection criteria and submission windows.
  </p>
</div>