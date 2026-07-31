---
layout: default
title: Home
---

<!-- Top Hero Grid: Intro Paragraph Left, Brand Title Right -->
<div class="hero-grid">
  <p class="intro-text">
    The Performance in Education (PIE) Special Interest Group (SIG) of the Japan Association for Language Teaching (JALT), founded in 2011 as the Speech, Drama, & Debate SIG, is involved with a myriad of teaching activities (still including drama and debate, but now much more!) that require students to cooperate and collaborate together, so it is natural that our SIG also participates in many collaborative activities with JALT chapters and SIGs.
  </p>

  <div class="brand-title-box">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<h2 class="section-title">Podcast</h2>

<!-- Podcast Grid: Player Card Left, Text & Stylized Logo Right -->
<div class="podcast-grid">
  <div class="podcast-player-card">
    <p><strong>PIE SIG Podcast Episode 12</strong></p>
    <p style="font-size:0.85rem; color:#555; margin-bottom:10px;">Why Settle for Student Participation When You Can Have Student Engagement?</p>
    <a href="https://open.spotify.com" target="_blank" style="display:inline-block; background:#1db954; color:#fff; padding:6px 14px; border-radius:15px; text-decoration:none; font-size:0.8rem; font-weight:bold;">Listen on Spotify</a>
  </div>

  <div class="podcast-info-side">
    <p>The PIE SIG Podcast features conversations with educators who use performance to make language teaching more engaging, creative, and effective. New episodes are released monthly.</p>
    <p>Listen on the PIE SIG website or Spotify, and follow along so you never miss one!</p>
    
    <!-- Stylized PIE Pod Logo -->
    <div class="pie-pod-logo-wrapper">
      <div class="pie-pod-text-logo">
        PIE
        <span>pod</span>
        <sub>PODCAST IN EDUCATION</sub>
      </div>
    </div>
  </div>
</div>

<!-- News Header Bar with Social Media Circles -->
<div class="news-header-bar">
  <h2>NEWS</h2>
  <div class="social-icons-group">
    <a href="#" class="social-icon" title="Facebook">f</a>
    <a href="#" class="social-icon" title="YouTube">yt</a>
    <a href="#" class="social-icon" title="X / Twitter">x</a>
    <a href="#" class="social-icon" title="LinkedIn">in</a>
  </div>
</div>

<!-- News List -->
<div class="news-list">
  {% for post in site.posts limit:5 %}
    <div class="news-post-item">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <span class="news-post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <p class="news-post-excerpt">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    </div>
  {% endfor %}
</div>

<!-- Bottom Banners (3 Side-by-Side Boxes for Partners) -->
<div class="footer-partner-logos">
  <div class="partner-box">
    <img src="/assets/images/beyond-classroom-logo.png" alt="Beyond the Classroom" onerror="this.parentNode.innerHTML='BEYOND THE CLASSROOM';">
  </div>
  <div class="partner-box">
    <img src="/assets/images/pansig-logo.png" alt="PanSIG Chukyo University" onerror="this.parentNode.innerHTML='PanSIG CHUKYO UNIVERSITY';">
  </div>
  <div class="partner-box">
    <img src="/assets/images/jalt-logo.png" alt="JALT" onerror="this.parentNode.innerHTML='JALT';">
  </div>
</div>