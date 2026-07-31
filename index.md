---
layout: default
title: Home
---

<!-- Top Hero Grid: Intro Text Left, Black PIE SIG Box Right -->
<div class="hero-grid">
  <p class="intro-text">
    The Performance in Education (PIE) Special Interest Group (SIG) of the Japan Association for Language Teaching (JALT), founded in 2011 as the Speech, Drama, & Debate SIG, is involved with a myriad of teaching activities (still including drama and debate, but now much more!) that require students to cooperate and collaborate together, so it is natural that our SIG also participates in many collaborative activities with JALT chapters and SIGs.
  </p>

  <div class="dark-brand-box">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<h2 class="section-title">Podcast</h2>

<!-- Podcast Grid: Media Player Left, Short Intro Text & Stylized Logo Right -->
<div class="podcast-grid">
  <div class="podcast-player">
    <iframe style="border-radius:12px" src="https://open.spotify.com/embed/show/3vU4S1oGkQ4Y9Z2H2eU7Gg?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  </div>

  <div class="podcast-info-side">
    <p>The PIE SIG Podcast features conversations with educators who use performance to make language teaching more engaging, creative, and effective. New episodes are released monthly.</p>
    <p>Listen on the PIE SIG website or Spotify, and follow along so you never miss one!</p>
    <img src="/assets/images/pie-pod-logo.png" alt="PIE pod" class="pie-pod-stylized-logo" onerror="this.src='https://via.placeholder.com/190x100?text=PIE+pod+Logo'">
  </div>
</div>

<!-- News Section Header with Dark Band and Social Media Icons -->
<div class="news-header-bar">
  <h2>News</h2>
  <div class="social-icons-group">
    <a href="#" class="social-icon" title="Facebook">f</a>
    <a href="#" class="social-icon" title="YouTube">yt</a>
    <a href="#" class="social-icon" title="X / Twitter">x</a>
    <a href="#" class="social-icon" title="LinkedIn">in</a>
  </div>
</div>

<!-- News Articles List -->
<div class="news-list">
  {% for post in site.posts limit:5 %}
    <div class="news-post-item">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <span class="news-post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <p class="news-post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    </div>
  {% endfor %}
</div>

<!-- Bottom Partner Logos Grid (Beyond the Classroom, PanSIG, JALT) -->
<div class="footer-partner-logos">
  <div class="partner-logo-box">
    <img src="/assets/images/beyond-classroom-logo.png" alt="Beyond the Classroom 2026" onerror="this.src='https://via.placeholder.com/220x80?text=Beyond+The+Classroom'">
  </div>
  <div class="partner-logo-box">
    <img src="/assets/images/pansig-logo.png" alt="PanSIG Chukyo University" onerror="this.src='https://via.placeholder.com/220x80?text=PanSIG+Chukyo+Univ'">
  </div>
  <div class="partner-logo-box">
    <img src="/assets/images/jalt-logo.png" alt="JALT" onerror="this.src='https://via.placeholder.com/220x80?text=JALT+Logo'">
  </div>
</div>