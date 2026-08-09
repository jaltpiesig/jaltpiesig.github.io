---
layout: default
title: Publications
permalink: /publications/
---

<!-- Hero Banner -->
<div class="hero-black-box mb-35">
  <div>
    <h2>PIE SIG PUBLICATIONS</h2>
    <p class="hero-intro-text">
      Explore peer-reviewed journals, special anthology volumes, and collaborative publications produced by the Performance in Education SIG.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Section 1: Main Academic Journals -->
<section class="mb-40">
  <h2 class="section-title">Peer-Reviewed Journals & Publications</h2>

  <!-- Journal Card: Mask & Gavel -->
  <div class="pub-journal-card mb-30">
    <h3 class="pub-journal-title">Mask & Gavel</h3>
    <div class="pub-issn">ISSN: 2188-4609 (Online)</div>
    
    <p class="pub-description">
      The primary peer-reviewed publication of the PIE SIG, featuring research articles, practical teaching ideas, book reviews, and creative reflections on speech, drama, debate, and performance in language learning.
    </p>

    <div class="pub-metadata-grid">
      <div><strong>Editor-in-Chief:</strong> PIE SIG Editorial Board</div>
      <div><strong>Frequency:</strong> Annual / Bi-Annual</div>
      <div><strong>Access:</strong> Open Access (Digital PDF)</div>
      <div><strong>Scope:</strong> Speech, Drama, Debate & Oral Interpretation</div>
    </div>

    <!-- Volume / Issues Container -->
    <div class="pub-volume-card">
      <div class="pub-volume-header">
        <h4 class="pub-volume-title">Featured Issue: Volume 9 (Latest Release)</h4>
        {% if site.data.publications.latest_issue_pdf %}
          <a href="{{ site.data.publications.latest_issue_pdf }}" class="pub-pdf-btn" target="_blank" rel="noopener">Download Full PDF</a>
        {% endif %}
      </div>

      <ul class="pub-chapter-list">
        {% for article in site.data.publications.latest_articles %}
          <li class="pub-chapter-item">
            <div class="pub-chapter-title">{{ article.title }}</div>
            <div class="pub-chapter-author">by {{ article.author }}</div>
            <div class="pub-chapter-meta">
              <span class="pub-tag">{{ article.type | default: "Research Article" }}</span>
              {% if article.pages %}<span class="pub-pages">pp. {{ article.pages }}</span>{% endif %}
            </div>
          </li>
        {% endfor %}
      </ul>
    </div>

    <div class="mt-15">
      <a href="/mask-and-gavel/" class="conf-btn">Browse Full Mask & Gavel Archives →</a>
    </div>
  </div>

  <!-- Journal Card: Best of PIE SIG Anthology -->
  <div class="pub-journal-card">
    <h3 class="pub-journal-title">The Best of Performance in Education</h3>
    <div class="pub-issn">Special Commemorative Series</div>
    
    <p class="pub-description">
      A landmark collection highlighting benchmark papers and practical performance frameworks selected from a decade of PIE SIG contributions.
    </p>

    <div class="pub-metadata-grid">
      <div><strong>Publisher:</strong> JALT Performance in Education SIG</div>
      <div><strong>Format:</strong> Digital Anthology (PDF)</div>
    </div>

    <a href="/best-of-pie-sig/" class="conf-btn">Explore Anthology & Articles →</a>
  </div>
</section>

<!-- Section 2: Special Collaborations -->
<section class="mb-40">
  <h2 class="section-title">Special Collaborations & Joint Publications</h2>
  <div class="collab-grid">
    {% for collab in site.data.publications.collaborations %}
      <div class="collab-card">
        <span class="collab-partner">{{ collab.partner }}</span>
        <h4 class="collab-title">{{ collab.title }}</h4>
        <div class="collab-date">{{ collab.date }}</div>
        {% if collab.description %}
          <p class="news-post-excerpt mt-10">{{ collab.description }}</p>
        {% endif %}
        {% if collab.url %}
          <a href="{{ collab.url }}" class="res-callout-link mt-10" style="display:inline-block;" target="_blank" rel="noopener">Read Issue →</a>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>

<!-- Section 3: Call for Papers Callout -->
<div class="res-callout-box">
  <h3 class="res-callout-title">Call for Papers & Submissions</h3>
  <p class="res-callout-text">
    We welcome submissions year-round from researchers, teachers, and performance practitioners. Check out our submission guidelines to submit your research paper, practical lesson plan, or performance review.
  </p>
</div>